---
name: us-undergrad-school-selection
description: Build customized U.S. undergraduate school lists for international applicants and their families. Use when Codex needs to recommend, compare, expand, or rebalance 20-school college lists; interpret official Common Data Set (CDS), admissions, international admissions, and financial-aid pages; estimate reach, target, and likely positioning for an international student; or explain why specific U.S. colleges fit a student's academics, budget, intended major, and family preferences.
---

# U.S. Undergrad School Selection

## Goal
Build a realistic, personalized U.S. undergraduate school list for an international applicant using the latest official school data and the student's family context. Default to a 20-school plan unless the user asks for a different scope.

## Operating Rules
- Browse the web before giving school-specific advice. Prefer the latest official CDS PDF or CDS webpage for quantitative data.
- Cite the exact source type and year for every material claim. Example: `CDS 2024-2025, Section C9` or `official international admissions page`.
- If the latest CDS is missing, use the most recent official CDS available and clearly say so. Supplement gaps with official admissions, international admissions, financial aid, registrar, academic department, and institutional research pages.
- Never invent CDS values, aid policies, admit rates, or test requirements.
- Separate `admission fit`, `financial fit`, and `preference fit`. A school can be academically plausible but financially unrealistic.
- Be conservative about the word `safety` for international applicants, especially for aid-seeking students and capped majors. If needed, use `lottery reach`, `reach`, `target`, `possible likely`, and `financial anchor` instead.
- Adapt the response language to the user.

## Workflow

### 1. Build the Applicant Brief
Load `references/profile-intake.md`.

Collect or infer:
- citizenship, current country, curriculum, and school type
- grade level, GPA/transcript context, course rigor, rank if available
- SAT or ACT, TOEFL or IELTS or Duolingo, AP or IB or A-Level or predicted scores
- intended major, alternate majors, and whether direct admission to major matters
- extracurricular profile, awards, research, portfolio, audition, or athletics hooks
- family budget in USD, need for aid, openness to loans, and merit-scholarship expectations
- geographic, size, campus, climate, safety, and culture preferences
- family priorities such as prestige, outcomes, affordability, flexibility, or support for international students
- application strategy constraints such as ED, REA, EA, or RD

If critical inputs are missing, ask focused follow-up questions. If the user wants a fast first pass, state the assumptions explicitly and continue.

### 2. Convert the Brief into Decision Rules
Create four buckets:
- `must-have`
- `strong preference`
- `nice to have`
- `hard no`

Also note hidden constraints that change list quality:
- major competitiveness
- aid sensitivity
- willingness to consider liberal arts colleges
- tolerance for cold weather, rural campuses, or religious affiliation
- willingness to include schools with uncertain aid for international students

### 3. Gather School Data
Load `references/cds-checklist.md`.

For each school under consideration:
- pull key CDS indicators from the latest official CDS
- add official international admissions and financial-aid policy details that CDS does not fully capture
- check whether the intended major is easy to enter, capped, portfolio-based, or direct-admit
- verify current test policy and English proficiency requirements
- record cost-of-attendance and international-aid notes separately from raw admit selectivity

Do not rely on ranking summaries, unofficial blogs, or aggregator sites when an official source exists.

### 4. Score and Filter
Load `references/scoring-framework.md`.

Evaluate each school on five dimensions:
- admission competitiveness
- affordability and aid realism
- academic and major fit
- outcomes and support environment
- preference fit

Adjust weights to the case. If budget is tight, increase affordability weight. If the student is applying to a selective program such as engineering, business, CS, nursing, design, or film, increase major-access weight.

### 5. Build the 20-School Portfolio
Unless the user asks otherwise, aim for a diversified list of 20 schools.

Typical starting structure:
- 4 lottery reach
- 6 reach
- 6 target
- 4 possible likely or financial anchor

Adjust the mix when necessary:
- aid-seeking international students may have few true safeties
- ultra-selective applicants may need more financial anchors
- students with narrow geographic limits may need fewer tiers and more tradeoff discussion

Do not include a school only because it is famous. Every school must survive the student's constraints and have a school-specific rationale.

### 6. Explain the Recommendation
Load `references/output-template.md`.

For every recommended school, explain:
- why it fits the student's academic and personal profile
- which sourced facts support the recommendation
- what the main risk or tradeoff is
- why it belongs in that tier rather than a safer or riskier tier

### 7. Sanity Check Before Finalizing
Confirm that:
- no school violates a `must-have` without a clear explanation
- cost and aid comments distinguish sticker price from likely affordability
- direct-entry or capped-major barriers are not hidden
- no claim depends on unsourced or stale data
- the final list is balanced by selectivity, cost strategy, and student preferences

## International Applicant Rules
- Treat `need-aware for internationals`, `limited aid`, and `merit scholarships only` as major strategic variables.
- If the family needs substantial aid, call out that many schools become more selective in practice than their published overall CDS admit rate suggests.
- If English testing, portfolio review, or national curriculum conversion is a potential blocker, surface it early.
- If the student prefers to compare U.S. News style prestige, reframe the discussion around fit, affordability, outcomes, and application strategy instead of refusing the request.

## Quality Bar
- Use school-specific reasons, not generic praise.
- Mention the CDS year whenever CDS is used.
- Link every school recommendation to at least one academic or admissions fact and one fit or finance fact.
- If data quality is uneven, say what is known, what is missing, and how that uncertainty changes the recommendation.
