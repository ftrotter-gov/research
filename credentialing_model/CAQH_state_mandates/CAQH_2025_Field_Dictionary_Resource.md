# CAQH Standard Provider Application v6.0 (Implemented 04/2025) — Data Field Dictionary

**Source:** District of Columbia Department of Insurance, Securities and Banking copy of the CAQH Standard Provider Application, v6.0, implemented 04/2025:  
https://disb.dc.gov/sites/default/files/dc/sites/disb/page_content/attachments/CAQH%20Standard%20Application%20Sample.pdf

## Scope and conventions

This resource inventories the data fields captured by the application and its supplemental forms. Code-list pages are reference data and are not included as provider-entered fields.

- **Data Section:** The section or subsection label associated with the field on the form.
- **Data Field Name:** The name of the captured field.
- **Data Field Description:** A concise description of the information captured by the field.
- **Data Type:** Recommended database column type for the field.
- **Repeatable:** `Yes` when the field belongs to a record or block for which the form permits more than one instance; otherwise `No`.

| Data Section | Data Field Name | Data Field Description | Data Type | Repeatable |
|---|---|---|---|---|
| Provider Type | Provider Type Code | Three-digit code identifying the provider's professional type from the CAQH provider type code list. | CHAR(3) | No |
| Name | Last Name | Provider's legal last name. | VARCHAR(80) | No |
| Name | Suffix | Generational or professional suffix such as Jr. or III. | VARCHAR(20) | No |
| Name | First Name | Provider's legal first name. | VARCHAR(80) | No |
| Name | Middle Name | Provider's legal middle name. | VARCHAR(80) | No |
| Name | Ever Used Another Name | Indicates whether the provider has used another name. | BOOLEAN | No |
| Name | Other Last Name | Prior/alternate last name. | VARCHAR(80) | Yes |
| Name | Other Name Suffix | Suffix associated with an alternate name. | VARCHAR(20) | Yes |
| Name | Other First Name | Prior/alternate first name. | VARCHAR(80) | Yes |
| Name | Other Middle Name | Prior/alternate middle name. | VARCHAR(80) | Yes |
| Name | Other Name Start Date | Date provider began using the alternate name. | DATE | Yes |
| Name | Other Name End Date | Date provider stopped using the alternate name. | DATE | Yes |
| General Information | Gender | Sex/gender selection printed on the form (Male/Female). | VARCHAR(20) | No |
| General Information | Social Security Number | U.S. Social Security Number; form instructs foreign nationals without an SSN to use FNIN instead. | CHAR(9) | No |
| General Information | Foreign National Identification Number | Foreign national identification number when no SSN is available. | VARCHAR(50) | No |
| General Information | FNIN Country of Issue | Country that issued the foreign national identification number. | CHAR(3) | No |
| General Information | Date of Birth | Provider's date of birth. | DATE | No |
| General Information | City of Birth | Provider's city of birth. | VARCHAR(100) | No |
| General Information | State of Birth | State/province of birth when applicable. | VARCHAR(50) | No |
| General Information | Country of Birth | Country of birth. | CHAR(3) | No |
| General Information | Non-English Language Code | Code for a non-English language spoken by the provider. | CHAR(3) | Yes |
| General Information | Practices Exclusively in Inpatient Setting | Indicates whether the provider practices exclusively in an inpatient setting. | BOOLEAN | No |
| Home Address | Street Number | House/building number for home address. | VARCHAR(20) | No |
| Home Address | Street | Street name for home address. | VARCHAR(120) | No |
| Home Address | Apartment Number | Apartment/unit identifier. | VARCHAR(30) | No |
| Home Address | City | Home-address city. | VARCHAR(100) | No |
| Home Address | State | Home-address state. | CHAR(2) | No |
| Home Address | ZIP Code | Home-address ZIP/postal code. | VARCHAR(10) | No |
| Home Address | Telephone | Home telephone number. | VARCHAR(25) | No |
| Home Address | Fax | Home fax number. | VARCHAR(25) | No |
| Home Address | Email | Provider contact email address. | VARCHAR(254) | No |
| Home Address | Preferred Method of Contact | Preferred follow-up channel, printed as Email or Fax. | VARCHAR(20) | No |
| Professional IDs | Federal DEA Number | Federal Drug Enforcement Administration registration number. | VARCHAR(20) | Yes |
| Professional IDs | DEA State of Registration | State associated with DEA registration. | CHAR(2) | Yes |
| Professional IDs | DEA Issue Date | DEA registration issue date. | DATE | Yes |
| Professional IDs | DEA Expiration Date | DEA registration expiration date. | DATE | Yes |
| Professional IDs | CDS Certificate Number | State controlled-dangerous-substance certificate/registration number. | VARCHAR(50) | Yes |
| Professional IDs | CDS State of Registration | State associated with CDS registration. | CHAR(2) | Yes |
| Professional IDs | CDS Issue Date | CDS registration issue date. | DATE | Yes |
| Professional IDs | CDS Expiration Date | CDS registration expiration date. | DATE | Yes |
| Professional IDs | License Type | Type of professional license/certification/registration; coded from provider type list on the form. | CHAR(3) | Yes |
| Professional IDs | State License Number | Professional license/certification/registration identifier. | VARCHAR(50) | Yes |
| Professional IDs | License Issuing State | State issuing the professional license. | CHAR(2) | Yes |
| Professional IDs | License Issue Date | License issue date. | DATE | Yes |
| Professional IDs | License Expiration Date | License expiration date. | DATE | Yes |
| Professional IDs | License Status Code | Three-digit CAQH license-status code. | CHAR(3) | Yes |
| Professional IDs | Currently Practicing in License State | Indicates whether provider currently practices in the state of the listed license. | BOOLEAN | Yes |
| Other ID Numbers | Participating Medicare Provider | Indicates whether provider is a participating Medicare provider. | BOOLEAN | No |
| Other ID Numbers | Medicare Number | Medicare provider identifier used by the form. | VARCHAR(50) | No |
| Other ID Numbers | Participating Medicaid Provider | Indicates whether provider is a participating Medicaid provider. | BOOLEAN | No |
| Other ID Numbers | Medicaid Number | Medicaid provider number. | VARCHAR(50) | No |
| Other ID Numbers | Medicaid State | State associated with Medicaid number. | CHAR(2) | No |
| Other ID Numbers | UPIN | Unique Physician Identification Number, if applicable. | VARCHAR(20) | No |
| Other ID Numbers | National Provider Identifier (NPI) | Ten-digit National Provider Identifier. | CHAR(10) | No |
| Other ID Numbers | Workers Compensation Number | Workers' compensation identifier. | VARCHAR(50) | No |
| Other ID Numbers | USMLE Number | United States Medical Licensing Examination number, entered without hyphens. | VARCHAR(30) | No |
| Other ID Numbers | ECFMG Number | ECFMG certificate/identifier for non-U.S./Canadian graduates. | VARCHAR(30) | No |
| Other ID Numbers | ECFMG Certificate Issue Date | Date the ECFMG certificate was issued. | DATE | No |
| Undergraduate School(s) | Official Name of Undergraduate School | Name of undergraduate institution. | VARCHAR(160) | Yes |
| Undergraduate School(s) | School Address | Street address of undergraduate institution. | VARCHAR(160) | Yes |
| Undergraduate School(s) | School City | City of undergraduate institution. | VARCHAR(100) | Yes |
| Undergraduate School(s) | School State | State of undergraduate institution. | VARCHAR(50) | Yes |
| Undergraduate School(s) | School ZIP/Postal Code | ZIP/postal code of undergraduate institution. | VARCHAR(20) | Yes |
| Undergraduate School(s) | School Country Code | Country code of undergraduate institution. | CHAR(3) | Yes |
| Undergraduate School(s) | School Telephone | Institution telephone number. | VARCHAR(25) | Yes |
| Undergraduate School(s) | School Fax | Institution fax number. | VARCHAR(25) | Yes |
| Undergraduate School(s) | Start Date | Month/year attendance began. | CHAR(7) | Yes |
| Undergraduate School(s) | End/Graduation Date | Month/year attendance ended or degree was awarded. | CHAR(7) | Yes |
| Undergraduate School(s) | Degree Awarded | Undergraduate degree awarded. | VARCHAR(100) | Yes |
| Undergraduate School(s) | Completed Undergraduate Education at School | Indicates whether undergraduate education was completed at that institution. | BOOLEAN | Yes |
| Professional School(s) | Graduate Type | U.S./Canadian graduate, non-U.S./Canadian graduate, or Fifth Pathway graduate. | VARCHAR(40) | Yes |
| Professional School(s) | U.S./Canadian School Code | CAQH school code for U.S./Canadian professional school. | CHAR(3) | Yes |
| Professional School(s) | Name of U.S./Canadian School | Name of U.S./Canadian professional school. | VARCHAR(160) | Yes |
| Professional School(s) | Official Name of Non-U.S. Professional School | Official name of non-U.S./Canadian professional school. | VARCHAR(160) | Yes |
| Professional School(s) | School Address | Professional school address. | VARCHAR(160) | Yes |
| Professional School(s) | School City | Professional school city. | VARCHAR(100) | Yes |
| Professional School(s) | School State | Professional school state/province where applicable. | VARCHAR(50) | Yes |
| Professional School(s) | School ZIP/Postal Code | Professional school ZIP/postal code. | VARCHAR(20) | Yes |
| Professional School(s) | School Country Code | Professional school country code. | CHAR(3) | Yes |
| Professional School(s) | School Telephone | Professional school telephone. | VARCHAR(25) | Yes |
| Professional School(s) | School Fax | Professional school fax. | VARCHAR(25) | Yes |
| Professional School(s) | Start Date | Month/year professional education began. | CHAR(7) | Yes |
| Professional School(s) | End/Graduation Date | Month/year professional education ended/graduation occurred. | CHAR(7) | Yes |
| Professional School(s) | Degree Awarded | Professional degree awarded. | VARCHAR(100) | Yes |
| Professional School(s) | Completed Graduate Education at School | Indicates whether graduate/professional education was completed at the institution. | BOOLEAN | Yes |
| Training | Institution/Hospital Name | Name of postgraduate training institution or hospital. | VARCHAR(160) | Yes |
| Training | Institution Address Number | Street/building number. | VARCHAR(20) | Yes |
| Training | Institution Street | Street name. | VARCHAR(120) | Yes |
| Training | Institution Suite/Building | Suite/building designation. | VARCHAR(50) | Yes |
| Training | Institution City | City. | VARCHAR(100) | Yes |
| Training | Institution State | State/province. | VARCHAR(50) | Yes |
| Training | Institution ZIP/Postal Code | ZIP/postal code. | VARCHAR(20) | Yes |
| Training | Institution Country Code | Country code. | CHAR(3) | Yes |
| Training | Institution Telephone | Telephone number. | VARCHAR(25) | Yes |
| Training | Institution Fax | Fax number. | VARCHAR(25) | Yes |
| Training | School Code | Code for affiliated medical/professional school when applicable. | CHAR(3) | Yes |
| Training | Program Type | Internship/Residency, Fellowship, or Other. | VARCHAR(30) | Yes |
| Training | Department/Specialty | Department or specialty of training, not abbreviated. | VARCHAR(160) | Yes |
| Training | Program Start Date | Month/year training began. | CHAR(7) | Yes |
| Training | Program End Date | Month/year training ended. | CHAR(7) | Yes |
| Training | Director Name | Name of program/director associated with the listed training program. | VARCHAR(160) | Yes |
| Training | Completed Training Program at Institution | Indicates whether the program was completed at the listed institution. | BOOLEAN | Yes |
| Training | Training Noncompletion Explanation | Explanation when the listed training program was not completed. | TEXT | Yes |
| Primary Specialty | Specialty Code | Three-digit CAQH specialty code for provider's primary specialty. | CHAR(3) | No |
| Primary Specialty | Board Certified | Indicates whether provider is board certified in the specialty. | BOOLEAN | No |
| Primary Specialty | Certifying Board Code | CAQH code identifying the certifying board. | VARCHAR(10) | No |
| Primary Specialty | Initial Certification Date | Initial board-certification date. | DATE | No |
| Primary Specialty | Recertification Date | Most recent recertification date, if applicable. | DATE | No |
| Primary Specialty | Certification Expiration Date | Certification expiration date, if applicable. | DATE | No |
| Primary Specialty | Directory Listing Requested | Indicates whether provider wishes to be listed in a directory under the specialty. | BOOLEAN | No |
| Primary Specialty | HMO Directory Indicator | Indicates HMO directory applicability/selection shown with the specialty. | BOOLEAN | No |
| Primary Specialty | PPO Directory Indicator | Indicates PPO directory applicability/selection shown with the specialty. | BOOLEAN | No |
| Primary Specialty | POS Directory Indicator | Indicates POS directory applicability/selection shown with the specialty. | BOOLEAN | No |
| Primary Specialty | Non-Board-Certified Status | Status when not board certified: exam taken/results pending, intends to sit, or does not intend to take exam. | VARCHAR(50) | No |
| Primary Specialty | Pending Exam Certifying Board Code | Certifying board code for an exam already taken with results pending. | VARCHAR(10) | No |
| Primary Specialty | Intended Board Exam Date | Date provider intends to sit for a board exam. | DATE | No |
| Primary Specialty | No-Exam Explanation | Explanation when provider does not intend to take a certifying board exam. | TEXT | No |
| Secondary Specialty | Specialty Code | Three-digit CAQH specialty code for a secondary specialty. | CHAR(3) | Yes |
| Secondary Specialty | Board Certified | Indicates whether provider is board certified in the specialty. | BOOLEAN | Yes |
| Secondary Specialty | Certifying Board Code | CAQH certifying board code. | VARCHAR(10) | Yes |
| Secondary Specialty | Initial Certification Date | Initial certification date. | DATE | Yes |
| Secondary Specialty | Recertification Date | Recertification date, if applicable. | DATE | Yes |
| Secondary Specialty | Certification Expiration Date | Certification expiration date, if applicable. | DATE | Yes |
| Secondary Specialty | Directory Listing Requested | Indicates whether directory listing is requested for the specialty. | BOOLEAN | Yes |
| Secondary Specialty | HMO Directory Indicator | HMO directory applicability/selection. | BOOLEAN | Yes |
| Secondary Specialty | PPO Directory Indicator | PPO directory applicability/selection. | BOOLEAN | Yes |
| Secondary Specialty | POS Directory Indicator | POS directory applicability/selection. | BOOLEAN | Yes |
| Secondary Specialty | Non-Board-Certified Status | Exam status/intention when not board certified. | VARCHAR(50) | Yes |
| Secondary Specialty | Pending Exam Certifying Board Code | Board code when exam has been taken and results are pending. | VARCHAR(10) | Yes |
| Secondary Specialty | Intended Board Exam Date | Intended exam date. | DATE | Yes |
| Secondary Specialty | No-Exam Explanation | Explanation for not intending to take certifying board exam. | TEXT | Yes |
| Practice Interests | Practice Interest / Activity / Procedure / Diagnosis / Population | Free-text additional professional practice interests, activities, procedures, diagnoses, or populations. | TEXT | No |
| Certifications | Basic Life Support Held | Indicates current Basic Life Support certification. | BOOLEAN | No |
| Certifications | Basic Life Support Expiration Date | Expiration date of BLS certification. | DATE | No |
| Certifications | CPR Held | Indicates current CPR certification. | BOOLEAN | No |
| Certifications | CPR Expiration Date | CPR certification expiration date. | DATE | No |
| Certifications | Advanced Cardiac Life Support Held | Indicates ACLS certification. | BOOLEAN | No |
| Certifications | Advanced Cardiac Life Support Expiration Date | ACLS expiration date. | DATE | No |
| Certifications | Neonatal Advanced Life Support Held | Indicates neonatal advanced life-support certification. | BOOLEAN | No |
| Certifications | Neonatal Advanced Life Support Expiration Date | Neonatal advanced life-support expiration date. | DATE | No |
| Certifications | Advanced Life Support in Obstetrics Held | Indicates advanced life support in obstetrics certification. | BOOLEAN | No |
| Certifications | Advanced Life Support in Obstetrics Expiration Date | ALOS/ALSO certification expiration date. | DATE | No |
| Certifications | Advanced Trauma Life Support Held | Indicates ATLS certification. | BOOLEAN | No |
| Certifications | Advanced Trauma Life Support Expiration Date | ATLS expiration date. | DATE | No |
| Certifications | Pediatric Advanced Life Support Held | Indicates PALS certification. | BOOLEAN | No |
| Certifications | Pediatric Advanced Life Support Expiration Date | PALS expiration date. | DATE | No |
| Primary Credentialing Contact | Use Primary Practice Office Manager as Credentialing Contact | Indicates whether the primary-practice office manager/address should be reused for credentialing contact information. | BOOLEAN | No |
| Primary Credentialing Contact | Last Name | Credentialing contact last name. | VARCHAR(80) | No |
| Primary Credentialing Contact | First Name | Credentialing contact first name. | VARCHAR(80) | No |
| Primary Credentialing Contact | Middle Initial | Credentialing contact middle initial. | CHAR(1) | No |
| Primary Credentialing Contact | Street Number | Credentialing contact address number. | VARCHAR(20) | No |
| Primary Credentialing Contact | Street | Credentialing contact street. | VARCHAR(120) | No |
| Primary Credentialing Contact | Suite/Building | Credentialing contact suite/building. | VARCHAR(50) | No |
| Primary Credentialing Contact | City | Credentialing contact city. | VARCHAR(100) | No |
| Primary Credentialing Contact | State | Credentialing contact state. | CHAR(2) | No |
| Primary Credentialing Contact | ZIP Code | Credentialing contact ZIP code. | VARCHAR(10) | No |
| Primary Credentialing Contact | Email Address | Credentialing contact email. | VARCHAR(254) | No |
| Primary Credentialing Contact | Telephone | Credentialing contact telephone. | VARCHAR(25) | No |
| Primary Credentialing Contact | Fax | Credentialing contact fax. | VARCHAR(25) | No |
| Primary Practice Location | Practice Location Number | Logical location identifier; primary location is the main-form location and supplemental locations are numbered. | SMALLINT | No |
| Primary Practice Location | Street Number | Practice street number. | VARCHAR(20) | No |
| Primary Practice Location | Street | Practice street name. | VARCHAR(120) | No |
| Primary Practice Location | Suite/Building | Practice suite/building. | VARCHAR(50) | No |
| Primary Practice Location | City | Practice city. | VARCHAR(100) | No |
| Primary Practice Location | State | Practice state. | CHAR(2) | No |
| Primary Practice Location | ZIP Code | Practice ZIP code. | VARCHAR(10) | No |
| Primary Practice Location | Physician Group / Practice Name for Directory | Practice/group name to appear in directory. | VARCHAR(160) | No |
| Primary Practice Location | Group / Corporate Name on W-9 | Legal group/corporate name as shown on W-9 if different. | VARCHAR(160) | No |
| Primary Practice Location | Telephone | Public practice telephone. | VARCHAR(25) | No |
| Primary Practice Location | Fax | Practice fax. | VARCHAR(25) | No |
| Primary Practice Location | Office Email Address | General office email address. | VARCHAR(254) | No |
| Primary Practice Location | Send General Correspondence Here | Indicates whether general correspondence should be sent to this location. | BOOLEAN | No |
| Primary Practice Location | Currently Practicing at Address | Indicates whether provider currently practices at this location. | BOOLEAN | No |
| Primary Practice Location | Previous or Future Start Date | Start date when location is previous/future rather than current. | DATE | No |
| Primary Practice Location | Individual Tax ID | Provider's individual taxpayer identification number used by practice. | CHAR(9) | No |
| Primary Practice Location | Group Tax ID | Group taxpayer identification number. | CHAR(9) | No |
| Primary Practice Location | Primary Tax ID Selection | Indicates whether individual or group Tax ID is the primary Tax ID. | VARCHAR(20) | No |
| Office Manager or Business Office Staff Contact | Last Name | Office manager/business contact last name. | VARCHAR(80) | No |
| Office Manager or Business Office Staff Contact | First Name | Office manager/business contact first name. | VARCHAR(80) | No |
| Office Manager or Business Office Staff Contact | Middle Initial | Middle initial. | CHAR(1) | No |
| Office Manager or Business Office Staff Contact | Email Address | Contact email. | VARCHAR(254) | No |
| Office Manager or Business Office Staff Contact | Telephone | Contact telephone. | VARCHAR(25) | No |
| Office Manager or Business Office Staff Contact | Fax | Contact fax. | VARCHAR(25) | No |
| Billing Contact | Use Office Manager and Office Address as Billing Information | Indicates whether billing contact/address is inherited from office-manager information. | BOOLEAN | No |
| Billing Contact | Last Name | Billing contact last name. | VARCHAR(80) | No |
| Billing Contact | First Name | Billing contact first name. | VARCHAR(80) | No |
| Billing Contact | Middle Initial | Billing contact middle initial. | CHAR(1) | No |
| Billing Contact | Street Number | Billing address number. | VARCHAR(20) | No |
| Billing Contact | Street | Billing street. | VARCHAR(120) | No |
| Billing Contact | Suite/Building | Billing suite/building. | VARCHAR(50) | No |
| Billing Contact | City | Billing city. | VARCHAR(100) | No |
| Billing Contact | State | Billing state. | CHAR(2) | No |
| Billing Contact | ZIP Code | Billing ZIP code. | VARCHAR(10) | No |
| Billing Contact | Email Address | Billing contact email. | VARCHAR(254) | No |
| Billing Contact | Telephone | Billing contact telephone. | VARCHAR(25) | No |
| Billing Contact | Fax | Billing contact fax. | VARCHAR(25) | No |
| Payment and Remittance | Billing Department | Billing department name when hospital-based. | VARCHAR(120) | No |
| Payment and Remittance | Check Payable To | Name to which reimbursement checks should be payable. | VARCHAR(160) | No |
| Payment and Remittance | Electronic Billing Capabilities | Indicates whether the practice supports electronic billing. | BOOLEAN | No |
| Payment and Remittance | Use Office Manager and Office Address as Payee Information | Indicates whether office-manager information is reused for payee/remittance contact. | BOOLEAN | No |
| Payment and Remittance | Payee Contact Last Name | Payee contact last name. | VARCHAR(80) | No |
| Payment and Remittance | Payee Contact First Name | Payee contact first name. | VARCHAR(80) | No |
| Payment and Remittance | Payee Contact Middle Initial | Payee contact middle initial. | CHAR(1) | No |
| Payment and Remittance | Payee Street Number | Payee/remittance address number. | VARCHAR(20) | No |
| Payment and Remittance | Payee Street | Payee/remittance street. | VARCHAR(120) | No |
| Payment and Remittance | Payee Suite/Building | Payee/remittance suite/building. | VARCHAR(50) | No |
| Payment and Remittance | Payee City | Payee/remittance city. | VARCHAR(100) | No |
| Payment and Remittance | Payee State | Payee/remittance state. | CHAR(2) | No |
| Payment and Remittance | Payee ZIP Code | Payee/remittance ZIP. | VARCHAR(10) | No |
| Payment and Remittance | Payee Email Address | Payee contact email. | VARCHAR(254) | No |
| Payment and Remittance | Payee Telephone | Payee telephone. | VARCHAR(25) | No |
| Payment and Remittance | Payee Fax | Payee fax. | VARCHAR(25) | No |
| Office Hours | Monday Start Time | Monday office-hours start time. | TIME | No |
| Office Hours | Monday End Time | Monday office-hours end time. | TIME | No |
| Office Hours | Tuesday Start Time | Tuesday office-hours start time. | TIME | No |
| Office Hours | Tuesday End Time | Tuesday office-hours end time. | TIME | No |
| Office Hours | Wednesday Start Time | Wednesday office-hours start time. | TIME | No |
| Office Hours | Wednesday End Time | Wednesday office-hours end time. | TIME | No |
| Office Hours | Thursday Start Time | Thursday office-hours start time. | TIME | No |
| Office Hours | Thursday End Time | Thursday office-hours end time. | TIME | No |
| Office Hours | Friday Start Time | Friday office-hours start time. | TIME | No |
| Office Hours | Friday End Time | Friday office-hours end time. | TIME | No |
| Office Hours | Saturday Start Time | Saturday office-hours start time. | TIME | No |
| Office Hours | Saturday End Time | Saturday office-hours end time. | TIME | No |
| Office Hours | Sunday Start Time | Sunday office-hours start time. | TIME | No |
| Office Hours | Sunday End Time | Sunday office-hours end time. | TIME | No |
| Office Hours | 24/7 Phone Coverage | Indicates whether 24/7 phone coverage is available. | BOOLEAN | No |
| Office Hours | After-Hours Coverage Method | Answering service, voicemail instructing caller to answering service, or voicemail with other instructions. | VARCHAR(60) | No |
| Office Hours | After-Hours Back Office Telephone | Non-public back-office telephone used for after-hours contact. | VARCHAR(25) | No |
| Open Practice Status | Accept New Patients Into Practice | Indicates whether practice accepts new patients. | BOOLEAN | No |
| Open Practice Status | Accept Existing Patients With Change of Payor | Indicates whether existing patients are accepted after changing payer. | BOOLEAN | No |
| Open Practice Status | Accept New Patients With Physician Referral | Indicates whether referred new patients are accepted. | BOOLEAN | No |
| Open Practice Status | Accept New Medicare Patients | Indicates whether new Medicare patients are accepted. | BOOLEAN | No |
| Open Practice Status | Accept New Medicaid Patients | Indicates whether new Medicaid patients are accepted. | BOOLEAN | No |
| Open Practice Status | Accept All New Patients | Indicates whether all new patients are accepted. | BOOLEAN | No |
| Open Practice Status | Practice Status Varies by Plan Explanation | Explanation of payer/plan-specific variations in open/closed status. | TEXT | No |
| Open Practice Status | Practice Limitations Exist | Indicates whether the practice applies limitations. | BOOLEAN | No |
| Open Practice Status | Gender Limitation | Male only, female only, none, or other relevant selection. | VARCHAR(20) | No |
| Open Practice Status | Minimum Age | Minimum patient age accepted. | SMALLINT | No |
| Open Practice Status | Maximum Age | Maximum patient age accepted. | SMALLINT | No |
| Open Practice Status | Other Practice Limitations | Free-text description of other practice limitations. | TEXT | No |
| Mid-Level Practitioners | Mid-Level Practitioners Care for Patients | Indicates whether NPs, PAs, or other mid-level practitioners care for patients at the practice. | BOOLEAN | Yes |
| Mid-Level Practitioners | Practitioner Last Name | Mid-level practitioner's last name. | VARCHAR(80) | Yes |
| Mid-Level Practitioners | Practitioner First Name | Mid-level practitioner's first name. | VARCHAR(80) | Yes |
| Mid-Level Practitioners | Practitioner Middle Initial | Mid-level practitioner's middle initial. | CHAR(1) | Yes |
| Mid-Level Practitioners | Practitioner Type | Practitioner type such as PA, CNP, NP. | VARCHAR(30) | Yes |
| Mid-Level Practitioners | Practitioner License / Certificate Number | License or certification number. | VARCHAR(50) | Yes |
| Mid-Level Practitioners | Practitioner State | State associated with listed license/certificate. | CHAR(2) | Yes |
| Languages | Office Personnel Language Code | Non-English language spoken by office personnel. | CHAR(3) | Yes |
| Languages | Interpreted Language Code | Language for which interpretation is available. | CHAR(3) | Yes |
| Languages | Interpreters Available | Indicates whether interpreters are available. | BOOLEAN | No |
| Accessibilities | Office Meets ADA Accessibility Requirements | Indicates whether office meets ADA accessibility requirements. | BOOLEAN | No |
| Accessibilities | Handicapped Access — Building | Indicates accessible building. | BOOLEAN | No |
| Accessibilities | Handicapped Access — Parking | Indicates accessible parking. | BOOLEAN | No |
| Accessibilities | Handicapped Access — Restroom | Indicates accessible restroom. | BOOLEAN | No |
| Accessibilities | Other Handicapped Access | Free-text other accessibility accommodations. | TEXT | No |
| Accessibilities | Accessible by Public Transportation | Indicates whether site is accessible by public transportation. | BOOLEAN | No |
| Accessibilities | Bus Access | Indicates bus access. | BOOLEAN | No |
| Accessibilities | Subway Access | Indicates subway access. | BOOLEAN | No |
| Accessibilities | Regional Train Access | Indicates regional train access. | BOOLEAN | No |
| Accessibilities | Other Transportation Access | Free-text other transportation access. | TEXT | No |
| Accessibilities | Text Telephony (TTY) | Indicates TTY availability. | BOOLEAN | No |
| Accessibilities | American Sign Language | Indicates ASL service availability. | BOOLEAN | No |
| Accessibilities | Mental/Physical Impairment Services | Indicates services for mental/physical impairments. | BOOLEAN | No |
| Accessibilities | Other Disability Services | Free-text other disability services. | TEXT | No |
| Services | Radiology Services | Indicates radiology services at the location. | BOOLEAN | No |
| Services | X-Ray Certification Type | Certification type for radiology/x-ray services when applicable. | VARCHAR(100) | No |
| Services | Drawing Blood | Indicates blood-draw services. | BOOLEAN | No |
| Services | Laboratory Services | Indicates laboratory services. | BOOLEAN | No |
| Services | Laboratory Accrediting/Certifying Program | Program such as CLIA, COLA, MLE when laboratory services are provided. | VARCHAR(100) | No |
| Services | Allergy Injections | Indicates allergy injections are provided. | BOOLEAN | No |
| Services | Age-Appropriate Immunizations | Indicates age-appropriate immunizations are provided. | BOOLEAN | No |
| Services | Allergy Skin Testing | Indicates allergy skin testing. | BOOLEAN | No |
| Services | Flexible Sigmoidoscopy | Indicates flexible sigmoidoscopy is performed. | BOOLEAN | No |
| Services | Routine Office Gynecology | Indicates pelvic/Pap gynecology services. | BOOLEAN | No |
| Services | Tympanometry/Audiometry Screening | Indicates tympanometry/audiometry screening. | BOOLEAN | No |
| Services | Asthma Treatment | Indicates asthma treatment. | BOOLEAN | No |
| Services | Physical Therapy | Indicates physical therapy services. | BOOLEAN | No |
| Services | Osteopathic Manipulation | Indicates osteopathic manipulation services. | BOOLEAN | No |
| Services | IV Hydration/Treatment | Indicates IV hydration/treatment. | BOOLEAN | No |
| Services | Cardiac Stress Test | Indicates cardiac stress testing. | BOOLEAN | No |
| Services | Cardiac Stress Test Class/Category | Class/category of stress test used when provided. | VARCHAR(100) | No |
| Services | Cardiac Stress Test Administrator | Person/type of professional administering the stress test. | VARCHAR(120) | No |
| Services | Anesthesia Administered in Office | Indicates whether anesthesia is administered in the office. | BOOLEAN | No |
| Services | EKGs | Indicates EKG services. | BOOLEAN | No |
| Services | Pulmonary Function Testing | Indicates pulmonary function testing. | BOOLEAN | No |
| Services | Care of Minor Lacerations | Indicates treatment of minor lacerations. | BOOLEAN | No |
| Services | Additional Office Procedures | Other procedures, including surgical procedures, provided at location. | TEXT | No |
| Practice Type | Type of Practice | Solo practice, single-specialty group, or multi-specialty group. | VARCHAR(40) | No |
| Partners/Associates | Partner/Associate Last Name | Last name of partner/associate. | VARCHAR(80) | Yes |
| Partners/Associates | Partner/Associate First Name | First name. | VARCHAR(80) | Yes |
| Partners/Associates | Partner/Associate Middle Initial | Middle initial. | CHAR(1) | Yes |
| Partners/Associates | Provider Type Code | Provider type code for partner/associate. | CHAR(3) | Yes |
| Partners/Associates | Specialty Code | Specialty code for partner/associate. | CHAR(3) | Yes |
| Partners/Associates | Covering Colleague Indicator | Indicates whether partner/associate provides coverage at this location. | BOOLEAN | Yes |
| Covering Colleagues | Covering Colleague Last Name | Last name of non-partner covering colleague. | VARCHAR(80) | Yes |
| Covering Colleagues | Covering Colleague First Name | First name. | VARCHAR(80) | Yes |
| Covering Colleagues | Covering Colleague Middle Initial | Middle initial. | CHAR(1) | Yes |
| Covering Colleagues | Provider Type Code | Provider type code for covering colleague. | CHAR(3) | Yes |
| Covering Colleagues | Specialty Code | Specialty code for covering colleague. | CHAR(3) | Yes |
| Admitting Arrangements | Has Hospital Privileges | Indicates whether provider has hospital privileges. | BOOLEAN | No |
| Admitting Arrangements | Admitting Arrangement Type | Description of admitting arrangements when provider does not admit patients directly. | TEXT | No |
| Hospital Privileges | Hospital Role | Identifies primary versus other hospital affiliation. | VARCHAR(20) | Yes |
| Hospital Privileges | Hospital Name | Hospital name. | VARCHAR(160) | Yes |
| Hospital Privileges | Department Name | Affiliated department. | VARCHAR(120) | Yes |
| Hospital Privileges | Street Number | Hospital street number. | VARCHAR(20) | Yes |
| Hospital Privileges | Street | Hospital street. | VARCHAR(120) | Yes |
| Hospital Privileges | Suite/Building | Hospital suite/building. | VARCHAR(50) | Yes |
| Hospital Privileges | City | Hospital city. | VARCHAR(100) | Yes |
| Hospital Privileges | State | Hospital state. | CHAR(2) | Yes |
| Hospital Privileges | ZIP Code | Hospital ZIP code. | VARCHAR(10) | Yes |
| Hospital Privileges | Telephone | Hospital/department telephone. | VARCHAR(25) | Yes |
| Hospital Privileges | Fax | Hospital/department fax. | VARCHAR(25) | Yes |
| Hospital Privileges | Full Unrestricted Privileges | Indicates whether privileges are full and unrestricted. | BOOLEAN | Yes |
| Hospital Privileges | Temporary Privileges | Indicates whether privileges are temporary. | BOOLEAN | Yes |
| Hospital Privileges | Admitting Privilege Status | Status such as none, full unrestricted, provisional, temporary. | VARCHAR(60) | Yes |
| Hospital Privileges | Percent of Total Annual Admissions | Percentage of provider's annual admissions occurring at hospital. | DECIMAL(5,2) | Yes |
| Hospital Privileges | Affiliation Start Date | Month/year affiliation began. | CHAR(7) | Yes |
| Hospital Privileges | Affiliation End Date | Month/year affiliation ended, when applicable. | CHAR(7) | Yes |
| Hospital Privileges | Terminated Affiliation Explanation | Explanation of a terminated affiliation. | TEXT | Yes |
| Hospital Privileges | Department Director Last Name | Department director's last name. | VARCHAR(80) | Yes |
| Hospital Privileges | Department Director First Name | Department director's first name. | VARCHAR(80) | Yes |
| Hospital Privileges | Department Director Middle Initial | Department director's middle initial. | CHAR(1) | Yes |
| Professional Liability Insurance Carrier | No Malpractice Insurance Indicator | Indicates provider does not carry malpractice/professional liability insurance and skips section. | BOOLEAN | Yes |
| Professional Liability Insurance Carrier | Self-Insured | Indicates self-insured coverage. | BOOLEAN | Yes |
| Professional Liability Insurance Carrier | Carrier or Self-Insured Name | Insurer or self-insured entity name. | VARCHAR(160) | Yes |
| Professional Liability Insurance Carrier | Street Number | Carrier address number. | VARCHAR(20) | Yes |
| Professional Liability Insurance Carrier | Street | Carrier street. | VARCHAR(120) | Yes |
| Professional Liability Insurance Carrier | Suite/Building | Carrier suite/building. | VARCHAR(50) | Yes |
| Professional Liability Insurance Carrier | City | Carrier city. | VARCHAR(100) | Yes |
| Professional Liability Insurance Carrier | State | Carrier state. | CHAR(2) | Yes |
| Professional Liability Insurance Carrier | ZIP Code | Carrier ZIP. | VARCHAR(10) | Yes |
| Professional Liability Insurance Carrier | Policy Number | Professional liability policy number. | VARCHAR(60) | Yes |
| Professional Liability Insurance Carrier | Original Effective Date | Original policy effective month/year. | CHAR(7) | Yes |
| Professional Liability Insurance Carrier | Effective Date | Coverage effective month/year. | CHAR(7) | Yes |
| Professional Liability Insurance Carrier | Expiration Date | Coverage expiration month/year. | CHAR(7) | Yes |
| Professional Liability Insurance Carrier | Coverage Type | Individual or shared coverage. | VARCHAR(20) | Yes |
| Professional Liability Insurance Carrier | Unlimited Coverage | Indicates unlimited coverage. | BOOLEAN | Yes |
| Professional Liability Insurance Carrier | Tail Coverage | Indicates whether policy includes tail coverage. | BOOLEAN | Yes |
| Professional Liability Insurance Carrier | Coverage Per Occurrence | Monetary coverage limit per occurrence. | DECIMAL(15,2) | Yes |
| Professional Liability Insurance Carrier | Aggregate Coverage | Monetary aggregate coverage limit. | DECIMAL(15,2) | Yes |
| Military Duty | Active Military Duty or Reserve | Indicates whether provider is currently on active military duty or in military reserve. | BOOLEAN | No |
| Work History | Practice / Employer Name | Employer/practice name. | VARCHAR(160) | Yes |
| Work History | Street Number | Employer address number. | VARCHAR(20) | Yes |
| Work History | Street | Employer street. | VARCHAR(120) | Yes |
| Work History | Suite/Building | Employer suite/building. | VARCHAR(50) | Yes |
| Work History | City | Employer city. | VARCHAR(100) | Yes |
| Work History | State | Employer state/province. | VARCHAR(50) | Yes |
| Work History | ZIP/Postal Code | Employer ZIP/postal code. | VARCHAR(20) | Yes |
| Work History | Country Code | Employer country code. | CHAR(3) | Yes |
| Work History | Start Date | Month/year work began. | CHAR(7) | Yes |
| Work History | End Date | Month/year work ended. | CHAR(7) | Yes |
| Work History | Reason for Departure | Reason provider left the position, if applicable. | TEXT | Yes |
| Work History | Telephone | Employer telephone. | VARCHAR(25) | Yes |
| Work History | Fax | Employer fax. | VARCHAR(25) | Yes |
| Gaps in Professional / Work History | Gap Start Date | Month/year gap began. | CHAR(7) | Yes |
| Gaps in Professional / Work History | Gap End Date | Month/year gap ended. | CHAR(7) | Yes |
| Gaps in Professional / Work History | Gap Explanation | Explanation of gap in training/work history. | TEXT | Yes |
| Professional References | Reference Last Name | Professional reference last name; three references are required on the main form. | VARCHAR(80) | Yes |
| Professional References | Reference First Name | Professional reference first name. | VARCHAR(80) | Yes |
| Professional References | Reference Provider Type Code | Provider type code for reference. | CHAR(3) | Yes |
| Professional References | Street Number | Reference address number. | VARCHAR(20) | Yes |
| Professional References | Street | Reference street. | VARCHAR(120) | Yes |
| Professional References | Apt/Suite/Building | Reference address unit/building. | VARCHAR(50) | Yes |
| Professional References | City | Reference city. | VARCHAR(100) | Yes |
| Professional References | State | Reference state. | CHAR(2) | Yes |
| Professional References | ZIP Code | Reference ZIP code. | VARCHAR(10) | Yes |
| Professional References | Telephone | Reference telephone. | VARCHAR(25) | Yes |
| Professional References | Fax | Reference fax. | VARCHAR(25) | Yes |
| Disclosure Questions | Q1 — Licensure/Registration/Certification Adverse Action | Yes/no response regarding relinquishment, denial, suspension, revocation, restriction, fines, reprimands, consent orders, probation, conditions or limitations. | BOOLEAN | No |
| Disclosure Questions | Q2 — Challenge to Licensure/Registration/Certification | Yes/no response regarding any challenge to licensure, registration or certification. | BOOLEAN | No |
| Disclosure Questions | Q3 — Hospital Privileges/Medical Staff Adverse Action | Yes/no response regarding denial, suspension, revocation, restriction, nonrenewal, probation/discipline, or proceedings concerning clinical privileges/medical staff membership. | BOOLEAN | No |
| Disclosure Questions | Q4 — Surrender/Limitation/Non-Reapplication for Privileges Under Investigation | Yes/no response regarding surrendering or limiting privileges or not reapplying while under investigation. | BOOLEAN | No |
| Disclosure Questions | Q5 — Managed Care Participation Termination/Discipline | Yes/no response regarding termination/nonrenewal for cause or disciplinary action by managed care/provider organizations. | BOOLEAN | No |
| Disclosure Questions | Q6 — Training Program Probation/Discipline/Resignation | Yes/no response regarding probation, discipline, reprimand, suspension or requested resignation during clinical education/training. | BOOLEAN | No |
| Disclosure Questions | Q7 — Training Withdrawal/Termination Under Investigation | Yes/no response regarding withdrawal or premature termination from training while under or avoiding investigation. | BOOLEAN | No |
| Disclosure Questions | Q8 — Board Certification/Eligibility Revoked | Yes/no response regarding revocation of board certification or eligibility. | BOOLEAN | No |
| Disclosure Questions | Q9 — Re-Certification Not Pursued/Surrendered Under Investigation | Yes/no response regarding choosing not to recertify or surrendering board certification while under investigation. | BOOLEAN | No |
| Disclosure Questions | Q10 — DEA/CDS Adverse Action | Yes/no response regarding challenge, denial, suspension, revocation, restriction, nonrenewal, or relinquishment of DEA/CDS authority. | BOOLEAN | No |
| Disclosure Questions | Q11 — Medicare/Medicaid/Government Program Sanction | Yes/no response regarding discipline, exclusion, debarment, suspension, reprimand, sanction, censure, disqualification or restriction in government healthcare programs. | BOOLEAN | No |
| Disclosure Questions | Q12 — Current Investigation/Civil Action | Yes/no response regarding current investigation by hospital/licensing/DEA/CDS/training/government or private health program, or relevant civil action. | BOOLEAN | No |
| Disclosure Questions | Q13 — NPDB/HIPDB Report | Yes/no response whether provider knows of information reported to NPDB or former HIPDB. | BOOLEAN | No |
| Disclosure Questions | Q14 — Regulatory Agency Sanction/Investigation | Yes/no response regarding sanctions or investigation by regulatory agencies such as CLIA or OSHA. | BOOLEAN | No |
| Disclosure Questions | Q15 — Sexual Harassment/Illegal Misconduct Action | Yes/no response regarding specified conviction/plea/sanction/discipline/resignation in exchange for no investigation within 10 years. | BOOLEAN | No |
| Disclosure Questions | Q16 — Military Facility Investigation/Sanction/Resignation | Yes/no response regarding investigation, sanction, reprimand, caution, termination or resignation involving a military hospital/facility/agency. | BOOLEAN | No |
| Disclosure Questions | Q17 — Liability Coverage Cancelled/Restricted/Declined/Nonrenewed | Yes/no response regarding professional liability coverage action based on individual liability history. | BOOLEAN | No |
| Disclosure Questions | Q18 — Liability Surcharge/High-Risk Rating | Yes/no response regarding surcharge or high-risk classification based on individual liability history. | BOOLEAN | No |
| Disclosure Questions | Q19 — Professional Liability Actions in Past 10 Years | Yes/no response regarding pending, settled, arbitrated, mediated or litigated professional liability actions within 10 years. | BOOLEAN | No |
| Disclosure Questions | Q20 — Felony | Yes/no response regarding conviction, guilty plea or nolo contendere plea to a felony. | BOOLEAN | No |
| Disclosure Questions | Q21 — Relevant Misdemeanor/Civil Offense in Past 10 Years | Yes/no response regarding specified misdemeanor/civil findings in the past 10 years. | BOOLEAN | No |
| Disclosure Questions | Q22 — Court-Martial | Yes/no response regarding court-martial for actions related to professional duties. | BOOLEAN | No |
| Disclosure Questions | Q23 — Current Illegal Drug Use | Yes/no response regarding current illegal drug use as defined in the form. | BOOLEAN | No |
| Disclosure Questions | Q24 — Chemical Substance Impairment | Yes/no response regarding chemical substances impairing ability to practice safely. | BOOLEAN | No |
| Disclosure Questions | Q25 — Risk to Patient Safety | Yes/no response regarding reason to believe provider poses a risk to patient safety/well-being. | BOOLEAN | No |
| Disclosure Questions | Q26 — Unable to Perform Essential Functions With Reasonable Accommodation | Yes/no response regarding ability to perform essential practitioner functions even with reasonable accommodation. | BOOLEAN | No |
| Disclosure Questions | Disclosure Question Number | Question number being explained on the supplemental disclosure form. | SMALLINT | Yes |
| Disclosure Questions | Disclosure Explanation | Narrative explanation for a Yes response to a disclosure question. | TEXT | Yes |
| Race and Ethnicity | American Indian or Alaska Native | Optional FHIR-aligned race/ethnicity selection. | BOOLEAN | No |
| Race and Ethnicity | Asian | Optional race/ethnicity selection. | BOOLEAN | No |
| Race and Ethnicity | Black or African American | Optional race/ethnicity selection. | BOOLEAN | No |
| Race and Ethnicity | Hispanic or Latino | Optional race/ethnicity selection. | BOOLEAN | No |
| Race and Ethnicity | Middle Eastern or North African | Optional race/ethnicity selection. | BOOLEAN | No |
| Race and Ethnicity | Native Hawaiian or Other Pacific Islander | Optional race/ethnicity selection. | BOOLEAN | No |
| Race and Ethnicity | White | Optional race/ethnicity selection. | BOOLEAN | No |
| Race and Ethnicity | Prefer Not to Say | Optional non-disclosure choice. | BOOLEAN | No |
| Race and Ethnicity | Do Not Have Information to Answer | Indicates provider does not have information to answer race/ethnicity question. | BOOLEAN | No |
| Standard Authorization, Attestation and Release | Printed Name | Provider's printed name associated with authorization/attestation. | VARCHAR(160) | No |
| Standard Authorization, Attestation and Release | Signature | Provider signature; in a digital system typically represented as an e-signature artifact/reference rather than free text. | VARCHAR(255) | No |
| Standard Authorization, Attestation and Release | Date Signed | Date authorization/attestation was signed. | DATE | No |
| Other Relevant Education | Institution/School Issuing Degree | Additional education institution name. | VARCHAR(160) | Yes |
| Other Relevant Education | Street Number | Institution address number. | VARCHAR(20) | Yes |
| Other Relevant Education | Street | Institution street. | VARCHAR(120) | Yes |
| Other Relevant Education | Suite/Building | Institution suite/building. | VARCHAR(50) | Yes |
| Other Relevant Education | City | Institution city. | VARCHAR(100) | Yes |
| Other Relevant Education | State | Institution state/province. | VARCHAR(50) | Yes |
| Other Relevant Education | ZIP/Postal Code | Institution ZIP/postal code. | VARCHAR(20) | Yes |
| Other Relevant Education | Country Code | Institution country code. | CHAR(3) | Yes |
| Other Relevant Education | Start Date | Month/year education began. | CHAR(7) | Yes |
| Other Relevant Education | End/Graduation Date | Month/year education ended/graduation occurred. | CHAR(7) | Yes |
| Other Relevant Education | Degree Awarded | Degree/certificate awarded. | VARCHAR(100) | Yes |
| Other Relevant Education | Telephone | Institution telephone. | VARCHAR(25) | Yes |
| Other Relevant Education | Fax | Institution fax. | VARCHAR(25) | Yes |
| Other Relevant Education | Completed Education at School | Indicates whether education was completed at that institution. | BOOLEAN | Yes |
| Fifth Pathway Education | Institution/Hospital Where U.S. Clinical Training Was Performed | Institution/hospital for Fifth Pathway U.S. clinical training. | VARCHAR(160) | No |
| Fifth Pathway Education | Address | Street address of Fifth Pathway institution. | VARCHAR(160) | No |
| Fifth Pathway Education | City | City. | VARCHAR(100) | No |
| Fifth Pathway Education | State | State. | CHAR(2) | No |
| Fifth Pathway Education | ZIP Code | ZIP code. | VARCHAR(10) | No |
| Fifth Pathway Education | Start Date | Month/year Fifth Pathway clinical training began. | CHAR(7) | No |
| Fifth Pathway Education | End Date | Month/year Fifth Pathway clinical training ended. | CHAR(7) | No |
| Fifth Pathway Education | Telephone | Institution telephone. | VARCHAR(25) | No |
| Fifth Pathway Education | Fax | Institution fax. | VARCHAR(25) | No |
| Partners/Associates Supplemental Form | Practice Location Number | Location to which supplemental partner/associate records belong. | SMALLINT | Yes |
| Partners/Associates Supplemental Form | Practice Name | Practice name used to identify associated location. | VARCHAR(160) | Yes |
| Partners/Associates Supplemental Form | Practice Address | Practice address used to identify associated location. | VARCHAR(255) | Yes |
| Covering Colleagues Supplemental Form | Practice Location Number | Location to which supplemental covering-colleague records belong. | SMALLINT | Yes |
| Covering Colleagues Supplemental Form | Practice Name | Practice name used to identify associated location. | VARCHAR(160) | Yes |
| Covering Colleagues Supplemental Form | Practice Address | Practice address used to identify associated location. | VARCHAR(255) | Yes |
| Additional Practice Location | Location Number | Number identifying each supplemental practice location. | SMALLINT | Yes |
| Malpractice Claims Explanation | Claim Status | Open or closed status of the malpractice claim. | VARCHAR(10) | Yes |
| Malpractice Claims Explanation | Description of Allegations | Narrative description of allegations. | TEXT | Yes |
| Malpractice Claims Explanation | Professional Liability Carrier Involved | Carrier involved in the claim. | VARCHAR(160) | Yes |
| Malpractice Claims Explanation | Carrier Street Number | Carrier address number. | VARCHAR(20) | Yes |
| Malpractice Claims Explanation | Carrier Street | Carrier street. | VARCHAR(120) | Yes |
| Malpractice Claims Explanation | Carrier Suite/Building | Carrier suite/building. | VARCHAR(50) | Yes |
| Malpractice Claims Explanation | Carrier City | Carrier city. | VARCHAR(100) | Yes |
| Malpractice Claims Explanation | Carrier State | Carrier state. | CHAR(2) | Yes |
| Malpractice Claims Explanation | Carrier ZIP Code | Carrier ZIP. | VARCHAR(10) | Yes |
| Malpractice Claims Explanation | Carrier Telephone | Carrier telephone. | VARCHAR(25) | Yes |
| Malpractice Claims Explanation | Policy Number | Policy number associated with claim. | VARCHAR(60) | Yes |
| Malpractice Claims Explanation | Date of Occurrence | Date of alleged occurrence. | DATE | Yes |
| Malpractice Claims Explanation | Date Claim Was Filed | Date claim was filed. | DATE | Yes |
| Malpractice Claims Explanation | Claim Settlement Date | Date claim was settled, if applicable. | DATE | Yes |
| Malpractice Claims Explanation | Amount of Award or Settlement | Monetary award/settlement amount. | DECIMAL(15,2) | Yes |
| Malpractice Claims Explanation | Method of Resolution | Dismissed, settled, mediation, judgment for plaintiff, arbitration, judgment for defendant, or other printed resolution. | VARCHAR(50) | Yes |
| Malpractice Claims Explanation | Defendant Role | Primary defendant or co-defendant. | VARCHAR(20) | Yes |
| Malpractice Claims Explanation | Number of Other Co-Defendants | Count of other co-defendants. | SMALLINT | Yes |
| Malpractice Claims Explanation | Provider Involvement in Case | Provider's involvement, e.g., attending or consulting. | VARCHAR(120) | Yes |
| Malpractice Claims Explanation | Included in NPDB | Provider's best-knowledge indicator whether case is included in NPDB. | BOOLEAN | Yes |
| Malpractice Claims Explanation | Alleged Injury Resulted in Death | Indicates whether alleged injury resulted in death. | BOOLEAN | Yes |
| Malpractice Claims Explanation | Description of Alleged Injury | Narrative description of alleged patient injury. | TEXT | Yes |
