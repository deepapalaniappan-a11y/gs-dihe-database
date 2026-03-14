# GS-DIHE Database

**Global South Collective for Disability Inclusion in Higher Education — Research Database**

## About

This repository contains the structured research database for the GS-DIHE Collective — the first comprehensive, open-access dataset mapping disability inclusion policies, practices, and support mechanisms in higher education institutions across the Global South.

The database documents institutional-level data across **seven domains**:

1. **Legal & Policy Framework** — National disability legislation, UNCRPD status, HE-specific regulations, judicial precedent
2. **Institutional Policy & Governance** — Disability offices, policies, strategic plans, accreditation criteria
3. **Academic Accommodations & Support** — Exam accommodations, scribes, assistive technology, accessible formats
4. **Physical & Digital Accessibility** — Campus infrastructure, website accessibility, universal design
5. **Informal & Community-Based Support** — Volunteer networks, WhatsApp groups, family involvement, NGO partnerships
6. **Grievance Redressal & Student Rights** — Complaint mechanisms, equal opportunity cells, student rights awareness
7. **Data, Monitoring & Research** — Disability-disaggregated data, self-identification, outcome tracking

## Current Coverage

| Region | Countries | Institutions |
|--------|-----------|-------------|
| South Asia | — | — |
| Southeast Asia | — | — |
| Sub-Saharan Africa | — | — |
| Latin America | — | — |
| MENA | — | — |

*This table is updated as data collection progresses.*

## Repository Structure

```
gs-dihe-database/
├── README.md                        ← You are here
├── LICENSE                          CC BY 4.0
├── CONTRIBUTING.md                  How to contribute data
├── CHANGELOG.md                     Major data update log
├── data/
│   ├── master_database.xlsx         Primary Excel workbook
│   ├── master_database.csv          CSV export (diff-friendly)
│   ├── expert_services.csv          Expert directory export
│   ├── country_profiles/            One .md per country
│   │   ├── india.md
│   │   ├── south_africa.md
│   │   └── ...
│   └── best_practices/              Documented innovations
├── research/
│   ├── questionnaire_v1.md          Institutional survey instrument
│   ├── outreach_tracker.csv         Email/contact tracking
│   ├── email_templates/
│   │   ├── initial_contact.md
│   │   ├── follow_up.md
│   │   └── network_invitation.md
│   └── consent_form.md              Informed consent
├── sources/
│   ├── source_log.csv               Master source log
│   └── policies/                    Downloaded policy PDFs
├── analysis/
│   ├── regional_summaries.md
│   └── figures/
├── conference/
│   ├── ahead_2026_abstract.md
│   ├── ahead_2026_paper.md
│   └── ahead_2026_slides.pptx
└── docs/
    ├── methodology.md
    ├── coding_guide.md
    └── data_dictionary.md
```

## How to Use This Data

The primary workbook (`data/master_database.xlsx`) contains all data across multiple sheets. For programmatic access or version-control-friendly diffs, use the CSV exports.

All data is licensed under [CC BY 4.0](LICENSE) — you are free to use, share, and adapt it with attribution.

### Download Options

- **Full dataset**: Clone this repository or download as ZIP
- **Excel workbook**: Download `data/master_database.xlsx` directly
- **CSV (diff-friendly)**: Download `data/master_database.csv`
- **Individual country profiles**: Browse `data/country_profiles/`

## How to Contribute

We welcome contributions from disability practitioners, researchers, and advocates. See [CONTRIBUTING.md](CONTRIBUTING.md) for details on:

- Submitting data for your institution
- Correcting or updating existing entries
- Adding country profiles or best practices
- Joining the GS-DIHE Collective

## Related Resources

- **GS-DIHE Portal** — [gs-dihe-portal repository](https://github.com/[username]/gs-dihe-portal) — The public-facing knowledge portal and resource library
- **GS-DIHE Knowledge Repository** — 12 practical topic modules for disability practitioners (hosted on the portal)
- **AHEAD 2026** — Research from this database will be presented at the AHEAD conference in November 2026

## Methodology

See [docs/methodology.md](docs/methodology.md) for the full research methodology, including data collection layers, coding standards, and quality assurance protocols.

## Citation

If you use this dataset in your work, please cite:

> GS-DIHE Collective. (2026). *Global South Disability Inclusion in Higher Education Database*. https://github.com/[username]/gs-dihe-database

## Contact

For questions, corrections, or collaboration enquiries, open an issue in this repository or contact us through the GS-DIHE Portal.

---

*The GS-DIHE Collective — Global South Collective for Disability Inclusion in Higher Education*
