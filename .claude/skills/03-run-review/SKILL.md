---
name: run-review
description: Use when creating a Workflow Playbook, launching a Work System, reviewing usage, running a 30-day review, or improving the system through the learning loop.
---

# Run Review

Use this skill during the **Run** phase.

Purpose:

> Install the system into daily work, create the operating manual, and improve it through feedback.

Outputs:

```text
Workflow Playbook
Feedback Scorecard
Review notes
```

---

## When To Use

Use when the user says things like:

- create the Workflow Playbook
- launch this Work System
- run the review
- do the 30-day review
- improve this workflow
- update memory from feedback

---

## Inputs

Read available context from:

- `templates/workflow-playbook.md`
- `templates/feedback-scorecard.md`
- `templates/work-system-package.md`
- relevant Work Map
- relevant System Blueprint
- any live outputs or feedback records

If no System Blueprint exists, run `/build-system` first.

---

## Create The Workflow Playbook

Define:

- when to use it
- owner
- trigger
- inputs
- steps
- AI role
- skills used
- human role
- review points
- output
- destination
- quality checklist
- metric
- review rhythm

---

## Run The Learning Loop

Use this model:

```text
Feedback detects the issue.
Memory stores the learning.
Control approves the change.
Context, Skills, or Workflow get updated.
```

Never update memory, context, skills, or control rules from a single bad output without human approval.

---

## Output Format: Workflow Playbook

```markdown
# Workflow Playbook — {Workflow Name}

## Purpose

## When To Use

## Owner

## Trigger

## Inputs

## Steps

## AI Role

## Skills Used

## Human Role

## Review Points

## Output

## Destination

## Quality Checklist

## Success Metric

## Review Rhythm

## Feedback Behavior

After each run:

Where approved outputs are saved:

Where issues are logged:

When review happens:

Who approves memory/system updates:
```

---

## Output Format: Feedback Scorecard

```markdown
# Feedback Scorecard — {Workflow Name}

## Metric

Baseline:
Current result:

## Output Quality

Good:
Edited:
Unusable:

## Adoption

Who used it:
How often:
Where it was skipped:

## Failure Points

## Context Gaps

## Skill Gaps

## Control Issues

## Memory Updates

Proposed:
Approved:
Rejected:

## Next Improvement

## Review Date
```

---

## Quality Standard

A good Run phase:

- makes the workflow usable by the team
- defines where outputs go
- avoids vague feedback
- turns learnings into approved updates
- schedules the next review
- leaves the team able to run the system without Shipyard in the room

