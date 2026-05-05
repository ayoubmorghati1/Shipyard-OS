---
name: map-workflow
description: Use when mapping a business workflow, diagnosing friction, choosing the first AI-assisted Work System to build, or producing a Work Map.
---

# Map Workflow

Use this skill during the **Map** phase.

Purpose:

> Diagnose the current work and decide what to improve first.

Output:

```text
01-workspace/{business-slug}/{workflow-slug}/01-work-map.md
```

## When To Use

Use when the user says things like:

- map this workflow
- audit this process
- find where AI can help
- choose what to build first
- create a Work Map
- run the Map phase

## Inputs

Read available context from:

- `01-workspace/00-intake.md`
- `01-workspace/{business-slug}/AGENTS.md` if it exists
- `01-workspace/{business-slug}/business-context/` if it exists
- `01-workspace/{business-slug}/business-context/index.md` if it exists
- `01-workspace/{business-slug}/business-context/open-questions.md` if it exists
- `01-workspace/{business-slug}/decisions/decision-log.md` if it exists
- `01-workspace/_template-work-system/01-work-map.md`
- `01-workspace/HOW-IT-WORKS.md`
- existing packages under `01-workspace/`
- `03-connectors/connected-tools.md` when tools matter

If context is missing, interview the user. Ask only the minimum questions needed to create a useful Work Map.

If the intake contains stable business context that is missing from `business-context/`, propose updating the relevant business-context files before or alongside the Work Map.

When you integrate source material or intake answers into business context, update `business-context/source-log.md`. When a gap blocks confident mapping, add it to `business-context/open-questions.md`.

## Level 2 File Behavior

Do not only explain the framework. Interview, reason, create the package folder, and write the file.

Use this standard path:

```text
01-workspace/{business-slug}/{workflow-slug}/01-work-map.md
```

Create this folder if needed:

```text
01-workspace/{business-slug}/{workflow-slug}/live-system-records/
```

Also create blank live record files if missing:

```text
live-interface.md
feedback-scorecard.md
review-notes.md
approved-outputs.md
memory-updates.md
```

If the user is mapping their own business and no business name is given, use:

```text
01-workspace/your-business/{workflow-slug}/
```

Slug rules:

- lowercase
- use hyphens instead of spaces
- remove punctuation
- keep it short and readable

If `01-work-map.md` already exists, update it instead of creating a duplicate.

After writing, tell the user the file path.

## Interview

Ask these, one at a time if needed:

1. What business outcome matters right now?
2. What repeated workflow affects that outcome?
3. What triggers the workflow?
4. What happens today, step by step?
5. Who is involved?
6. What tools or files are involved?
7. Where does it slow down, break, repeat, or depend too much on one person?
8. What should AI help with?
9. What should AI never do alone?
10. How will we know the workflow improved?

## Scoring

Score each opportunity 1-5:

```text
Impact:
Frequency:
Pain:
Readiness:
Ease:
```

Priority Score:

```text
Impact + Frequency + Pain + Readiness + Ease
```

Rule:

> Map many. Build one first.

## Output Format

Produce:

```markdown
# Work Map - {Workflow Name}

## Business Goal

## Workflow Name

## Current Trigger

## Current Steps

## People Involved

## Tools Involved

## Knowledge Sources

## Friction Points

## AI Opportunity

## Risk Level

## Success Metric

## Priority Score

Impact:
Frequency:
Pain:
Readiness:
Ease:
Total:

## Recommendation

## First Build Scope
```

## Quality Standard

A good Work Map is:

- business-led, not tool-led
- plain language
- specific enough to build from
- honest about risk
- focused on one first workflow
