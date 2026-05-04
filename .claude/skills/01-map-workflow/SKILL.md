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
Work Map
```

---

## When To Use

Use when the user says things like:

- map this workflow
- audit this process
- find where AI can help
- choose what to build first
- create a Work Map
- run the Map phase

---

## Inputs

Read available context from:

- `shipyard-intake.md`
- `templates/work-map.md`
- `framework/shipyard-work-system.md`
- client-specific files under `clients/` if present

If context is missing, ask only the minimum questions needed to create a useful Work Map.

---

## Level 2 File Behavior

This skill should not only answer in chat. It should create or update the Work System Package files whenever filesystem access is available.

Use this standard path:

```text
clients/{client-slug}/{workflow-slug}/01-work-map.md
```

If the user is mapping Shipyard's own business, use:

```text
clients/shipyard/{workflow-slug}/01-work-map.md
```

If the client or workflow name is missing, ask for it.

Slug rules:

- lowercase
- use hyphens instead of spaces
- remove punctuation
- keep it short and readable

Before writing the Work Map:

1. Create `clients/{client-slug}/{workflow-slug}/` if it does not exist.
2. Create `live-system-records/` inside the package folder if it does not exist.
3. Save the Work Map to `01-work-map.md`.
4. If the file already exists, update it rather than creating a duplicate.

After writing, tell the user the file path.

---

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

---

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

---

## Output Format

Produce:

```markdown
# Work Map — {Workflow Name}

## Business Goal

## Current Workflow

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

Build now / later / ignore.

## First Build Scope
```

---

## Quality Standard

A good Work Map is:

- business-led, not tool-led
- plain language
- specific enough to build from
- honest about risk
- focused on one first workflow
