# U.S. Undergrad School Selection Skill

This repository contains a Codex skill for building customized U.S. undergraduate school lists for international applicants.

It is designed for students, families, and counselors who want a more grounded college list based on official school data instead of rankings alone. The skill emphasizes:

- official `Common Data Set (CDS)` sources
- official admissions and international student pages
- international financial aid and merit scholarship reality
- major-specific selectivity, especially for `Computer Science`
- a balanced `20-school` list with school-by-school rationale

## Included Skill

This repository includes:

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

After installation, Codex should be able to discover the skill as:

```text
$us-undergrad-school-selection
```

## English Example Prompts

```text
Use $us-undergrad-school-selection to build a 20-school U.S. undergraduate list for an international applicant using the latest official CDS data and current school policies.
```

```text
Use $us-undergrad-school-selection. The student is a Chinese international applicant in grade 11 with IB 42/45 predicted, SAT 1520, intended major in computer science, annual family budget of 60000 USD, and a preference for East Coast medium-to-large universities. Build a 20-school list and explain why each school is recommended.
```

```text
Use $us-undergrad-school-selection to rebalance my current college list. Keep only schools that are realistic for an aid-seeking international student and explain which schools are admission reaches versus financial anchors.
```

## Chinese Example Prompts

```text
使用 $us-undergrad-school-selection。请基于学生背景、最新官方 CDS 和学校官网信息，为申请美国本科的国际生生成一个 20 所学校的选校方案，并解释每所学校为什么推荐。
```

```text
使用 $us-undergrad-school-selection。学生是中国国际生，11 年级，IB 体系，预估 42/45，SAT 1520，想申请计算机专业，家庭预算每年 6 万美元，需要考虑奖学金，偏好美国东海岸和中大型大学。请给出 20 所学校的推荐名单，并说明每所学校的录取匹配度、预算匹配度和主要风险。
```

```text
使用 $us-undergrad-school-selection。请帮我重新平衡现有选校名单，去掉对需要资助的国际生不现实的学校，并补充更适合作为 financial anchor 的学校。
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

## Feedback

If you use this skill and notice a missing decision factor or a recommendation that feels clearly wrong, structured feedback is more useful than general comments.

The most helpful feedback includes:

- the student profile type
- the main strategy mode, such as ranking-first or budget-first
- any new selection factor the skill did not handle well
- schools that should have been removed, downgraded, upgraded, or added
- whether the `30-school` longlist, `20-school` shortlist, or `ED/EA/RD` strategy felt inaccurate

Suggested feedback format:

```text
Case type:
- Curriculum:
- International status:
- Academic level:
- Intended field:
- Primary strategy mode:

New factor:
- Factor:
- User wording:
- Classification:
- Was it handled well:
- If not, what went wrong:

Recommendation error:
- Error type:
- School(s) involved:
- What should have changed:

Outcome:
- 30-school list useful:
- 20-school list useful:
- Early-round strategy useful:
- Main inaccuracy:
```
