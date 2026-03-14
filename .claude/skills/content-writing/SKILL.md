# Content Writing Skill — GS-DIHE Knowledge Repository

## When to Use
Use this skill when asked to write, draft, or create content for Knowledge Repository modules (modules 1–12).

## Module Structure
Every module must follow this file structure:
```
modules/module-NN-short-name/
├── README.md            # Main guide (3,000–6,000 words)
├── templates/           # Minimum 3 downloadable tools
│   ├── [tool-1].md
│   ├── [tool-2].md
│   └── [tool-3].xlsx    # If spreadsheet needed
└── case-studies/        # Minimum 2 real institution examples
    ├── [country]-[institution].md
    └── [country]-[institution].md
```

## README.md Structure for Each Module
1. **Title and one-paragraph summary** — what this module covers and why it matters
2. **Who this guide is for** — specify the practitioner audience
3. **The essentials** — 5–8 core operational sections, each answering a specific "how do I..." question
4. **Quick-start checklist** — a numbered list of first steps for someone starting from zero
5. **Global South vs. Western models** — a comparison table or section showing how approaches differ
6. **Case studies** — links to the case-study files with 1-sentence summaries
7. **Templates and tools** — links to the template files with descriptions
8. **Sources and further reading** — with URLs

## Writing Rules
- Lead with Global South examples (India, South Africa, Kenya, Brazil, Philippines)
- Use Western models (UK DSA, US AHEAD, Australia ADCET) as comparison, not as the standard
- Every recommendation must be actionable — "do X, then Y" not "consider the implications of X"
- Include specific numbers, institution names, policy references, and URLs
- Use Markdown formatting: headers, bold for key terms, tables for comparisons
- No bullet-point-only sections — use prose paragraphs with bullet lists for specific items only
- Templates must be ready to use — a practitioner should be able to download and adapt immediately

## Case Study Format
Each case study file should include:
- Institution name, city, country, type
- What they built (the specific system/programme)
- How it works operationally (step by step)
- Scale (number of students served, volunteers involved)
- What makes it distinctive
- Challenges and limitations
- Source URLs

## Quality Check Before Committing
- [ ] README.md is 3,000–6,000 words
- [ ] At least 3 templates in templates/
- [ ] At least 2 case studies in case-studies/
- [ ] All factual claims have source URLs
- [ ] Global South examples appear before Western ones
- [ ] Quick-start checklist is present and actionable
- [ ] No placeholder text like "TBD" or "[to be added]"
