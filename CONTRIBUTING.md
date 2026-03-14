# Contributing to the GS-DIHE Database

Thank you for your interest in contributing to the Global South Collective for Disability Inclusion in Higher Education. This database grows through the knowledge and effort of practitioners, researchers, and advocates across the Global South.

## Ways to Contribute

### 1. Submit Data for Your Institution

If you work at or are familiar with a higher education institution in the Global South, you can contribute by providing data about its disability inclusion practices. We collect information across seven domains:

- Legal & policy context
- Institutional disability policies and offices
- Academic accommodations and support services
- Physical and digital accessibility
- Informal and community-based support systems
- Grievance redressal and student rights mechanisms
- Data collection and research infrastructure

**How to submit**: Fill out our institutional questionnaire (available at [link to be added]) or open an issue in this repository with the information you can provide.

### 2. Correct or Update Existing Entries

If you notice inaccurate or outdated information in the database, please let us know by opening an issue with:

- The institution name and country
- Which field(s) need correction
- The correct information and its source

### 3. Add a Country Profile

If you have expertise on disability inclusion in higher education in a specific country, you can contribute a country profile narrative. See `data/country_profiles/` for the template and existing examples.

### 4. Flag a Best Practice

If you know of an innovative or notable disability inclusion practice at a Global South institution, submit it for the Best Practices collection. Include:

- Institution name and country
- Description of the practice
- Which domain(s) it relates to
- Any published source or documentation

### 5. Join the GS-DIHE Collective

Beyond contributing data, you can join the broader collective — access the discussion forum, connect with practitioners, and participate in the research programme. Visit the GS-DIHE Portal for details.

## Data Standards

When contributing data, please follow the coding standards documented in [docs/coding_guide.md](docs/coding_guide.md):

- Use **Y / N / Partial / Unknown / ND** for binary fields (ND = no data available)
- Use **1–5 Likert scale** for infrastructure ratings
- Use **ISO 3166-1 alpha-3** country codes (IND, ZAF, KEN, BRA, PHL, etc.)
- Use coded accommodation lists: SCR (scribes), EXT (extra time), ALT (alternative formats), AT (assistive technology), NR (note-taking/recording), SL (sign language)
- Always cite your source — every data point should be traceable

## Commit Message Format

If you are submitting changes via pull request, please use descriptive commit messages:

```
Add 3 institutions: Kenya (2), Ghana (1) — Domains 1–3 complete
Update south_africa.md: add 2023 DHET circular reference
Fix: correct CRPD ratification date for Nepal
```

## Language

The database is maintained in English. When sources are in other languages, note the source language in the Source_Language field and provide English translations of key findings. Machine translation is acceptable for initial entry but should be flagged with 'MT' in the notes.

## Ethics

- Do not submit personal information about individual students
- Institutional data should be based on publicly available information or information shared with explicit consent
- If providing information from your own institution, ensure you are authorised to share it
- Respondent details from questionnaires are kept confidential unless consent is given for publication

## Questions?

Open an issue in this repository, or reach out through the GS-DIHE Portal.

---

*All contributions to this repository are licensed under [CC BY 4.0](LICENSE).*
