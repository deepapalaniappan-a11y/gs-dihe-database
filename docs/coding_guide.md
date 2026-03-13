# GS-DIHE Database: Coding Guide

This document defines the standardised codes, abbreviations, and conventions used across the GS-DIHE Database. All contributors should follow these standards to ensure cross-national comparability.

## Binary and Status Fields

| Code | Meaning |
|------|---------|
| Y | Yes — confirmed present |
| N | No — confirmed absent |
| Partial | Partially present or partially implemented |
| Unknown | Existence is uncertain; could not be determined |
| ND | No data — no information available despite research |

**Important**: Use `ND` (no data) rather than leaving cells blank. Blank cells are ambiguous; `ND` confirms that the researcher looked and could not find information. `N` means the researcher confirmed the absence.

## Country Codes

Use ISO 3166-1 alpha-3 codes:

| Country | Code | Country | Code |
|---------|------|---------|------|
| India | IND | South Africa | ZAF |
| Bangladesh | BGD | Kenya | KEN |
| Nepal | NPL | Ghana | GHA |
| Sri Lanka | LKA | Nigeria | NGA |
| Pakistan | PAK | Ethiopia | ETH |
| Philippines | PHL | Rwanda | RWA |
| Indonesia | IDN | Uganda | UGA |
| Vietnam | VNM | Brazil | BRA |
| Thailand | THA | Mexico | MEX |
| Malaysia | MYS | Colombia | COL |
| Egypt | EGY | Argentina | ARG |
| Jordan | JOR | Chile | CHL |
| Morocco | MAR | China | CHN |
| Tunisia | TUN | Mongolia | MNG |
| UAE | ARE | Fiji | FJI |

## Institution Type Codes

| Code | Meaning |
|------|---------|
| PUB | Public / government-funded university |
| PVT | Private university |
| AUTO | Autonomous institution (India-specific) |
| DEEMED | Deemed university (India-specific) |
| TECH | Technical / polytechnic institution |
| OPEN | Open university / distance learning |

## Accommodation Codes

Used in the `Exam_Accommodations` field as comma-separated lists:

| Code | Accommodation |
|------|--------------|
| SCR | Scribes / amanuensis |
| EXT | Extra time |
| ALT | Alternative formats (Braille, large print, digital) |
| AT | Assistive technology permitted during exams |
| NR | Note-taking / recording support |
| SL | Sign language interpretation |
| SEP | Separate exam room |
| FLX | Flexible scheduling |
| RDR | Reader (oral reading of exam) |
| CMP | Computer / word processor in lieu of handwriting |

Example: `SCR,EXT,ALT,SEP` means the institution provides scribes, extra time, alternative formats, and separate exam rooms.

## Infrastructure Accessibility Rating (1–5)

| Rating | Description |
|--------|-------------|
| 1 | No accessibility features observed or documented |
| 2 | Minimal — isolated features (e.g., one ramp at main building) |
| 3 | Moderate — some accessible infrastructure, significant gaps remain |
| 4 | Good — most buildings accessible, systematic approach visible |
| 5 | Comprehensive — universal design principles applied, full accessibility |

## WCAG Compliance Levels

| Code | Meaning |
|------|---------|
| A | WCAG 2.1 Level A |
| AA | WCAG 2.1 Level AA |
| AAA | WCAG 2.1 Level AAA |
| NONE | No WCAG compliance detected |
| ND | Not assessed / no data |

## Data Completeness Score

Calculated as the percentage of applicable fields with substantive data (including confirmed negatives):

| Range | Band | Meaning |
|-------|------|---------|
| 0–25% | Identification | Only basic institutional info populated |
| 26–50% | Partial | 1–2 domains populated |
| 51–75% | Moderate | 3–5 domains populated |
| 76–100% | Comprehensive | 6–7 domains with substantive data |

## Source Language Codes

| Code | Language |
|------|----------|
| EN | English |
| HI | Hindi |
| PT | Portuguese |
| ES | Spanish |
| FR | French |
| AR | Arabic |
| MT | Machine-translated (append to original language, e.g., `PT-MT`) |

## Source Type Codes

Used in the Sources_Log sheet:

| Code | Source Type |
|------|-----------|
| INST | Institutional website / official document |
| GOV | Government / regulatory body |
| ACAD | Academic paper / thesis |
| NGO | NGO report / civil society publication |
| INTL | International body (UNESCO, World Bank, etc.) |
| NEWS | News article / media coverage |
| PRAC | Practitioner knowledge (from questionnaire or interview) |

## Notes Fields

Every domain has a free-text Notes field. Use these for:

- Nuance that coded fields cannot capture
- Contextual observations
- Contradictions between sources
- Notable absence of information
- Emerging practices not yet formalised

Keep notes concise but specific. Avoid generic observations; include details that would help another researcher understand the context.
