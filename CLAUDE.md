# GS-DIHE Database — Project Guide for Claude

## Project Identity

**Global South Collective for Disability Inclusion in Higher Education (GS-DIHE)**
A research database and knowledge repository mapping disability inclusion infrastructure across Global South universities, targeting the AHEAD 2026 conference (November 2026).

- **Owner:** Deepa Palaniappan (deepapalaniappan-a11y)
- **License:** CC BY 4.0
- **Primary audience:** Disability practitioners, accessibility officers, and policy researchers at Global South universities

## Repository Structure

```
gs-dihe-database/
├── CLAUDE.md                    # This file — project context for Claude
├── README.md                    # Public-facing repository description
├── LICENSE                      # CC BY 4.0
├── CONTRIBUTING.md              # Contribution guidelines
├── CHANGELOG.md                 # Version history
├── .gitignore
├── data/
│   ├── master_database.xlsx     # 12-sheet workbook (7-domain framework)
│   ├── master_database.csv      # Diff-friendly export
│   ├── expert_services.csv
│   └── country_profiles/
│       ├── india.md             # Substantive — 54 institutions mapped
│       ├── south_africa.md      # Placeholder
│       ├── kenya.md             # Placeholder
│       ├── brazil.md            # Placeholder
│       └── philippines.md       # Placeholder
├── docs/
│   ├── coding_guide.md          # Y/N/Partial/Unknown/ND coding standards
│   ├── data_dictionary.md       # 59-column schema documentation
│   └── methodology.md           # Data collection methodology
├── modules/                     # Knowledge Repository modules
│   └── module-03-scribe-volunteer-management/  # First module (building)
│       ├── README.md            # Main practitioner guide
│       ├── templates/           # Downloadable tools
│       └── case-studies/        # Institution profiles
├── research/
│   ├── questionnaire_v1.md
│   ├── outreach_tracker.csv
│   ├── consent_form.md
│   └── email_templates/
├── sources/
│   └── source_log.csv
├── analysis/
│   └── regional_summaries.md
└── conference/
    ├── ahead_2026_abstract.md
    └── ahead_2026_paper.md
```

## Seven-Domain Framework

All institutional data is organized across these domains:
1. **Legal & Policy** — national law, CRPD ratification, HE regulation, judicial precedent
2. **Institutional Policy & Governance** — disability office, policy documents, strategic plan
3. **Academic Accommodations** — exams, scribes, AT, extra time, accessible formats
4. **Physical & Digital Access** — campus rating (1–5 Likert), WCAG, universal design
5. **Informal & Community Support** — volunteers, WhatsApp networks, family, NGOs
6. **Grievance Redressal** — complaints mechanisms, anti-discrimination, rights awareness
7. **Data & Research** — disability data collection, self-identification, outcome tracking

## Coding Standards

- **Binary fields:** Y / N / Partial / Unknown / ND (no data). NEVER leave blank — use ND.
- **Infrastructure ratings:** 1–5 Likert scale
- **Accommodation codes:** SCR (scribe), EXT (extra time), ALT (alternative format), AT (assistive tech), NR (note reader), SL (sign language)
- **Country codes:** ISO 3166-1 alpha-3 (IND, ZAF, KEN, BRA, PHL)
- **Institution IDs:** CC-NNN format (e.g., IND-001, ZAF-001)
- **Commit message format:** "Add 3 institutions: India (2), Kenya (1) — Domains 1–3 complete"

## 12 Knowledge Repository Modules

| # | Module | Status | Priority |
|---|--------|--------|----------|
| 1 | Setting Up a Disability Office | Not started | Tier 2 |
| 2 | Reasonable Accommodations | Not started | Tier 1 |
| 3 | Scribe & Volunteer Management | **Building now** | Tier 1 |
| 4 | Assistive Technology on a Budget | Not started | Tier 1 |
| 5 | Campus Physical Accessibility | Not started | Tier 3 |
| 6 | Digital Accessibility | Not started | Tier 2 |
| 7 | Grievance Redressal Mechanisms | Not started | Tier 2 |
| 8 | Faculty & Staff Training | Not started | Tier 1 |
| 9 | Government Policies Navigator | Not started | Tier 2 |
| 10 | Funding & Resource Mobilization | Not started | Tier 3 |
| 11 | Data Collection & Reporting | Not started | Tier 3 |
| 12 | Informal & Community Support | Not started | Tier 3 |

## Module File Structure Convention

Each module lives at `modules/module-NN-short-name/` and contains:
- `README.md` — Main practitioner guide (the module content)
- `templates/` — Downloadable tools (checklists, forms, spreadsheets)
- `case-studies/` — Real institution examples with source URLs

## Writing Style & Tone

- **Practical over theoretical** — every section should answer "what do I do Monday morning?"
- **Asset narrative** — document what Global South institutions HAVE built, not just gaps
- **Global South first, Western reference second** — Indian/African/Latin American examples lead; UK/US/Australia are comparison points
- **Specific and grounded** — name institutions, cite policies, give numbers
- **No generic academic language** — write for a practitioner setting up a disability office, not a journal reviewer

## Key India Legal Framework (applies to all IND- entries)

- RPwD Act 2016: 5% reservation, reasonable accommodation (s.2(y)), non-discrimination (s.16–18)
- CRPD: Ratified
- UGC: HEPSN scheme, Accessibility Guidelines 2022, Equal Opportunity Centres directive
- NEP 2020: Inclusive education provisions
- Key precedent: Vikash Kumar v. UPSC (2021) — substantive, not merely formal accommodation
- Government scribe guidelines: August 2018 OM, August 2022 OM (post-Vikas Kumar), August 2025 Revised Guidelines

## Restrictions for Claude

- **DO NOT** modify CLAUDE.md, workflow files, or LICENSE without explicit instruction
- **DO NOT** delete any existing data — only add or update
- **DO NOT** push directly to main — always create a branch and open a PR
- **DO NOT** fabricate institutional data — if unsure, mark as ND (no data) or Unknown
- **DO** follow the coding standards above exactly
- **DO** cite sources with URLs for any factual claims about institutions
- **DO** run `python -c "import openpyxl"` to verify Python dependencies before Excel operations
- **DO** create meaningful commit messages following the format above
