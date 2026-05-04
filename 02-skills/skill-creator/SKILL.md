---
name: skill-creator
description: Use when creating a reusable Shipyard skill from a repeated task, workflow step, or proven prompt pattern.
---

# Skill Creator

Use this skill to create reusable skills for Shipyard-OS.

Output location:

```text
02-skills/user-created/{skill-slug}/SKILL.md
```

## When To Use

Use when a workflow step repeats across multiple Work Systems and deserves reusable instructions.

Examples:

- analyze a sales call
- draft a proposal
- summarize a meeting
- turn feedback into memory updates
- create a weekly leadership brief

## Do Not Use

Do not create a skill for a one-off task.

Do not create tiny skills like "summarize" or "rewrite" unless the business has a specific SOP for them.

## Interview

Ask only what is needed:

1. What job should this skill perform?
2. When should it be used?
3. What inputs does it need?
4. What process should it follow?
5. What output should it produce?
6. What should it avoid?
7. What does a good example look like?

## Skill Format

Create:

```markdown
---
name: {skill-slug}
description: Use when {clear trigger and job}.
---

# {Skill Name}

## Purpose

## When To Use

## Inputs

## Process

## Output

## Review Rules

## Good Example

## Failure Modes
```

## Quality Standard

A good skill:

- has a clear trigger
- is reusable across Work Systems
- is specific enough to produce consistent output
- includes review rules
- stays concise
