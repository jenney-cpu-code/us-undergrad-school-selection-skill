# U.S. Undergrad School Selection Skill

This repository contains a Codex skill for building customized U.S. undergraduate school lists for international applicants.

The skill is designed for families, students, and counselors who want a more grounded college list based on official school data instead of rankings alone. It emphasizes:

- official `Common Data Set (CDS)` sources
- official admissions and international student pages
- international financial aid and merit scholarship reality
- major-specific selectivity, especially for `Computer Science`
- a balanced `20-school` list with school-by-school rationale

## Included Skill

The skill folder in this repository is:

- `us-undergrad-school-selection/`

Install that folder into your local Codex skills directory to use it.

## Installation

Copy the skill folder into:

```bash
~/.codex/skills/
```

Example:

```bash
cp -R us-undergrad-school-selection ~/.codex/skills/
```

After that, Codex should be able to discover the skill as:

```text
$us-undergrad-school-selection
```

## Example Prompts

```text
Use $us-undergrad-school-selection to build a 20-school U.S. undergraduate list for an international applicant using the latest official CDS data and current school policies.
```

```text
Use $us-undergrad-school-selection. The student is a Chinese international applicant in grade 11 with IB 42/45 predicted, SAT 1520, intended major in computer science, annual family budget of 60000 USD, and a preference for East Coast medium-to-large universities. Build a 20-school list and explain why each school is recommended.
```

```text
Use $us-undergrad-school-selection to rebalance my current college list. Keep only schools that are realistic for an aid-seeking international student and explain which schools are admission reaches versus financial anchors.
```

## What The Skill Does

- gathers the student and family profile
- translates preferences into decision rules
- checks the latest official `CDS` and official school pages
- separates admission fit from financial fit
- accounts for international applicant constraints
- produces a `20-school` recommendation with reasons and risks

## Notes

- The skill should browse the web before giving school-specific advice.
- Official sources should be prioritized over third-party summaries.
- International aid policies and testing policies can change, so answers should cite the specific year and source used.
