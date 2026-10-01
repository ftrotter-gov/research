# Forms.io JSON Form Implementation of the 855 Forms

This directory contains Form.io implementations of CMS-855 Medicare enrollment forms.

## Architecture

### Simple Forms (855O)

Small forms like the 855O use a single-file architecture:

- `855o_index.html` - HTML wrapper that loads the form
- `855o.json` - Complete form definition

**Example:** See `CoreDM/formio/855o_index.html` and `CoreDM/formio/855o.json`

### Complex Forms (855B) - Modular Architecture

Large forms like the 855B use a modular architecture with separate section files:

```
CoreDM/formio/855b/
├── 855b_index.html          # Main HTML file with async loader
├── wizard.json              # Wizard configuration listing all sections
└── section_json/            # Individual section definitions
    ├── section1.json        # Section 1: Basic Information
    ├── section2.json        # Section 2: Identifying Information
    ├── section3.json        # Section 3: Final Adverse Legal Actions
    └── ...                  # Additional sections as needed
```

#### Modular Architecture Benefits

1. **Maintainability**: Each section can be edited independently
2. **Collaboration**: Multiple developers can work on different sections
3. **Reusability**: Sections can be reused across similar forms
4. **Version Control**: Easier to track changes to specific sections
5. **Testing**: Individual sections can be tested in isolation

#### How the Modular Architecture Works

1. **wizard.json** - Configuration file that lists all section files:

```json
{
  "display": "wizard",
  "title": "CMS-855B Medicare Enrollment Application",
  "pageFiles": [
    "section_json/section1.json",
    "section_json/section2.json"
  ]
}
```

2. **Section JSON Files** - Each contains form components for one section:

```json
{
  "title": "Section 1: Basic Information",
  "key": "section1BasicInformation",
  "components": [
    // Form components here
  ]
}
```

3. **HTML File** - Loads sections asynchronously and builds the wizard:

```javascript
async function buildWizard() {
  const wrapper = await (await fetch('./wizard.json')).json();
  const pages = await Promise.all(
    wrapper.pageFiles.map(p => fetch(p).then(r => r.json()))
  );
  return {
    display: "wizard",
    title: wrapper.title,
    components: pages.map((page, i) => ({
      type: "panel",
      title: page.title || `Page ${i+1}`,
      key: page.key || `page${i+1}`,
      components: page.components || []
    }))
  };
}
```

## Implementation Guidelines

### For All Forms

1. Use the CDN for all JavaScript and CSS
2. Find the PDF form in `CoreDM/forms/`
3. Use the **enhanced CSV** from `CoreDM/forms_analysis/` for field reference
4. Do not mark fields as "required" initially (for faster testing)
5. Use Python's HTTP server for local testing: `python3 -m http.server 8855`

### Form Naming Convention

- HTML file: `{form_number}_index.html` (e.g., `855o_index.html`)
- Simple forms: `{form_number}.json` (e.g., `855o.json`)
- Complex forms: Use subdirectory structure (e.g., `855b/`)

### When to Use Modular Architecture

Use modular architecture when:

- Form has more than 5 major sections
- Form has more than 200 fields
- Multiple developers will work on the form
- Sections may be reused in other forms

Use single-file architecture when:

- Form is relatively simple (< 5 sections)
- Form has fewer than 200 fields
- Quick prototyping is needed

## Testing

1. Start the HTTP server:

```bash
cd CoreDM/formio
python3 -m http.server 8855
```

2. Open browser to:
   - Simple forms: `http://localhost:8855/855o_index.html`
   - Modular forms: `http://localhost:8855/855b/855b_index.html`

## Form Status

- ✅ **855O** - Complete (simple architecture)
- ✅ **855I** - Complete (modular architecture, all 15 sections)
- 🚧 **855B** - In Progress (modular architecture, Section 1 complete)
- ⏳ **855A, 855S** - Planned

### 855I Notes

The CMS-855I (rev. 05/23) models physicians and non-physician practitioners:

- **No attachments.** Unlike the 855A (1 attachment) and 855B (3 attachments), the
  855I has none; the form is Sections 1-15 only.
- **Blank sections are included as stubs.** Sections 5, 7, 9, 10, and 11 are marked
  "This Section Intentionally Left Blank" on the paper form. They are included as stub
  pages (the 855A convention) so that wizard page numbers match the paper form.
- **The CMS-855R is discontinued.** All reassignment-of-benefits actions are now
  reported in Section 4F, so the 855I's Section 12 has no CMS-855R checkbox.
- **Section 2G (Physician Specialty)** carries all 71 specialty labels from the PDF.
  The paper form marks each with P=Primary / S=Secondary; this is modeled as one
  `select` for the primary specialty plus one `multiple: true` `select` for secondary
  specialties, rather than 142 individual controls. Specialty value slugs match those
  already used in `855o.json`.
- **Fixed-count PDF tables use unbounded `datagrid`s.** The paper form allocates a
  fixed number of rows (e.g. 3 adverse-action rows, 12 + 4 home-service location rows).
  These are modeled as `datagrid`s, consistent with how the 855A/855B handled the
  equivalent tables.
- **Sections 2G-2K are conditionally gated.** A `practitionerType` discriminator shows
  Section 2G for physicians and Section 2H for non-physician practitioners; Sections 2I
  (Psychologist), 2J (PT/OT), and 2K (CNS/NP) appear only for the relevant specialty
  types selected in 2H.
- **New component types.** The 855I is the first form here to use `container` (to scope
  conditionally-shown address blocks) and `signature` (Section 15 signatures). Both are
  core Form.io types.

### The "(Shows new form) ◿" convention

*Applies to all four forms: 855A, 855B, 855I, 855O.*

On paper, these forms say things like "Go to Section 1B below" — an instruction that
makes no sense in a wizard, where the target is hidden until you trigger it. Conditional
sections therefore *look* missing.

To fix this, every option that **reveals** additional fields has the suffix
`(Shows new form) ◿` appended to its label, where `◿` is the Lower Right Triangle
character (U+25FF, `&#9727;` / `&#x25FF;`).

| Form | Markers |
|------|---------|
| 855A | 20 |
| 855B | 62 |
| 855I | 43 |
| 855O | 10 |
| **Total** | **135** |

Implementation notes:

- The marker lives entirely in the **JSON labels** — there is no supporting JavaScript
  or CSS. This keeps the indicator visible in the underlying data, so it survives schema
  export and stays greppable: `grep -c '(Shows new form)' section_json/*.json`
- An earlier version wrapped the marker in a green `<span>` via a DOM-walking script in
  `855i_index.html`. That was removed: it added fragile client-side machinery (a
  `TreeWalker` plus a `MutationObserver` to survive conditional reveals) for a purely
  cosmetic gain, and it hid the marker from anyone reading the JSON directly.
- Only *revealing* options are marked. Triggers that **hide** content when selected are
  deliberately left unmarked, since marking them would be actively misleading. In the
  855I these are `licenseNotApplicable`, `certificationNotApplicable`, `deaNotApplicable`,
  `medicalRecordSameAsCorrespondence`, `recordsStoredAtPracticeLocation`,
  `iAmTheManagingEmployee`, and `billingAgencyNotApplicable`. The 855I's
  `practiceArrangement` radio is also unmarked: all three of its options are `show: false`
  conditions that *narrow* which sub-sections apply rather than revealing new ones.
- Markers were applied by analysing each form's `conditional` blocks programmatically
  (including `json`-logic conditions), not by hand, so coverage is exhaustive. To
  re-derive or audit them, see the analysis approach described above.

## References

- Form PDFs: `CoreDM/forms/`
- Field Analysis: `CoreDM/forms_analysis/*_enhanced.csv`
- Form.io Documentation: <https://help.form.io/>
