# GS-DIHE Research Methodology

## Overview

The GS-DIHE Database uses a mixed-methods approach combining desk-based secondary research with primary data collection through institutional surveys. The guiding principle in early phases is **depth over breadth** — comprehensive, well-sourced entries for fewer institutions are more valuable than skeletal entries for many.

## Data Collection Layers

1. **Institutional Websites** — University disability/accessibility office pages, policy repositories, strategic plans, annual reports.
2. **National Regulators** — UGC (India), DHET (South Africa), CHED (Philippines), MEC (Brazil), etc. — mandates, guidelines, data.
3. **Published Literature** — Academic papers, NGO reports, UNESCO/World Bank publications, CRPD shadow reports, doctoral theses.
4. **Toolkits & Guidelines** — Published disability inclusion toolkits from international and local organisations.
5. **Primary Research** — Questionnaire responses, practitioner interviews, and community contributions through the GS-DIHE network.
6. **News & Media** — News articles about institutional disability initiatives, court cases, student activism, government announcements. Monitored through Google Alerts, university press offices, and disability-focused news outlets. Particularly important for Domains 1, 5, and 6.

**Note on web scraping**: For large-scale screening, lightweight web scraping tools (Python scripts checking university websites for disability-related keywords) may be used to identify which institutions have visible disability content online. This serves as a triage mechanism to prioritise manual research. Scripts and methods are documented in this file as they are developed.

## Seven-Domain Framework

All data collection follows the seven-domain framework documented in the [data dictionary](data_dictionary.md). Researchers work through each institution systematically by domain, recording findings and marking gaps with 'ND' (no data) rather than leaving cells blank.

## Source Standards

### Priority sources (highest reliability):
- National legislation and regulatory directives
- Published institutional policies
- Peer-reviewed research
- UNESCO/World Bank publications
- AHEAD/EADSNE guidelines

### Secondary sources:
- News articles and media coverage
- NGO and civil society reports
- Conference presentations and working papers

### Practitioner knowledge:
- Contributions from the GS-DIHE network are clearly identified as practitioner-reported data, not independently verified unless confirmed by documentary evidence.

## Quality Assurance

- Every entry includes a Completeness Score (0–100%)
- Every factual claim is traceable to a source in the Sources_Log
- Source language is always recorded
- Machine translation is flagged with 'MT'
- Data is reviewed on Fridays during consolidation sessions
- Periodic verification passes are conducted before major milestones

## Ethics

- Individual student information is never recorded
- Institutional data is based on publicly available information or information shared with informed consent
- Questionnaire respondents' personal details are confidential unless consent is given
- The research follows the consent framework in `research/consent_form.md`
