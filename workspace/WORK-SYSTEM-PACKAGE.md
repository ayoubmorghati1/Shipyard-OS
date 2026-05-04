# Work System Package

A Work System Package is the folder for one AI-assisted workflow.

It is the thing you build, teach, hand off, run, and improve.

## Standard Folder

```text
workspace/{business-slug}/{workflow-slug}/
|--- 01-work-map.md
|--- 02-system-blueprint.md
|--- 03-workflow-playbook.md
`--- live-system-records/
    |--- live-interface.md
    |--- feedback-scorecard.md
    |--- review-notes.md
    |--- approved-outputs.md
    `--- memory-updates.md
```

## 1. Work Map

Purpose: diagnosis.

Answers:

- What workflow matters?
- What is broken or slow today?
- Why should we build this first?
- What metric should improve?

## 2. System Blueprint

Purpose: architecture.

Defines:

- Workflow
- Context
- Memory Base
- Skills
- Interface
- Control
- Feedback

## 3. Workflow Playbook

Purpose: operating manual.

Defines:

- when to run the workflow
- what inputs are needed
- what the AI does
- what the human checks
- where outputs go
- how feedback is captured

## 4. Live System Records

Purpose: live links, evidence, and improvement history.

Stores:

- live tool links
- connected app locations
- approved outputs
- feedback scorecards
- review notes
- approved memory updates

## Clean Rule

```text
Blueprint defines the system.
Playbook explains how to run it.
Live System Records show what actually happened.
```

## When To Split Files

Keep the first system simple.

Only split extra files when something gets too large for the main package files.

Examples:

- `context-pack.md`
- `skill-card.md`
- `control-rules.md`

By default, those sections live inside `02-system-blueprint.md`.
