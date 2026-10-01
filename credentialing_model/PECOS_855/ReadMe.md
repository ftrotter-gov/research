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
- 🚧 **855B** - In Progress (modular architecture, Section 1 complete)
- ⏳ **855A, 855I, 855S** - Planned

## References

- Form PDFs: `CoreDM/forms/`
- Field Analysis: `CoreDM/forms_analysis/*_enhanced.csv`
- Form.io Documentation: <https://help.form.io/>
