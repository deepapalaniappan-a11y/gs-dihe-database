# GS-DIHE Database: Data Dictionary

Complete column schema for the Master_Database sheet. Each row represents one higher education institution.

## Identification (Columns A–I)

| Column | Field Name | Type | Description |
|--------|-----------|------|-------------|
| A | Institution_ID | Auto | Unique identifier. Format: `CC-NNN` (country code + number, e.g., IND-001) |
| B | Institution_Name | Text | Full official name of the institution |
| C | Country | Text | Country name |
| D | Country_Code | Code | ISO 3166-1 alpha-3 (see coding_guide.md) |
| E | Region | Text | Geographic region (South Asia, Southeast Asia, Sub-Saharan Africa, Latin America, MENA, East Asia, Pacific Islands) |
| F | City | Text | City where main campus is located |
| G | Institution_Type | Code | PUB / PVT / AUTO / DEEMED / TECH / OPEN |
| H | Year_Founded | Number | Year the institution was established |
| I | Approximate_Enrolment | Number | Approximate total student enrolment (most recent available) |

## Domain 1 — Legal & Policy Framework (Columns J–O)

| Column | Field Name | Type | Description |
|--------|-----------|------|-------------|
| J | National_Disability_Law | Text | Name and year of the primary national disability law (e.g., "RPwD Act 2016") |
| K | CRPD_Ratified | Y/N | Whether the country has ratified the UN CRPD |
| L | HE_Specific_Regulation | Text | Any higher education–specific disability regulations or directives |
| M | Key_Legal_Provisions | Text | Key provisions relevant to HE (e.g., "reasonable accommodation mandated", "5% reservation") |
| N | Judicial_Precedent | Text | Relevant court cases affecting institutional practice |
| O | Legal_Notes | Text | Free text — contextual observations on legal framework |

## Domain 2 — Institutional Policy & Governance (Columns P–V)

| Column | Field Name | Type | Description |
|--------|-----------|------|-------------|
| P | Has_Disability_Policy | Status | Y / N / Partial / Unknown / ND |
| Q | Policy_Document_URL | URL | Link to the policy document if publicly available |
| R | Has_Disability_Office | Status | Y / N / Partial / ND |
| S | Office_Name_and_URL | Text+URL | Name of the office/cell and link to its webpage |
| T | Inclusion_in_Strategic_Plan | Status | Y / N / Partial / ND |
| U | Accreditation_Disability_Criteria | Text | Whether accreditation body includes disability criteria and details |
| V | Institutional_Notes | Text | Free text |

## Domain 3 — Academic Accommodations & Support (Columns W–AC)

| Column | Field Name | Type | Description |
|--------|-----------|------|-------------|
| W | Exam_Accommodations | Coded list | Comma-separated codes: SCR, EXT, ALT, AT, NR, SL, SEP, FLX, RDR, CMP |
| X | Assistive_Tech_Provision | Text | Description of AT available |
| Y | Scribes_Available | Status | Y / N / Partial / ND |
| Z | Extra_Time_Policy | Text | Details of extra time allocation |
| AA | Accessible_Formats | Text | Which formats are available (Braille, large print, digital, audio) |
| AB | LMS_Accessibility | Text | Accessibility of the learning management system |
| AC | Academic_Notes | Text | Free text |

## Domain 4 — Physical & Digital Accessibility (Columns AD–AI)

| Column | Field Name | Type | Description |
|--------|-----------|------|-------------|
| AD | Campus_Accessibility_Rating | 1–5 | Likert scale (see coding_guide.md) |
| AE | Infrastructure_Details | Text | Specific features: ramps, lifts, tactile paths, signage, washrooms |
| AF | Website_WCAG_Level | Code | A / AA / AAA / NONE / ND |
| AG | Digital_Tools | Text | Assistive technologies in labs/libraries |
| AH | Universal_Design_Adoption | Text | Whether UD principles are applied in new construction |
| AI | Access_Notes | Text | Free text |

## Domain 5 — Informal & Community Support (Columns AJ–AO)

| Column | Field Name | Type | Description |
|--------|-----------|------|-------------|
| AJ | Volunteer_Networks | Text | Description of student volunteer programmes supporting disability |
| AK | Peer_Support_Mechanisms | Text | Peer mentoring, buddy systems, support groups |
| AL | WhatsApp_Informal_Groups | Status+Text | Y / N / ND, plus description if known |
| AM | Family_Involvement_Pattern | Text | Role of families in accommodation and support |
| AN | NGO_Partnerships | Text | External organisations partnering with the institution |
| AO | Informal_Notes | Text | Free text |

## Domain 6 — Grievance Redressal & Student Rights (Columns AP–AU)

| Column | Field Name | Type | Description |
|--------|-----------|------|-------------|
| AP | Has_Complaint_Mechanism | Status | Y / N / Partial / ND |
| AQ | Anti_Discrimination_Provision | Text | Specific provisions for disability-based discrimination |
| AR | Equal_Opportunity_Cell | Status+Text | Y / N / ND, plus name and details |
| AS | Student_Rights_Awareness | Text | How students are informed of their rights |
| AT | Documented_Cases | Text | Any publicly known complaint cases or outcomes |
| AU | Grievance_Notes | Text | Free text |

## Domain 7 — Data, Monitoring & Research (Columns AV–BA)

| Column | Field Name | Type | Description |
|--------|-----------|------|-------------|
| AV | Collects_Disability_Data | Status | Y / N / Partial / ND |
| AW | Self_ID_Mechanism | Text | How students self-identify as having a disability |
| AX | Research_Output | Text | Institutional research publications on disability |
| AY | National_Data_Participation | Text | Whether institution reports to national disability data systems |
| AZ | Outcome_Tracking | Text | Whether completion/graduation rates are tracked by disability status |
| BA | Data_Notes | Text | Free text |

## Metadata (Columns BB–BG)

| Column | Field Name | Type | Description |
|--------|-----------|------|-------------|
| BB | Data_Source_Primary | Text | Main source used for this entry |
| BC | Data_Source_Secondary | Text | Additional sources |
| BD | Source_Language | Code | EN / HI / PT / ES / FR / AR / MT (see coding_guide.md) |
| BE | Date_Last_Updated | Date | YYYY-MM-DD format |
| BF | Completeness_Score | Percentage | 0–100% (see coding_guide.md) |
| BG | Researcher_Notes | Text | Internal notes, flags for follow-up, quality observations |
