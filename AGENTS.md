# Shipyard-OS Agent Instructions

You are working inside Shipyard-OS.

Your job is to help a business owner map, build, run, and improve AI-assisted Work Systems. Stay business-led and platform-agnostic. Do not make the system about one AI tool unless that tool has been chosen as the live interface.

## Core Method

```text
Map -> Build -> Run
```

## Core Package

Each workflow should become one Work System Package:

```text
01-workspace/{business-slug}/{workflow-slug}/
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

## Core Documents

```text
Work Map = diagnosis
System Blueprint = architecture
Workflow Playbook = operating manual
Live System Records = links, outputs, feedback, and memory updates
```

## Six-Part Work System

Every System Blueprint must define:

```text
Workflow
Context
Skills
Interface
Control
Feedback
```

Memory lives in the system as follows:

```text
Context contains the Memory Base.
Feedback proposes and approves updates to the Memory Base.
live-system-records/memory-updates.md records what changed and why.
```

## Operating Rules

- Start with the workflow, not the AI tool.
- Map many opportunities, but build one first.
- Keep the first version simple enough to run this week.
- Define Skills as reusable AI SOPs, not tiny generic actions.
- Add connectors only when they directly support a workflow.
- Keep live app links in `live-system-records/live-interface.md`.
- Keep approved outputs in `live-system-records/approved-outputs.md`.
- Keep review evidence in `live-system-records/feedback-scorecard.md` and `review-notes.md`.
- Never update memory, context, skills, or control rules from one bad output without human approval.

## Skill Locations

Official Shipyard method skills:

```text
02-skills/shipyard-skills/
```

Reusable skills created by the user:

```text
02-skills/user-created/
```

Platform adapter notes:

```text
04-adapters/
```

Global tool and data connections:

```text
03-connectors/connected-tools.md
```

## Business-Level Agent Briefs

Each business can have its own living agent brief:

```text
01-workspace/{business-slug}/AGENTS.md
```

Use it for business-wide context:

- who the business is
- what matters now
- how the operator likes to work
- voice and communication preferences
- global memory and decisions
- active Work Systems
- connected tools

Do not put workflow-specific operating instructions here. Put those inside the relevant Work System Package.

Business-level support folders:

```text
01-workspace/{business-slug}/business-context/
01-workspace/{business-slug}/brand-assets/
01-workspace/{business-slug}/decisions/
```

Use `business-context/` for interpreted context, `brand-assets/` for raw source material, and `decisions/` for business-wide decisions. Use workflow-level `live-system-records/` for what happened inside one Work System.

Maintain business context like a small wiki:

```text
business-context/index.md = navigation and page map
business-context/source-log.md = source integration history
business-context/open-questions.md = unresolved context gaps
```

When source material changes the business context, update the relevant page, source log, and index. If something is unclear, add it to open questions.

## Skill Systems

Skills are reusable components. A Work System Package can orchestrate multiple skills into one end-to-end business workflow.

Use this rule:

```text
02-skills/user-created/ = reusable skill library
02-system-blueprint.md = skills selected or needed
03-workflow-playbook.md = skill chain and handoffs
```

Avoid mega skills. Avoid isolated skills that leave the human manually copying output from one step into the next. Prefer focused reusable skills wired together by the Workflow Playbook.
