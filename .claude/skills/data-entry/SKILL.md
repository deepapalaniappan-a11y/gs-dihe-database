# Data Entry Skill — GS-DIHE Database

## When to Use
Use this skill when asked to add institutions, update data, create country profiles, or modify the database.

## Adding New Institutions
1. Assign the next available ID in CC-NNN format (e.g., IND-055, ZAF-001)
2. Fill ALL fields — use ND (no data) for missing information, NEVER leave blank
3. Use the coding standards from CLAUDE.md exactly
4. Add the source URL to sources/source_log.csv
5. Update the relevant country profile in data/country_profiles/

## Coding Standards (Critical)
- Binary: Y / N / Partial / Unknown / ND
- Infrastructure: 1–5 Likert
- Accommodations: SCR / EXT / ALT / AT / NR / SL
- Countries: ISO alpha-3 (IND, ZAF, KEN, BRA, PHL)
- Institution IDs: CC-NNN (IND-001, ZAF-001)

## CSV Operations
When updating CSV files:
```python
import csv
# Always use utf-8 encoding
# Always preserve existing headers
# Append new rows, never overwrite existing data
```

## Excel Operations
When updating .xlsx files:
```python
import openpyxl
# Always load with data_only=False to preserve formulas
# Always save to a new filename first, verify, then replace
# Never delete sheets — only add data to existing sheets
```

## Country Profile Format (data/country_profiles/)
Each country profile should include:
- Country name, legal framework summary, CRPD status
- Higher education system overview (number of universities, regulatory body)
- Disability legislation relevant to HE
- Key institutions mapped (table format)
- Distinctive features of the country's approach
- Gaps and areas needing more data
- Sources with URLs

## Source Logging
Every new data point must have an entry in sources/source_log.csv:
```
institution_id,source_type,source_url,access_date,notes
IND-055,institutional_website,https://example.edu.in/eoc,2026-03-15,EOC page
```

## Commit Message Format
"Add N institutions: Country (n), Country (n) — Domains X–Y complete"

Example: "Add 3 institutions: India (2), South Africa (1) — Domains 1–4 complete"

## Quality Check Before Committing
- [ ] All new entries have institution IDs assigned
- [ ] No blank fields — all use ND where data is missing
- [ ] Source URLs logged in source_log.csv
- [ ] Country profile updated if adding to a new country
- [ ] Commit message follows the format above
