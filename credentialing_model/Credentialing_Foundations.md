# Credentialing Foundations

**Scope:** U.S. credentialing of individual clinicians, with emphasis on hospitals, health plans, primary-source verification, accreditation, and credentialing infrastructure.  
**Status:** Working background reference; NPD design implications intentionally excluded.  
**Last updated:** October 1, 2026.

---

## 1. The General Regulatory Pattern

There is no single national credentialing statute, regulator, or universally binding list of “trusted credential sources.” Credentialing obligations arise from several overlapping layers of authority. The applicable stack depends on the organization doing the credentialing and the purpose of the credentialing decision.

### Hospital / clinical privileges stack

```text
Federal statute and regulation
        ↓
CMS Conditions of Participation
        ↓
State hospital + professional licensure / scope-of-practice law
        ↓
Accreditation / deemed-status standards (for example, Joint Commission)
        ↓
Hospital medical-staff bylaws, credentialing policies, and privileging criteria
        ↓
Primary-source / recognized-source verification
        ↓
Medical-staff recommendation
        ↓
Hospital governing-body appointment and privileging decision
```

### Health-plan / network participation stack

```text
Federal program rules (when applicable: MA, Medicaid, etc.)
        +
State insurance / managed-care / professional-practice law
        ↓
Accreditation and contractual requirements (often NCQA or another accreditor)
        ↓
Plan credentialing policies and delegated-credentialing arrangements
        ↓
Primary-source / recognized-source verification, often performed by a CVO
        ↓
Credentialing committee / plan governance
        ↓
Network participation decision
```

The critical conceptual point is that **the organization that creates the duty to verify is often different from the organization that supplies the underlying evidence**. A statute, regulation, accreditor, state Medicaid contract, or payer policy may require verification; a state licensing board, specialty board, training program, federal database, or qualifying verification intermediary may then supply the evidence.

---

## 2. What Makes a Source “Trusted,” and Who Blesses the Trust?

“Trusted source” should not be treated as a universal property of an organization. Trust is normally **attribute-specific and rule-specific**.

A useful model is:

```text
Credential fact being tested
        ↓
Entity that legally or institutionally creates that fact
        ↓
Primary source
        ↓
Any recognized equivalent source, approved agent, or qualifying CVO
        ↓
Rule / accreditor / regulator that permits that verification path
        ↓
Credentialing organization’s documented verification
        ↓
Separate credentialing / privileging / participation decision
```

For example:

- A **state medical board** is authoritative for the license it issues and actions it takes on that license.
- An **ABMS member board** is authoritative for the board certification it issues; ABMS may serve as a recognized verification channel for certification by its member boards.
- A **medical school or residency program** is the underlying source of education or training completion; a recognized intermediary may be permitted to verify that fact.
- The **NPDB** is a federally established repository for specified reportable events. It is not the issuer of a medical license or specialty certification.
- A **CVO** can perform verification work, but its authority derives from the quality and provenance of its verification process and from the rules that permit the credentialing organization to rely on it.

Accordingly, the right question is not simply “Is source X trusted?” but:

1. **What specific fact is being verified?**
2. **Who created or controls that fact?**
3. **What law, regulation, accreditation standard, contract, or policy requires it to be verified?**
4. **Does that governing regime require direct primary-source verification, or permit an approved agent, recognized source, designated equivalent source, or CVO?**
5. **What evidence of verification, provenance, date, and result must be retained?**
6. **Who remains legally or contractually responsible for the final credentialing decision?**

This produces a more accurate model of trust:

> **Source × Attribute × Governing Rule × Time**

rather than a static “trusted / untrusted” whitelist.

---

## 3. Hospitals: CMS Conditions of Participation

The federal starting point for Medicare-participating hospitals is the **Hospital Conditions of Participation (CoPs)**.

### 3.1 Medical-staff credential review

[42 CFR § 482.22 — Condition of participation: Medical staff](https://www.law.cornell.edu/cfr/text/42/482.22) requires a hospital to have an organized medical staff operating under bylaws approved by the governing body. Among other things, the medical staff must:

- examine the credentials of eligible candidates for medical-staff membership;
- make recommendations to the governing body concerning appointment;
- operate consistently with state law, including scope-of-practice law; and
- maintain bylaws describing qualifications for appointment and criteria and procedures for granting individual clinical privileges.

This federal rule therefore creates a **credentialing and privileging governance obligation**, but it does not itself create a single nationwide approved-source list for every credential element.

The hospital’s process is further informed by CMS interpretive guidance in the **State Operations Manual, Appendix A — Survey Protocol, Regulations and Interpretive Guidelines for Hospitals**. The current CMS materials are available through the [CMS State Operations Manual](https://www.cms.gov/medicare/health-safety-standards/guidance-for-laws-regulations/hospitals) and related survey guidance.

### 3.2 Role of state law

Section 482.22 repeatedly incorporates **state law**, including scope-of-practice requirements. State law may affect, among other things:

- who may be appointed to a medical staff;
- who may receive particular clinical privileges;
- which professions require licensure, certification, or registration;
- scope-of-practice limits;
- hospital licensing requirements;
- peer-review requirements and protections;
- credentialing application or timing requirements; and
- the status and evidentiary role of state professional boards.

Thus, even where federal CoPs establish the overall obligation, the hospital must evaluate the clinician against the law of the state in which the hospital operates.

---

## 4. Deeming: How CMS Requirements Connect to the Joint Commission

### 4.1 Statutory basis

The principal statutory basis for Medicare accreditation-based deeming is [42 U.S.C. § 1395bb (Social Security Act § 1865) — Effect of accreditation](https://www.law.cornell.edu/uscode/text/42/1395bb).

The statute permits the Secretary to treat an accredited provider entity as meeting applicable Medicare conditions when the Secretary finds that the accrediting body’s accreditation demonstrates that the federal requirements are met or exceeded. The statute directs the Secretary to consider the accreditor’s standards, survey procedures, resources, monitoring processes, and ability to provide information for enforcement and validation.

CMS implements the accrediting-organization approval framework in [42 CFR Part 488](https://www.law.cornell.edu/cfr/text/42/part-488), including [42 CFR § 488.5](https://www.law.cornell.edu/cfr/text/42/488.5), which governs applications and reapplications by national accrediting organizations.

CMS describes the practical effect as follows: most covered provider and supplier types may demonstrate compliance with Medicare health and safety requirements through a **CMS-approved accreditation organization (AO)** rather than a state survey agency. CMS refers to this as **deemed status**. See [CMS — Accrediting Organizations](https://www.cms.gov/medicare/health-safety-standards/quality-safety-oversight-general-information/accrediting-organizations-aos).

### 4.2 Why Joint Commission standards matter

The [Joint Commission](https://www.jointcommission.org/) is one of the national AOs whose applicable accreditation programs are approved by CMS. A hospital that chooses the Joint Commission deeming pathway is therefore not merely adopting a private trade association’s suggestions. It is choosing an accreditation program that operates within a federal statutory and regulatory mechanism for demonstrating compliance with Medicare requirements.

The Joint Commission explains the deeming framework in its [Federal Deemed Status FAQ](https://www.jointcommission.org/en-us/knowledge-library/support-center/survey-or-review-preparation/deemed-status). CMS retains oversight: accreditation does not eliminate CMS authority, and CMS conducts validation and complaint activity and may determine that a provider does not satisfy federal requirements notwithstanding accreditation.

### 4.3 The basic enforcement chain

```text
Medicare participation requirement
        ↓
CMS CoPs
        ↓
Hospital chooses State Survey Agency path OR CMS-approved AO path
        ↓
If AO path: Joint Commission surveys against applicable approved standards
        ↓
Deficiencies can require correction / affect accreditation or the hospital’s deeming status
        ↓
CMS retains validation, complaint, certification, and enforcement authority
```

This explains why an accreditation requirement can have practical regulatory force even when the detailed credentialing requirement is written in an accreditation manual rather than directly in the CFR.

---


## 5. CMS-Approved Hospital Accrediting Organizations for Deeming: How They Differ

CMS approval is **program-specific**: an accrediting organization can have deeming authority for one provider type without having it for another. The current CMS overview of approved accrediting organizations is at [CMS — Accrediting Organizations](https://www.cms.gov/medicare/health-safety-standards/quality-safety-oversight-general-information/accrediting-organizations-aos). For the acute-care hospital program, the principal CMS-approved national accrediting organizations are **The Joint Commission (TJC), DNV Healthcare (DNV), the Center for Improvement in Healthcare Quality (CIHQ), and the Accreditation Commission for Health Care (ACHC)**. CMS reporting has separately identified these organizations as hospital deeming programs, and each currently maintains a hospital accreditation program used for Medicare deeming.

This comparison should not be generalized automatically to psychiatric hospitals, critical access hospitals, ambulatory surgical centers, laboratories, or other provider types; CMS approval must be checked for the particular program.

| Accrediting organization | Hospital accreditation model and credentialing emphasis | Practical contrast |
|---|---|---|
| [The Joint Commission](https://www.jointcommission.org/) | Uses a broad hospital accreditation framework with a dedicated Medical Staff chapter and extensive public interpretive guidance on credentialing, privileging, primary-source verification, CVOs, practitioner identification, telemedicine, and privilege design. Its current [Primary Source Verification FAQ](https://www.jointcommission.org/en-us/knowledge-library/support-center/standards-interpretation/standards-faqs/000001472) defines PSV and places responsibility on the accredited organization for determining whether an equivalent source/CVO is acceptable. | For this research, TJC is particularly important because it has historically published unusually explicit credential-source guidance, including former lists of “designated equivalent sources,” making its standards useful for tracing how a particular verification source becomes acceptable. |
| [DNV Healthcare](https://www.dnv.com/healthcare/) | DNV’s U.S. hospital program uses its [NIAHO® accreditation model](https://www.dnv.com/services/niaho-accreditation-for-acute-care-hospitals/), which aligns hospital requirements with the CMS Conditions of Participation and integrates ISO 9001 quality-management principles. DNV conducts annual surveys within a three-year accreditation cycle and emphasizes continuous quality-management systems rather than episodic survey preparation. | DNV must still satisfy the same underlying CMS CoPs, including medical-staff credentialing and privileging requirements, but embeds those requirements in a broader ISO-style quality-management architecture. The principal difference is therefore more about the accreditation and quality-management model than permission to ignore or substitute for federal credentialing duties. |
| [Center for Improvement in Healthcare Quality (CIHQ)](https://cihq.org/acc-default-hospitals.asp) | CIHQ states that CMS accepts its accreditation to deem acute-care hospitals compliant with the Hospital CoPs. Its hospital standards and survey materials are organized closely around Medicare participation requirements, with a stated collegial and educational survey approach. Current hospital accreditation materials are linked directly from its hospital program page. | CIHQ is comparatively CMS-CoP-centered and presents itself as a lower-complexity, educational alternative. Its credentialing rules still must be at least as stringent as the federal medical-staff requirements within the scope of CMS approval; its public source-specific credentialing guidance is less extensive than TJC’s public FAQ ecosystem. |
| [Accreditation Commission for Health Care (ACHC)](https://achc.org/hospital/) | ACHC’s hospital program incorporates the former HFAP hospital accreditation lineage following the 2020 ACHC/HFAP merger. Its published hospital standards require primary-source verification for specified credentials, NPDB querying, and documentation supporting requested privileges; ACHC expressly permits a CVO to perform PSV while requiring the hospital’s credentialing process to meet applicable standards. See also [ACHC — Verifying Personnel Credentials Is a Crucial Task for Hospitals](https://achc.org/verifying-hospital-credentials/). | ACHC’s published materials are comparatively prescriptive about several credential-file elements and identify concrete verification mechanisms and sources. Historically, HFAP was the hospital accreditor associated with the American Osteopathic Association; today the relevant hospital accreditation program is housed within ACHC. |

### 5.1 What all CMS-approved hospital AOs have in common

The AOs are not free to invent a credentialing regime below the federal floor. Under [42 U.S.C. § 1395bb](https://www.law.cornell.edu/uscode/text/42/1395bb) and [42 CFR § 488.5](https://www.law.cornell.edu/cfr/text/42/488.5), CMS reviews whether an AO’s standards and survey processes meet or exceed the applicable Medicare requirements. Thus every approved hospital AO must evaluate hospital compliance with the substance of the Hospital CoPs, including the medical-staff and privileging requirements in [42 CFR § 482.22](https://www.law.cornell.edu/cfr/text/42/482.22).

The differences among AOs principally concern **how the federal floor is operationalized and surveyed**: the specificity of accreditation standards, the organization of the standards, survey cadence and philosophy, additional quality-system requirements, documentation expectations, and the amount of interpretive guidance supplied to accredited hospitals.

### 5.2 Primary-source verification across the hospital deeming organizations

For credentialing, the most useful comparison is not simply whether an accrediting organization requires primary-source verification (PSV). All four operate above the same CMS floor. The more important questions are: **which credential elements must be verified; what counts as the primary source or an acceptable substitute; whether CVOs or equivalent sources may be used; and what surveyors actually inspect to enforce the requirement.**

| Deeming organization | Credential elements expressly subjected to PSV | Sources or substitute mechanisms expressly recognized in public materials | How the requirement is enforced |
|---|---|---|---|
| **The Joint Commission (TJC)** | Current hospital standards require written verification from the primary source whenever feasible, or from a qualifying CVO, for **current licensure, relevant training, and current competence** in the credentialing/privileging process. Its broader HR requirements also require PSV of licenses, certifications, or registrations that are legally required to practice. | The current [TJC PSV FAQ](https://www.jointcommission.org/en-us/knowledge-library/support-center/standards-interpretation/standards-faqs/000001472) defines PSV as verification by the **original source or an approved agent of that source**, and permits qualifying CVO reports. TJC no longer maintains its former list of named “designated equivalent sources.” An organization may use an equivalent source for education, board certification, or licensure if it determines that the source satisfies TJC's CVO criteria. Historical 2024 guidance named AMA Physician Professional Data, ABMS (for ABMS-member-board certification), ECFMG, AOA, FSMB, NCCPA, AAPA-profile information, and NBPAS for specified data elements. | TJC states that surveyors evaluate whether PSV was actually completed; merely placing a copy of a license in the file is insufficient. Its [Hospital Survey Activity Guide](https://www.jointcommission.org/-/media/tjc/documents/accred-and-cert/survey-process-and-survey-activity-guide/2025/2025-hospital-organization-sag_c.pdf) directs surveyors to discuss how PSV is performed for licensure, training, and competence and to evaluate credentialing files/processes. |
| **DNV Healthcare (NIAHO)** | DNV's NIAHO standards have expressly required PSV at initial appointment for **licensure, education, specific training, experience, current competence, required certifications, and—when applicable—DEA registration**; reappointment focuses again on current licensure, current competence, and required certifications. | DNV's April 2025 Revision 25-0 expressly treated an **AMA Master Profile** or **Osteopathic Physician Profile** as acceptable for specified verification and separately required ECFMG verification when applicable; it also required database profiles from sources such as AMA, AOA, NPDB, OIG, and Medicare/Medicaid exclusion sources. DNV states that [Revision 25-1](https://www.dnv.com/publications/niaho-requirements-revision-25-1-updated/) superseded prior revisions effective September 8, 2025. Because the current full manual is distributed through DNV's download form, source-specific statements should be checked against the current manual before treating the older named-source examples as unchanged. | NIAHO survey guidance directs surveyors to sample medical-staff appointment/reappointment records, verify the mechanism used to examine credentials, and determine whether the required appointment elements were reviewed. DNV's model also subjects hospitals to **annual surveys**, giving credentialing-process failures a recurring accreditation-review pathway rather than a once-per-three-year-only touchpoint. |
| **Accreditation Commission for Health Care (ACHC)** | ACHC's 2025 Acute Care Hospital standard 03.01.15 requires review/verification of licensure history, medical education and postgraduate training, malpractice history, specialty-board status, sanctions/discipline, criminal history, and hospital employment/affiliations as part of application and reapplication. | ACHC is unusually explicit. Its [2025 Acute Care Hospital requirements](https://achc.org/wp-content/uploads/2025/06/2025_Accred-Req-for-ACH_eff.07.01.2025.pdf) require PSV from **state licensing agencies** and identify **FSMB** or **FACIS** for specified disciplinary information; for training/education they expressly identify the **AMA Physician Profile, AOA Official Osteopathic Physician Profile, and ECFMG**, as applicable. ACHC allows a **CVO** to perform PSV, but the hospital remains responsible for ensuring the CVO process satisfies ACHC standards. ACHC's hospital guidance also states that licenses/certificates must be verified with the appropriate issuing licensing agency. | ACHC embeds enforcement directly into its scoring procedure: for standard 03.01.15, surveyors are instructed to review **no fewer than ten files** and verify consistent application of credentialing criteria, a summary of submitted and verified information, appropriate medical-staff/governing-body review, and practice within granted privileges. ACHC also warns that allowing practice without appropriate state licensure/certification may be grounds for loss of accreditation. |
| **Center for Improvement in Healthcare Quality (CIHQ)** | CIHQ's hospital standards are closely organized around the CMS Conditions of Participation. Its historical public standards expressly required primary-source verification for credentials required by federal, state, or local law and required the medical staff to examine credentials for appointment/reappointment. | CIHQ's [current hospital program page](https://cihq.org/acc-default-hospitals.asp) publishes links to its 2026 hospital standards and survey activity guide, but its current source-specific standards are less readily indexable than TJC's or ACHC's public guidance. I have not found a current CIHQ publication that functions as a named national-source whitelist comparable to TJC's historical list or ACHC's current named examples. Accordingly, the safer characterization is that CIHQ enforces the **primary-source requirement and the hospital's approved credentialing process**, with the precise acceptable source often determined by the credential itself, state law, and hospital policy rather than by a broad CIHQ source list. | CIHQ surveys the hospital against its CMS-aligned standards and the hospital's own approved credentialing process. A useful historical example is a CIHQ survey finding for failure to perform PSV and use current credential information; current CIHQ-accredited hospital policies also commonly operationalize CIHQ standards through file-level PSV. The current CIHQ survey guide should be treated as the controlling source when available. |

#### 5.2.1 What “blessing a source” actually means

The four AOs reveal at least four different mechanisms by which a credential source can become acceptable:

1. **The issuer itself is the primary source.** A state medical board is authoritative for the license it issues; a certifying board is authoritative for its own certification; a training program is authoritative for completion of its own training. No accreditor needs to create that underlying authority.
2. **An accreditor expressly names an intermediary or equivalent source.** ACHC currently does this for several sources; TJC historically did so through its designated-equivalent-source examples; DNV has also named specified profile services in its published NIAHO standards.
3. **An accreditor recognizes a class of intermediary rather than a named vendor.** TJC's current approach is the clearest example: an equivalent source may be used when the hospital determines it meets TJC's CVO criteria. In this model, the accreditor is blessing a **verification architecture**, not a permanent vendor list.
4. **The hospital defines the source within an accreditor-approved process.** Where an AO does not publish a detailed named-source list, the hospital must be able to demonstrate during survey that its selected source actually verifies the relevant credential from an authoritative source and that its written process satisfies the AO standard, CMS requirements, and state law.

This means that the phrase **“approved primary source” can be misleading**. A source can be acceptable because it is the original issuer, because an accreditor has specifically recognized it for a defined data element, because it qualifies as an agent/CVO of the primary source, or because the hospital can demonstrate that its verification chain meets the applicable standard. Acceptance is therefore **attribute-specific and rule-specific**, not a universal accreditation badge attached to an organization.

#### 5.2.2 Comparative enforcement pattern

Across the AOs, enforcement generally occurs through the accreditation survey rather than through a separate federal credential-source licensing regime. Surveyors review medical-staff bylaws and credentialing policies, sample credential files, compare the hospital's documentation to the accreditor's required elements, and cite deficiencies when required verification is absent, stale, improperly sourced, or inconsistent with the hospital's approved process. Deficiencies can require corrective action and, if sufficiently serious or unresolved, can threaten accreditation and therefore the hospital's continued reliance on accreditation for Medicare deeming. CMS separately retains validation and complaint-survey authority over the deeming process.

### 5.3 Joint Commission is especially important for source-of-truth analysis

For the credential-source question, TJC deserves disproportionate attention not because CMS has declared TJC superior to the other AOs, but because TJC has historically articulated the verification-source problem particularly explicitly. Its public guidance has addressed direct primary-source verification, approved agents, CVOs, and—historically—named “designated equivalent sources.” That makes TJC a useful case study for understanding the mechanism by which a downstream credentialing organization is permitted to rely on a source other than the original issuer.

DNV, CIHQ, and ACHC must nevertheless be examined in parallel because the acceptable verification architecture for a hospital depends on its chosen deeming organization as well as CMS requirements, state law, and the credential element being verified.

---

## 6. The Joint Commission and Primary-Source Verification

### 6.1 Current definition and responsibility

The Joint Commission’s current public guidance is its [Primary Source Verification FAQ](https://www.jointcommission.org/en-us/knowledge-library/support-center/standards-interpretation/standards-faqs/000001472).

As of its April 22, 2026 update, the Joint Commission states that primary-source verification (PSV) is used to confirm that an individual possesses a valid license, certification, or registration when required by law or regulation. It defines PSV as verification of a practitioner’s reported qualifications by the **original source or an approved agent of that source**. Acceptable mechanisms can include direct correspondence, documented telephone verification, secure electronic verification from the original source, or qualifying CVO reports.

The accredited organization—not the practitioner—is responsible for completing and documenting the verification. The documentation must establish such matters as the date of verification, who performed it, what was verified, and the result.

### 6.2 “Designated equivalent sources”: historical and current treatment

The Joint Commission’s approach has evolved.

In a March 6, 2024 notice, **Revised Glossary Definition of “Designated Equivalent Source,”** the Joint Commission described a designated equivalent source as a selected agency maintaining a specific credential item identical to the information at the primary source. Importantly, it stated that listing an organization did **not** constitute an endorsement and that “equivalent” did not mean that listed organizations used equally rigorous verification processes. See [Joint Commission Online — March 6, 2024](https://www.jointcommission.org/en-us/knowledge-library/newsletters/joint-commission-online/06-mar-24).

The 2024 examples included:

- AMA Physician Professional Data for specified U.S./Puerto Rico medical-school graduation and postgraduate education completion;
- ABMS for certification by an ABMS member board;
- ECFMG for foreign medical-school graduation;
- AOA Physician Database for specified osteopathic education, training, and specialty certification;
- FSMB for actions against a physician’s medical license;
- AAPA Profile / AMA Physician Profile Service for specified PA education information;
- NCCPA for PA certification; and
- NBPAS for NBPAS certification.

The **current 2026 Joint Commission FAQ explicitly says that the Joint Commission no longer maintains a glossary definition containing examples of designated equivalent sources**. Instead, an accredited organization may use an equivalent source for education, board certification, and licensure if the organization can determine that the source meets the Joint Commission’s criteria for a CVO. See the [current PSV FAQ](https://www.jointcommission.org/en-us/knowledge-library/support-center/standards-interpretation/standards-faqs/000001472).

This evolution is important. It shifts the model away from a simple published Joint Commission whitelist and toward **organizational responsibility for evaluating the verification intermediary**.

### 6.3 Earlier Joint Commission guidance as a historical comparison

An earlier version of the Joint Commission FAQ, preserved at [Joint Commission — Hospital and Hospital Clinics / Medical Staff / PSV](https://www.jointcommission.org/standards/standard-faqs/hospital-and-hospital-clinics/medical-staff-ms/000001357/), expressly referred to selected agencies as “designated equivalent sources” and pointed users to glossary examples.

The difference between that earlier formulation and the current 2026 FAQ is useful evidence of the change in approach.

---

## 7. National Practitioner Data Bank (NPDB)

The [National Practitioner Data Bank (NPDB)](https://www.npdb.hrsa.gov/) is a federal information repository administered by HRSA. Its legal framework principally derives from the **Health Care Quality Improvement Act of 1986 (HCQIA), Title IV of Public Law 99-660**, together with later statutory authorities consolidated in [45 CFR Part 60](https://www.law.cornell.edu/cfr/text/45/part-60).

The NPDB is unusual in the credentialing ecosystem because federal law directly imposes both **querying** and **reporting** duties in specified circumstances.

### 7.1 Mandatory hospital queries

Under [42 U.S.C. § 11135](https://www.law.cornell.edu/uscode/text/42/11135) and [45 CFR § 60.17](https://www.law.cornell.edu/cfr/text/45/60.17), a hospital must request NPDB information concerning a health care practitioner:

1. when the practitioner applies for medical-staff membership, including courtesy staff, or for clinical privileges; and
2. every two years for a practitioner who remains on the medical staff or has clinical privileges.

Hospitals may query at other times as well.

**Consequence of failing to query:** the statute and regulation provide that, in a medical-malpractice action, a hospital that failed to make the required query is presumed to have knowledge of information that had been reported to the NPDB concerning the practitioner. Conversely, a hospital may rely on NPDB information and generally is not liable for that reliance unless it knows the information is false. See [42 U.S.C. § 11135(b)-(c)](https://www.law.cornell.edu/uscode/text/42/11135) and [45 CFR § 60.17(b)-(c)](https://www.law.cornell.edu/cfr/text/45/60.17).

### 7.2 Required adverse-clinical-privileges reports

Under [42 U.S.C. § 11133](https://www.law.cornell.edu/uscode/text/42/11133) and [45 CFR § 60.12](https://www.law.cornell.edu/cfr/text/45/60.12), a health care entity must report specified actions involving physicians and dentists, including:

- a professional review action that adversely affects clinical privileges for **more than 30 days**; and
- acceptance of the surrender or restriction of clinical privileges while the physician or dentist is under investigation for possible incompetence or improper professional conduct, or in return for not conducting such an investigation or proceeding.

The NPDB’s operational explanation is available in the [NPDB Guidebook — Reporting Adverse Clinical Privileges Actions](https://npdb.hrsa.gov/guidebook/EClinicalPrivileges.jsp).

The reporting deadline is generally **within 30 days of the reportable action** under [45 CFR § 60.5](https://www.law.cornell.edu/cfr/text/45/60.5).

### 7.3 Other NPDB report categories

The NPDB receives additional categories of reports, including medical-malpractice payments, licensure and certification actions, negative findings by certain accreditation and peer-review bodies, health-care-related criminal convictions and civil judgments, federal/state program exclusions, and certain other adjudicated actions or decisions. See [NPDB — What You Must Report](https://www.npdb.hrsa.gov/hcorg/whatYouMustReportToTheDataBank.jsp) and [45 CFR Part 60](https://www.law.cornell.edu/cfr/text/45/part-60).

### 7.4 How the hospital reporting obligation is enforced

The reporting rule has a specific statutory enforcement mechanism rather than a generic “credentialing fine.”

If HHS has reason to believe a health care entity has **substantially failed** to make required reports, the Secretary investigates. The entity receives notice of the alleged noncompliance, an opportunity to correct it, and an opportunity for a hearing. If substantial noncompliance is ultimately found, the entity’s name is published in the Federal Register. See [42 U.S.C. § 11111(b)](https://www.law.cornell.edu/uscode/text/42/11111), [42 U.S.C. § 11133(c)](https://www.law.cornell.edu/uscode/text/42/11133), and [45 CFR § 60.12(c)](https://www.law.cornell.edu/cfr/text/45/60.12).

The consequence is significant: the entity loses the HCQIA limitation-on-damages protections in [42 U.S.C. § 11111(a)(1)](https://www.law.cornell.edu/uscode/text/42/11111) for qualifying professional-review actions commenced during the statutory three-year period, beginning 30 days after publication.

Other NPDB reporting regimes have different sanctions. The NPDB summarizes them in [What You Must Report — Sanctions for Failing to Report](https://www.npdb.hrsa.gov/hcorg/whatYouMustReportToTheDataBank.jsp).

### 7.5 NPDB is mandatory evidence, not the final credentialing decision

A hospital’s legal duty to query the NPDB does not mean that the NPDB makes the privileging decision. The hospital remains responsible for evaluating the information under its bylaws, applicable law, accreditation requirements, due-process obligations, and its clinical-privileging criteria.

---

## 8. Medicare Advantage Credentialing

Medicare Advantage (MA) has a distinct federal credentialing rule.

[42 CFR § 422.204 — Provider selection and credentialing](https://www.law.cornell.edu/cfr/text/42/422.204) requires an MA organization to maintain written provider-selection and evaluation policies and a documented credentialing process.

For physicians and other health professionals, initial credentialing must include:

- a written application;
- **verification of licensure or certification from primary sources**;
- disciplinary status;
- eligibility for Medicare payment;
- site visits as appropriate; and
- an applicant attestation concerning correctness and completeness.

Recredentialing must occur at least every **three years** and must update initial credentialing information and consider specified performance information.

This is important because the obligation to use primary-source verification for licensure or certification is embedded directly in the federal MA regulation, not merely in an NCQA manual.

### 8.1 MA accreditation and deeming

[42 CFR § 422.156](https://www.law.cornell.edu/cfr/text/42/422.156) establishes a separate Medicare Advantage accreditation/deeming mechanism. An MA organization may be deemed to meet specified Medicare requirements when it is fully accredited in the applicable area by a private national accreditation organization approved by CMS using CMS-approved standards. “Provider participation rules” are among the areas identified as deemable.

Accordingly, an accreditation organization can become operationally important because CMS has incorporated accredited compliance into the MA regulatory structure. This is conceptually parallel to, but legally distinct from, hospital deemed status.

---

## 9. Medicaid Managed Care Credentialing

Medicaid managed care deliberately preserves more state control.

[42 CFR § 438.214 — Provider selection](https://www.law.cornell.edu/cfr/text/42/438.214) requires each state to establish a **uniform credentialing and recredentialing policy** for relevant Medicaid managed-care providers. MCOs, PIHPs, and PAHPs must follow the state policy and maintain a documented credentialing and recredentialing process. They must also satisfy additional state requirements.

The federal rule therefore creates a national structural requirement but delegates substantial substantive detail to the states.

CMS expressly explained when adopting the rule that it declined to require every state to follow NCQA credentialing standards, reasoning that states should retain flexibility to establish their uniform policies. See the discussion accompanying the Medicaid managed-care final rule, including the CMS response reproduced in the [2002 final rule materials](https://www.cms.gov/regulations-and-guidance/regulations-and-policies/quarterlyproviderupdates/downloads/cms2104f.pdf).

Therefore, for Medicaid the practical stack frequently looks like:

```text
42 CFR § 438.214
        ↓
State Medicaid agency uniform credentialing policy
        ↓
Managed-care contract requirements
        ↓
Optional / contractually required accreditation standards (state-specific)
        ↓
MCO credentialing policy and delegated arrangements
        ↓
Verification sources / CVO
        ↓
Network credentialing decision
```

A state may choose to incorporate NCQA accreditation, NCQA-like standards, or another credentialing framework into its contracts, but that must be examined state by state.

---

## 10. Commercial and Other Non-MA Health Plans

For commercial insurers and other non-MA payers, there is no single federal credentialing rule equivalent to [42 CFR § 422.204](https://www.law.cornell.edu/cfr/text/42/422.204) that universally governs every plan.

The governing requirements can instead come from combinations of:

- state insurance and managed-care statutes and regulations;
- state-mandated credentialing application rules;
- network adequacy and provider-directory rules;
- contractual requirements imposed by purchasers or government programs;
- accreditation requirements;
- delegated credentialing contracts; and
- the plan’s own credentialing policies.

This is one of the reasons NCQA has such broad practical influence without being the legislature or licensing authority: a plan may need or choose NCQA accreditation because of state requirements, customer requirements, market expectations, delegation arrangements, or internal policy. Once the organization undertakes an NCQA accreditation or certification regime, the applicable NCQA standards become requirements for maintaining that accreditation or certification.

---

## 11. NCQA: How Its Requirements “Force” a Particular Approach

The [National Committee for Quality Assurance (NCQA)](https://www.ncqa.org/) performs several distinct roles relevant to credentialing.

### 11.1 Health Plan Accreditation

NCQA’s [Health Plan Accreditation](https://www.ncqa.org/programs/health-plans/health-plan-accreditation-hpa/) includes credentialing and recredentialing among its assessed domains. Its public [Health Plan Accreditation requirements overview](https://www.ncqa.org/programs/health-plans/health-plan-accreditation-hpa/process/requirements/) identifies credentialing and recredentialing as a core requirement area. Detailed NCQA standards are maintained in NCQA’s standards publications and are not all reproduced publicly.

NCQA standards do not independently become “law” merely because NCQA publishes them. They become binding on a particular organization through one or more mechanisms:

1. **Voluntary accreditation:** the organization chooses to seek and maintain NCQA accreditation.
2. **Government incorporation or recognition:** a statute, regulation, state Medicaid agency, or government contract can require, recognize, or deem compliance based on NCQA accreditation.
3. **Commercial contract:** a payer, provider organization, delegated entity, employer, or customer may contractually require NCQA accreditation/certification or compliance with NCQA standards.
4. **Delegated credentialing:** a plan may require a delegate or CVO to satisfy NCQA requirements because the plan remains accountable under its own accreditation and contracts.

Thus NCQA often acts as a **standards multiplier**: the standards become practically mandatory because another actor has made NCQA status or NCQA-conforming performance a condition of doing business or satisfying oversight.

### 11.2 Credentialing Accreditation vs. CVO Certification

NCQA distinguishes full-scope credentialing from credentials verification.

Its [Credentialing Accreditation standards overview](https://www.ncqa.org/programs/health-plans/credentialing/benefits-support/standards/) describes full-scope services as including:

- verification of practitioner credentials through a **primary source, recognized source, or contracted agent of the primary source**;
- a credentialing committee that reviews credentials and makes credentialing recommendations; and
- ongoing monitoring of sanctions, complaints, and quality issues.

Its [Credentials Verification Organization (CVO) Certification standards overview](https://www.ncqa.org/programs/health-plans/credentials-verification-organization-cvo/benefits-support/standards/) addresses organizations that perform the verification function for clients.

The distinction is important:

> **CVO verification can be an input to credentialing; the CVO does not necessarily make the client health plan’s final network-participation decision.**

---

## 12. DataSpring (formerly CAQH)

In June 2026, CAQH announced that it had rebranded as **DataSpring, powered by CAQH**. See [DataSpring — CAQH Rebrands as DataSpring](https://www.dataspring.com/blog/caqh-rebrands-as-dataspring-to-power-the-next-era-of-healthcare-data).

The corporate/legal organization continues to identify itself as the Council for Affordable Quality Healthcare, Inc. doing business as DataSpring; its services include **Credentialing (formerly ProView)**. See the [DataSpring Privacy Policy](https://www.dataspring.com/about/privacy-policy).

### 12.1 Provider-supplied credentialing data

The [DataSpring Provider Data Portal](https://www.dataspring.com/solutions/provider-data/credentialing-suite) allows clinicians to maintain professional and practice information and authorize health plans and other organizations to receive it. DataSpring states that its single credentialing application is accepted or supported across all 50 states.

This is principally a **standardized collection, attestation, exchange, and workflow function**. The existence of information in the Provider Data Portal should not by itself be conflated with independent primary-source verification of every field.

### 12.2 Primary-source verification services

DataSpring separately offers a **Primary Source Verification** service that it describes as validating credentialing information against licensing boards, medical schools, government registries, and other authoritative sources. See [DataSpring Credentialing Suite — Primary Source Verification](https://www.dataspring.com/solutions/provider-data/credentialing-suite).

This distinction is important:

```text
Provider assertion / attestation in DataSpring
                    ≠
Primary-source verified credential merely by virtue of being present
```

A DataSpring service may separately perform PSV and create verification evidence.

### 12.3 State adoption and regulatory entrenchment of the CAQH application

CAQH's competitive position did not arise only from voluntary payer adoption. During its nonprofit era, CAQH actively standardized the provider credentialing application and adapted the platform to state-specific requirements. Over time, a number of states incorporated the CAQH application or CAQH-supported electronic workflow into statute, regulation, insurance-department policy, or statewide administrative-simplification programs. This gave the CAQH data model and application format a form of **regulatory entrenchment**: even where CAQH itself was not the credentialing decision-maker or primary-source verifier, providers and payers could be legally required to use, accept, or support the CAQH application or a state-selected database built around it.

CAQH's own historical materials describe the scale of that adoption. A 2012 CAQH fact sheet stated that **Indiana, Kansas, Kentucky, Louisiana, Maryland, Missouri, New Jersey, New Mexico, Ohio, Rhode Island, Tennessee, Vermont, and the District of Columbia** had adopted the CAQH Standard Provider Credentialing Application as a mandated or designated form. A 2023 CAQH map reported that **12 states and the District of Columbia had adopted the CAQH provider credentialing application**, another 25 states had voluntarily deployed it, and the CAQH system supported 13 unique state forms. See [CAQH — Provider Credentialing Application Accepted Nationwide (2023 map)](https://www.caqh.org/sites/default/files/2023-03/CAQH%20Credentialing%20Map_2023.pdf) and [CAQH — historical Universal Provider Datasource fact sheet](https://www.caqh.org/sites/default/files/oldsitefiles/pdf/UCDFactSheet.pdf).

Representative state examples show that the legal mechanisms differ:

| State / jurisdiction | How CAQH is embedded |
|---|---|
| **Vermont** | [18 V.S.A. § 9408a](https://legislature.vermont.gov/statutes/section/18/221/09408a) directs the state to prescribe the CAQH credentialing application, or a similar nationally recognized form prescribed by the Commissioner, and requires insurers and hospitals that perform credentialing to use the prescribed form. This is a direct statutory standardization of the application layer. |
| **Tennessee** | [Tenn. Code § 56-7-1009](https://law.justia.com/codes/tennessee/title-56/chapter-7/part-10/section-56-7-1009/) requires health insurance entities that credential or recredential network providers to **accept the CAQH application** in addition to their own applications. The statute expressly does not require the payer to become a CAQH participant or pay CAQH a fee. This is an acceptance mandate rather than an exclusive-platform mandate. |
| **Washington** | [RCW 48.43.750](https://apps.leg.wa.gov/rcw/default.aspx?cite=48.43.750) requires health carriers to use the credentialing database selected under state law and prohibits them from requiring a different submission format; [RCW 48.43.755](https://apps.leg.wa.gov/rcw/default.aspx?cite=48.43.755) correspondingly requires providers to submit through that selected database. Washington's administrative-simplification program selected CAQH as that database beginning in 2024. This is a statewide infrastructure mandate rather than merely a form-acceptance rule. |
| **Maryland** | Maryland historically designated the CAQH application as its uniform credentialing form. After CAQH changed corporate structure, the Maryland Insurance Administration issued [Bulletin 26-20 (July 24, 2026)](https://insurance.maryland.gov/Pages/Bulletins/Bulletin-26-20.aspx), provisionally designating **DataSpring, formerly CAQH**, as the uniform online credentialing application and multi-carrier common online provider-directory information system while the state adjusted its statute to the new corporate structure. This illustrates how deeply the CAQH workflow had become embedded: the state had to address continuity when CAQH ceased being a nonprofit alliance. |

The key policy point is that these state laws generally **standardize the application and data-exchange layer; they do not necessarily make every provider-supplied CAQH field a primary-source-verified credential or require the payer to accept the provider into its network**. The legal advantage is nevertheless substantial: once a common application schema and portal are referenced in law, regulation, or statewide administrative infrastructure, competing credentialing systems must often interoperate with that installed standard rather than simply replace it.

DataSpring's current credentialing materials describe the continuing effect of this history: its single credentialing application is accepted or supported in all 50 states, and its platform is maintained to accommodate state-specific credentialing requirements. See [DataSpring — Credentialing Suite](https://www.dataspring.com/solutions/provider-data/credentialing-suite) and [DataSpring — Resources](https://www.dataspring.com/resources).

### 12.4 Role of the CAQH ID

The CAQH Provider ID remains a widely used identifier within credentialing workflows. DataSpring support materials continue to reference the CAQH Provider ID, and third-party credentialing systems use it to retrieve or associate clinician credentialing data. The persistence of the CAQH ID is another consequence of the installed CAQH/DataSpring ecosystem: newer credentialing platforms can use the identifier as a key for importing, reconciling, maintaining, or routing provider credentialing information rather than requiring a wholly new provider identity and application record.

---

## 13. CertifyOS and SharedCred / National Shared Credentialing Program

[CertifyOS](https://www.certifyos.com/) is a commercial provider-data and credentialing technology company that offers credentialing, monitoring, licensing, enrollment, roster, and provider-data-management services.

Its [credentialing product](https://www.certifyos.com/products/credentialing) states that CertifyOS operates an NCQA-certified CVO and performs automated primary-source verification and continuous monitoring. CertifyOS also integrates with CAQH/DataSpring information; its public API documentation includes retrieval of practitioner data using a CAQH Provider ID.

### 13.1 SharedCred / National Shared Credentialing Program

In September 2026 CertifyOS announced **SharedCred**, described by the company as a National Shared Credentialing Program. Initial participating health plans announced by CertifyOS were UnitedHealthcare, Cigna Healthcare, and Centene.

See:

- [CertifyOS — Why We Built SharedCred](https://www.certifyos.com/blogs/why-we-built-sharedcred)
- [CertifyOS / PR Newswire — National Shared Credentialing Program announcement, September 2026](https://www.prnewswire.com/news-releases/certifyos-launches-the-first-national-shared-credentialing-program-with-commitments-from-unitedhealthcare-cigna-healthcare-and-centene-302887322.html)

The announcement states that participating plans share recredentialing rosters with CertifyOS; CertifyOS administers credentialing and performs PSV described as meeting NCQA and Medicaid standards across licensure states. It also states that providers use the portal to enter their **CAQH ID and required information once**.

The operational distinction from CAQH/DataSpring is important. **DataSpring is principally the established provider-data collection and exchange layer; CertifyOS positions itself as an automation and orchestration layer that consumes CAQH data, performs or coordinates verification, and pushes standardized provider information and credentialing artifacts into payer and delegated-entity workflows.** CertifyOS describes the legacy problem as a provider's CAQH profile being manually re-keyed into many payer systems. Its credentialing product states that its CAQH integration standardizes application information and **auto-rosters** provider data, while its integration documentation says CertifyOS integrates with CAQH to automate rostering and can return continuing data updates. See [CertifyOS — Credentialing](https://www.certifyos.com/products/credentialing) and [CertifyOS — CAQH/NPDB integration](https://knowledgebase.certifyos.com/does-certify-integrate-with-caqh-and/or-npdb).

CertifyOS has described its relationship with CAQH as complementary rather than substitutive: CAQH/DataSpring supplies a large-scale standardized provider-data foundation, while CertifyOS retrieves provider profiles through integration/API mechanisms, auto-rosters providers into relevant payer or delegated-group workflows, monitors changes, and can send updates to downstream systems. See [CertifyOS — CAQH & CertifyOS Together](https://www.certifyos.com/blogs/caqh-certifyos-modern-pdm).

SharedCred extends that automation concept beyond a single payer. CertifyOS describes SharedCred as producing **one governed, source-verified credentialing evidence packet** to a verification standard agreed in advance by participating plans, coordinating recredentialing clocks and provider outreach, and then making that common packet available to each plan. Each plan retains its own standards, committee process, restricted-source handling, and final network decision. See [CertifyOS — SharedCred](https://www.certifyos.com/sharedcred). Thus, the most useful shorthand is:

```text
CAQH / DataSpring
  standardized provider-supplied profile + installed state/payer data standard
                         ↓
CertifyOS integration / automation
  retrieve + normalize + verify + monitor + roster / transmit into downstream workflows
                         ↓
SharedCred
  perform common verification once + create governed evidence packet for multiple participating plans
                         ↓
Each payer
  retains plan-specific checks, committee governance, and final credentialing/network decision
```

CertifyOS’s earlier public documentation likewise says that a credentialing event can be initiated with a small set of identifying data including a CAQH ID when applicable. See [CertifyOS Knowledge Base — What do I need to kick off a credentialing event?](https://knowledgebase.certifyos.com/what-do-i-need-to-kick-off-a-credentialing-event-with-certify).

### 13.2 Regulatory status should be kept distinct from commercial claims

SharedCred is an important market development, but its launch should not be interpreted as a new federal regulatory regime or as automatic nationwide legal substitution for every payer’s credentialing responsibilities. The extent to which a health plan may rely on SharedCred depends on applicable federal program requirements, state law, accreditation requirements, delegation rules, contractual arrangements, and the plan’s continuing governance responsibilities.

A useful real-world illustration comes from MVP Health Care’s 2026 implementation notice, which says CertifyOS will support credentialing/recredentialing operations while **MVP retains credentialing governance, standards, and final authority**. See [MVP Health Care — CertifyOS credentialing services](https://www.mvphealthcare.com/providers/communications/2026-q3-certifyos-will-support-mvp-credentialing-services-for-practitioners).

That is a useful example of the broader principle:

> **Outsourcing verification or workflow does not necessarily outsource legal or governance accountability for the credentialing decision.**

---

## 14. NAMSS and Professional Credentialing Practice

The [National Association Medical Staff Services (NAMSS)](https://www.namss.org/) is a professional organization for medical-services professionals and credentialing practitioners. It is not itself a government regulator or credential issuer.

Its **Ideal Credentialing Standards (ICS)** are useful because they organize credentialing around defined data elements and source types. The current NAMSS materials identify 13 essential criteria for initial credentialing and distinguish:

- **Primary Source Verification:** obtaining and verifying a credential directly from the original issuing entity.
- **Designated Equivalency Sources:** entities recognized under applicable regulatory/accreditation rules that verify credential information through the primary source.
- **Secondary Sources:** sources that are not the original issuer and generally have more limited acceptable use.

See [NAMSS — Ideal Credentialing Standards](https://www.namss.org/Advocacy/Ideal-Credentialing-Standards).

NAMSS expressly notes that acceptable designated-equivalency sources vary by accrediting organization and state regulation. This reinforces the broader model that source trust is contextual rather than universal.

---

## 15. Board Certification Is a Multi-Source Credential Domain

Board certification is not a single national credential issued or controlled by ABMS. The authoritative source for a particular board certification is the organization that actually issues and maintains that certification, while the **acceptability of that certification for hospital privileges, payer credentialing, or another purpose is determined separately by the applicable law, accreditation standard, contract, or organizational policy**.

This distinction is especially important because different certifying systems can cover overlapping specialties and can apply different approaches to initial certification, continuing certification, examinations, continuing medical education, and maintenance requirements. A credentialing system should therefore preserve both **the certifying body** and **the specific certification**, rather than normalizing all board certification to an ABMS indicator.

### 15.1 ABMS and its Member Boards

The [American Board of Medical Specialties (ABMS)](https://www.abms.org/) is an umbrella organization whose [24 Member Boards](https://www.abms.org/member-boards/) issue physician specialty and subspecialty certifications. For a certification issued by an ABMS Member Board, the issuing Member Board is the underlying certifying authority, and ABMS maintains an ecosystem for standards and certification data across those boards.

ABMS is therefore an authoritative or recognized source **for ABMS-system certifications**, but it is not the authoritative source for every form of physician board certification in the United States. Historical Joint Commission guidance illustrates this precision: its 2024 examples described ABMS as an equivalent source specifically for verification of certification **by an ABMS member board**, not for board certification generally. See [Joint Commission Online — March 6, 2024](https://www.jointcommission.org/en-us/knowledge-library/newsletters/joint-commission-online/06-mar-24).

### 15.2 AOA specialty board certification

The [American Osteopathic Association (AOA) Board Certification](https://certification.osteopathic.org/) system is a separate physician specialty-certification ecosystem. The AOA administers specialty and subspecialty certification through its osteopathic specialty certifying boards and an Osteopathic Continuous Certification framework. Its [specialties and subspecialties directory](https://certification.osteopathic.org/specialties-and-subspecialties/) identifies the certifications available through that system.

AOA certification should therefore be represented independently from ABMS certification. Historical Joint Commission guidance separately recognized the AOA Physician Database for specified osteopathic education, training, and osteopathic specialty-board-certification information.

### 15.3 American Board of Physician Specialties (ABPS)

The [American Board of Physician Specialties (ABPS)](https://www.abpsus.org/) is the certifying body of the American Association of Physician Specialists and operates a separate multi-specialty physician board-certification system. ABPS describes its Member Boards as offering certification in multiple specialties to qualified MD and DO physicians. See [ABPS — About](https://www.abpsus.org/about-us/) and [ABPS — Board Certifications](https://www.abpsus.org/board-certifications/).

ABPS certification is not an ABMS certification. Whether an ABPS certification satisfies a particular hospital, payer, state, employer, or other credentialing requirement depends on the rule or policy governing that decision. There is no single nationwide rule making every specialty-certification system interchangeable for every credentialing purpose.

### 15.4 National Board of Physicians and Surgeons (NBPAS)

The [National Board of Physicians and Surgeons (NBPAS)](https://nbpas.org/) offers a continuing-certification pathway that was created in response to concerns among some physicians about traditional maintenance/continuing-certification requirements. Its current [certification criteria](https://nbpas.org/pages/certification-criteria) require, among other things, prior certification through an ABMS or AOA member board in the applicable specialty, an active unrestricted medical license, and specified continuing medical education.

NBPAS therefore represents a particularly useful example of why the credentialing data model must distinguish **initial certifying history, current certification issuer, and the governing organization’s acceptance policy**. Joint Commission’s 2024 designated-equivalent-source examples specifically included NBPAS for verification of **NBPAS certification**. The inclusion did not mean that NBPAS and ABMS certifications were declared universally interchangeable; the same Joint Commission notice stated that listing a source was not an endorsement and that “equivalent” referred to the ability to provide information identical to the relevant primary source.

There is active disagreement among certification organizations about equivalence and continuing-certification models. For example, ABMS has publicly disputed claims that NBPAS certification is equivalent to continued ABMS certification. See [ABMS — Response to NBPAS assertion of certifying-body equivalency](https://www.abms.org/newsroom/the-abms-response-to-national-board-of-physicians-and-surgeons-assertion-of-certifying-body-equivalency/). For credentialing purposes, this disagreement should be recorded as a policy/recognition question rather than resolved by assuming one certification system is universally controlling.

### 15.5 Dental specialty certification

Dentistry has a distinct specialty-recognition and certification structure and should not be forced into the physician ABMS/AOA model. The [National Commission on Recognition of Dental Specialties and Certifying Boards](https://ncrdscb.ada.org/) recognizes dental specialties and national certifying boards. Its [recognized certifying boards](https://ncrdscb.ada.org/recognized-certifying-boards) page states that, following recognition of a dental specialty, a national certifying board for that specialty must separately obtain recognition and that the Commission recognizes no more than one certifying board for each recognized specialty.

The Commission's current recognized-board population includes boards in areas such as dental public health, endodontics, oral and maxillofacial pathology, oral and maxillofacial surgery, oral medicine, orofacial pain, orthodontics, pediatric dentistry, periodontology, prosthodontics, and dental anesthesiology. See the Commission's [2026 Annual Report of Recognized Dental Specialty Certifying Boards](https://ncrdscb.ada.org/-/media/project/ada-organization/ada/ncrdscb/files/2026_certifyingboards_annualreport.pdf).

Dental credentialing therefore reinforces the same general principle: **board certification is an attribute whose authoritative source depends on the profession, specialty, and issuing board; downstream acceptance depends on the credentialing regime.**

### 15.6 Practical source model for board certification

A board-certification record should conceptually retain at least:

```text
Profession
    ↓
Specialty / subspecialty
    ↓
Certifying organization / issuing board
    ↓
Certification identifier or title
    ↓
Initial certification date
    ↓
Current status / expiration or reverification information
    ↓
Continuing-certification pathway, if applicable
    ↓
Verification source and verification date
    ↓
Separate rule or policy determining whether that certification is accepted
```

This prevents an important category error: **verification that a certification exists is different from a determination that the certification satisfies a particular credentialing requirement.**

---

## 16. Working Taxonomy of Credentialing Roles

| Role | Function | Examples |
|---|---|---|
| **Regulator / program authority** | Creates legal participation or credentialing requirements | CMS; state departments of health; state insurance departments; state Medicaid agencies |
| **Credential issuer / primary source** | Creates or controls the underlying credential fact | State licensing board; specialty board; medical school; training program |
| **Federal mandatory repository** | Receives and discloses statutorily defined reports | NPDB |
| **Accreditor / standards setter** | Establishes operational standards; may acquire regulatory significance through deeming, contract, or incorporation | Joint Commission; NCQA |
| **Credentials Verification Organization (CVO)** | Performs verification on behalf of another organization | NCQA-certified CVOs; commercial credentialing organizations |
| **Provider-data exchange / application utility** | Collects, standardizes, attests, and distributes provider-supplied data | DataSpring / CAQH Provider Data Portal |
| **Credentialing workflow / infrastructure vendor** | Automates collection, PSV, monitoring, workflow, and delegated operations | CertifyOS; DataSpring credentialing services |
| **Professional practice / standards organization** | Develops best-practice guidance and professional standards | NAMSS |
| **Decision maker** | Makes the actual appointment, privileges, or network-participation decision | Hospital governing body; health-plan credentialing governance |

---

## 17. Glossary of Entities and Terms

### Entities

| Entity | Description |
|---|---|
| [Centers for Medicare & Medicaid Services (CMS)](https://www.cms.gov/) | Federal agency administering Medicare and overseeing major aspects of Medicaid. CMS establishes hospital Conditions of Participation, Medicare Advantage requirements, provider/supplier enrollment requirements, and accrediting-organization/deeming frameworks. |
| [The Joint Commission](https://www.jointcommission.org/) | National health-care accrediting organization. For certain provider types and programs, Joint Commission accreditation may support CMS deemed status. Its credentialing standards address primary-source verification, medical-staff credentialing, privileging, and use of CVOs. |
| [DNV Healthcare](https://www.dnv.com/healthcare/) | CMS-approved hospital accrediting organization whose NIAHO® model aligns with the CMS Conditions of Participation and integrates ISO 9001 quality-management principles. DNV uses annual surveys within a three-year accreditation cycle and emphasizes continuous systems improvement. |
| [Center for Improvement in Healthcare Quality (CIHQ)](https://cihq.org/acc-default-hospitals.asp) | CMS-approved hospital accrediting organization for Medicare deemed-status programs. CIHQ organizes its hospital accreditation closely around CMS Conditions of Participation and publishes hospital standards and survey guides for participating hospitals. |
| [Accreditation Commission for Health Care (ACHC)](https://achc.org/hospital/) | CMS-approved accrediting organization with an acute-care hospital program that incorporates the former HFAP hospital accreditation lineage. Its hospital credentialing materials address primary-source verification, NPDB querying, CVO use, and evidence supporting privileges. |
| [National Committee for Quality Assurance (NCQA)](https://www.ncqa.org/) | Private nonprofit standards and accreditation organization particularly influential in health-plan quality, credentialing, delegated credentialing, and CVO certification. Its standards can become practically mandatory through accreditation, government contracts, deeming/recognition, delegation, or commercial agreements. |
| [National Practitioner Data Bank (NPDB)](https://www.npdb.hrsa.gov/) | Federal repository administered by HRSA containing statutorily specified reports such as malpractice payments, adverse licensure actions, certain adverse clinical-privileges actions, exclusions, and other reportable actions. Hospitals have specific federal duties to query it and health-care entities have defined reporting duties. |
| [American Board of Medical Specialties (ABMS)](https://www.abms.org/) | Federation of member medical specialty boards. ABMS and its member boards are central to physician specialty-board certification. Joint Commission’s 2024 designated-equivalent-source examples included ABMS for verification of certification by an ABMS member board. |
| [Federation of State Medical Boards (FSMB)](https://www.fsmb.org/) | National organization representing U.S. state medical and osteopathic boards. It aggregates and distributes medical-licensure and disciplinary information and supports services used by boards and credentialing organizations. The underlying legal licensing authority remains with the applicable state board. |
| [AMA Physician Professional Data / AMA Physician Profile](https://www.ama-assn.org/practice-management/masterfile/ama-physician-professional-data) | American Medical Association physician information services derived from AMA physician professional data. Historically recognized by credentialing frameworks for specified education and postgraduate-training verification. Joint Commission’s 2024 examples referenced AMA Physician Professional Data for specified U.S. and Puerto Rican medical-school and postgraduate-education information. |
| [Educational Commission for Foreign Medical Graduates (ECFMG)](https://www.ecfmg.org/) | Organization responsible for certification-related functions concerning international medical graduates seeking entry into U.S. graduate medical education and related pathways. Historically used as a recognized verification source for specified foreign medical-education information. |
| [American Osteopathic Association (AOA)](https://osteopathic.org/) | National professional organization for osteopathic physicians. Its physician data and specialty-certification ecosystem can provide specified osteopathic education, training, and certification information. |
| [American Academy of Physician Associates (AAPA)](https://www.aapa.org/) | National professional organization representing physician associates/assistants. Historical Joint Commission materials referenced AAPA profile information, via AMA profile services, for specified PA education information. |
| [National Commission on Certification of Physician Assistants (NCCPA)](https://www.nccpa.net/) | National certifying organization for PAs. Certification information from NCCPA is a primary/recognized credential source for the certification it administers. |
| [National Board of Physicians and Surgeons (NBPAS)](https://nbpas.org/) | Physician continuing-certification organization offering an alternative pathway for physicians with prior ABMS/AOA certification. Its model emphasizes active licensure and CME rather than simply continuing the original ABMS/AOA certificate. Joint Commission’s 2024 examples included NBPAS specifically as a source for verification of NBPAS certification. |
| [DataSpring, powered by CAQH](https://www.dataspring.com/) | The 2026 brand of CAQH. Operates large-scale provider-data and administrative-data services. Its credentialing ecosystem includes the Provider Data Portal (formerly CAQH ProView), provider attestations/data exchange, primary-source verification services, and sanctions monitoring. |
| [CertifyOS](https://www.certifyos.com/) | Commercial provider-data infrastructure company providing credentialing, CVO, monitoring, licensing, enrollment, roster, and provider-data-management services. In September 2026 it announced SharedCred / the National Shared Credentialing Program with several national health plans as initial participants. |
| [National Association Medical Staff Services (NAMSS)](https://www.namss.org/) | Professional association for medical-services and credentialing professionals. Publishes Ideal Credentialing Standards and other practice guidance; it is not itself a regulator or issuer of clinicians’ credentials. |
| [Health Resources and Services Administration (HRSA)](https://www.hrsa.gov/) | HHS agency that administers the NPDB program. HRSA publishes the NPDB Guidebook and operational guidance implementing the statutory and regulatory NPDB framework. |

### Terms

| Term | Definition |
|---|---|
| **Credentialing** | The organizational process of collecting and evaluating information about a clinician’s qualifications and determining whether the clinician satisfies defined requirements. Depending on the setting, the process may result in a recommendation or decision about appointment, privileges, network participation, or another relationship. |
| **Privileging** | The process by which a health-care organization authorizes an individual practitioner to perform specific clinical services or procedures within the organization. Credentialing supplies evidence relevant to privileging, but the concepts are distinct. |
| **Primary source** | The original entity that issued, created, or controls the credential or authoritative fact, such as a state board for a license or a certifying board for its certification. |
| **Primary Source Verification (PSV)** | Verification of a reported qualification directly with the original source or through a verification path permitted by the applicable standard, such as an approved agent or qualifying CVO. The exact definition and permitted mechanisms depend on the governing regime. |
| **Designated equivalent source / equivalency source** | Historically, a source recognized as maintaining specified information equivalent to the primary source. The term is not a universal statutory category, and accepted sources can differ by accreditor, state, and credential element. Joint Commission’s current 2026 public guidance no longer maintains its former glossary list of examples. |
| **Recognized source** | NCQA terminology used in the credentialing/CVO context for a source accepted under NCQA standards as a permissible verification pathway for specified information. |
| **Credentials Verification Organization (CVO)** | An organization that performs credential verification on behalf of a credentialing organization. A CVO may contact primary sources or use permitted recognized/agent sources and return verification evidence; final credentialing authority may remain with the client. |
| **Deeming** | The regulatory mechanism under which a government program treats an entity accredited by an approved accreditation organization as meeting specified program requirements, subject to the scope of the approval and continuing government oversight. **Deemed status** is the resulting status of an entity whose accreditation is being accepted in that way. Hospital deeming and Medicare Advantage deeming arise under different provisions. |
| **Delegated credentialing** | An arrangement in which one organization delegates specified credentialing or verification functions to another entity. Delegation generally does not eliminate the delegating organization’s oversight/accountability obligations under applicable accreditation, regulatory, or contractual requirements. |
| **Recredentialing** | Periodic reevaluation of an already credentialed clinician. The required interval and elements depend on the applicable framework; for Medicare Advantage, federal regulation requires recredentialing at least every three years. |
| **Attestation** | A clinician’s representation that supplied information is accurate, complete, and/or current. Attestation is evidence of the clinician’s assertion but is not inherently equivalent to independent primary-source verification. |
| **Source provenance** | Information establishing where a credential fact came from, how it was obtained, when it was verified, which source was consulted, and what result was returned. Provenance is essential to determining whether downstream reliance satisfies a particular credentialing rule. |

---

## 18. Core Laws, Regulations, and Policy References

| Authority / policy | Why it matters |
|---|---|
| [42 CFR § 482.22 — Hospital medical staff](https://www.law.cornell.edu/cfr/text/42/482.22) | Establishes the Medicare Hospital Condition of Participation governing medical-staff organization, credential review, recommendations for appointment, medical-staff bylaws, and the granting of clinical privileges. |
| [42 U.S.C. § 1395bb — Effect of accreditation / Medicare deeming](https://www.law.cornell.edu/uscode/text/42/1395bb) | Provides the statutory basis for CMS to recognize qualifying accreditation as evidence that a provider or supplier meets applicable Medicare conditions, subject to federal oversight and validation. |
| [42 CFR Part 488 — Survey, certification, and enforcement procedures](https://www.law.cornell.edu/cfr/text/42/part-488) | Implements Medicare/Medicaid survey, certification, accrediting-organization approval, validation, deficiency, and enforcement processes for covered provider and supplier types. |
| [42 CFR § 488.5 — Accrediting-organization application/reapplication](https://www.law.cornell.edu/cfr/text/42/488.5) | Specifies what a national accrediting organization must submit to CMS to obtain or renew approval of an accreditation program used for Medicare deeming. |
| [42 U.S.C. § 11111 — HCQIA professional-review protections](https://www.law.cornell.edu/uscode/text/42/11111) | Establishes qualified immunity/limitations on damages for professional review actions meeting HCQIA standards and links loss of those protections to certain failures to satisfy NPDB reporting obligations. |
| [42 U.S.C. § 11133 — Reporting certain professional-review actions](https://www.law.cornell.edu/uscode/text/42/11133) | Requires health care entities to report specified adverse clinical-privilege actions and certain privilege surrenders/restrictions involving physicians and dentists. |
| [42 U.S.C. § 11135 — Hospital duty to obtain NPDB information](https://www.law.cornell.edu/uscode/text/42/11135) | Requires hospitals to query the NPDB when practitioners apply for medical-staff membership or clinical privileges and periodically thereafter, and defines consequences for failure to query. |
| [45 CFR Part 60 — NPDB regulations](https://www.law.cornell.edu/cfr/text/45/part-60) | Consolidates the federal regulations governing NPDB reporting, querying, disclosure, dispute, confidentiality, and related operational requirements. |
| [45 CFR § 60.5 — NPDB reporting deadlines](https://www.law.cornell.edu/cfr/text/45/60.5) | Establishes the general 30-day timeframe for submitting reportable information to the NPDB after the reportable action or event. |
| [45 CFR § 60.12 — Adverse clinical-privileges reporting](https://www.law.cornell.edu/cfr/text/45/60.12) | Implements the HCQIA duty to report specified professional-review actions and privilege surrenders/restrictions involving physicians and dentists and describes consequences of substantial reporting failures. |
| [45 CFR § 60.17 — Mandatory hospital NPDB queries](https://www.law.cornell.edu/cfr/text/45/60.17) | Implements hospitals’ mandatory NPDB query obligations for initial appointment/privileges and recurring review of practitioners who remain on staff or hold privileges. |
| [45 CFR § 60.18 — Who may request NPDB information](https://www.law.cornell.edu/cfr/text/45/60.18) | Defines which entities and persons may obtain NPDB information and the purposes for which they may query. |
| [42 CFR § 422.204 — Medicare Advantage provider selection and credentialing](https://www.law.cornell.edu/cfr/text/42/422.204) | Requires Medicare Advantage organizations to maintain provider-selection policies and a documented credentialing/recredentialing process, including primary-source verification of licensure or certification. |
| [42 CFR § 422.156 — Medicare Advantage accreditation deeming](https://www.law.cornell.edu/cfr/text/42/422.156) | Allows qualifying Medicare Advantage accreditation by a CMS-approved national accrediting organization to deem compliance with specified Medicare requirements. |
| [42 CFR § 438.214 — Medicaid managed-care provider selection and credentialing](https://www.law.cornell.edu/cfr/text/42/438.214) | Requires states to establish a uniform Medicaid managed-care credentialing/recredentialing policy and requires MCOs, PIHPs, and PAHPs to maintain documented processes consistent with that policy. |
| [CMS — Accrediting Organizations](https://www.cms.gov/medicare/health-safety-standards/quality-safety-oversight-general-information/accrediting-organizations-aos) | CMS policy page explaining approved accrediting organizations, Medicare deeming, and the federal oversight framework connecting private accreditation to Medicare certification. |
| [CMS — Strengthening Oversight of Accrediting Organizations (2026)](https://www.cms.gov/newsroom/fact-sheets/strengthening-cms-oversight-accrediting-organizations) | Summarizes CMS’s 2026 final-rule changes intended to strengthen AO oversight, reduce conflicts of interest, and align AO survey activity more closely with federal survey expectations. |
| [DNV — NIAHO® Accreditation for Acute Care Hospitals](https://www.dnv.com/services/niaho-accreditation-for-acute-care-hospitals/) | Describes DNV’s CMS-aligned hospital accreditation model, including its integration of ISO 9001 principles and annual survey approach. |
| [CIHQ — Hospital Accreditation](https://cihq.org/acc-default-hospitals.asp) | Describes CIHQ’s CMS-approved hospital accreditation program used for deeming and links its current hospital standards, accreditation policies, and survey activity guides. |
| [ACHC — Hospital Accreditation](https://achc.org/hospital/) | Describes ACHC’s hospital accreditation program, which incorporates the former HFAP hospital program and provides a CMS-approved accreditation pathway for Medicare deeming for acute-care hospitals. |
| [ACHC — Verifying Personnel Credentials](https://achc.org/verifying-hospital-credentials/) | Explains ACHC expectations for primary-source validation of hospital personnel licenses and illustrates how ACHC operationalizes credential verification in its hospital standards. |
| [Joint Commission — Primary Source Verification FAQ](https://www.jointcommission.org/en-us/knowledge-library/support-center/standards-interpretation/standards-faqs/000001472) | Current Joint Commission interpretation of primary-source verification, acceptable verification methods, CVO use, documentation requirements, and the organization’s current approach to equivalent sources. |
| [Joint Commission — 2024 designated-equivalent-source revision](https://www.jointcommission.org/en-us/knowledge-library/newsletters/joint-commission-online/06-mar-24) | Historical Joint Commission notice showing the former designated-equivalent-source examples and clarifying that listing a source was not an endorsement or declaration of equal rigor. |
| [NPDB Guidebook](https://www.npdb.hrsa.gov/guidebook/) | HRSA’s principal operational guidance explaining how NPDB reporting, querying, subjects, disputes, investigations, and specific report categories are administered. |
| [NAMSS — Ideal Credentialing Standards](https://www.namss.org/Advocacy/Ideal-Credentialing-Standards) | Professional-practice framework from NAMSS describing recommended credentialing data elements and distinctions among primary, equivalent, and secondary verification sources. |
| [ABMS — Member Boards](https://www.abms.org/member-boards/) | Identifies the physician specialty certifying boards that participate in the ABMS system; useful for distinguishing ABMS-system certification from other board-certification pathways. |
| [AOA — Board Certification](https://certification.osteopathic.org/) | Describes the separate AOA physician specialty-board-certification system and its specialty boards and continuing-certification framework. |
| [ABPS — Board Certification](https://www.abpsus.org/board-certifications/) | Describes the specialties and certification pathway offered by the American Board of Physician Specialties, a physician certifying system outside ABMS. |
| [NBPAS — Certification Criteria](https://nbpas.org/pages/certification-criteria) | Defines the eligibility and ongoing requirements for the NBPAS alternative continuing-certification pathway, including prior ABMS/AOA certification, licensure, and CME requirements. |
| [National Commission — Recognized Dental Specialty Certifying Boards](https://ncrdscb.ada.org/recognized-certifying-boards) | Identifies the dental specialty certifying boards recognized within the National Commission’s dental specialty-recognition framework. |

---

## 19. Research Notes / Boundaries for Future Expansion

This document deliberately begins with **individual-clinician credentialing**. Hospital/facility data sources such as the American Hospital Association are outside the present scope and can be addressed separately when organizational/facility credentialing is studied.

Areas intended for later expansion include:

- state-by-state credentialing laws and source requirements;
- professional category differences (physicians, PAs, APRNs, dentists, psychologists, etc.);
- delegated credentialing rules in greater detail;
- source-specific freshness / re-verification intervals;
- URAC and other payer accreditors;
- DEA / controlled-substance registration verification;
- OIG LEIE, SAM.gov exclusions, and Medicare preclusion/payment-eligibility sources;
- malpractice coverage and claims-history verification;
- education and training source hierarchies;
- ongoing monitoring between credentialing cycles; and
- precise mapping of credential attributes to primary, recognized, equivalent, and secondary sources.

