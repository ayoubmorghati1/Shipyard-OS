# Shipyard-OS

Shipyard-OS is a cloneable workspace for building AI-assisted Work Systems.

It helps a business owner or team turn one repeated workflow into a practical AI operating layer: mapped, built, run, reviewed, and improved.

It is platform-agnostic. The live system can run through Claude, ChatGPT, Gemini, Copilot, Codex, ClickUp, Google Drive, Slack, a CRM, Make, Zapier, n8n, or a custom app. The repo is the planning and operating structure around the work.

## Start Here

Open:

```text
01-workspace/START-HERE.md
```

Then use:

```text
01-workspace/00-intake.md
01-workspace/_template-work-system/
02-skills/shipyard-skills/
```

## The Simple Model

```text
Map -> Build -> Run
```

| Phase | What happens | Main file created |
| --- | --- | --- |
| Map | Diagnose the workflow and choose what to improve first | `01-work-map.md` |
| Build | Design the AI-assisted Work System | `02-system-blueprint.md` |
| Run | Operate, review, and improve the workflow | `03-workflow-playbook.md` + records |

## The Work System Package

Every workflow gets one package:

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

Clean rule:

```text
Work Map = why this workflow matters
System Blueprint = what system should exist
Workflow Playbook = how to run it
Live System Records = what actually happened
```

## Repository Map

```text
Shipyard-OS/
|--- README.md
|--- AGENTS.md
|--- 01-workspace/
|   |--- START-HERE.md
|   |--- 00-intake.md
|   |--- HOW-IT-WORKS.md
|   |--- WORK-SYSTEM-PACKAGE.md
|   |--- _template-work-system/
|   |--- _example-work-system/
|   `--- your-business/
|       |--- AGENTS.md
|       |--- business-context/
|       |--- brand-assets/
|       |--- decisions/
|       `--- {workflow-slug}/
|--- 02-skills/
|   |--- shipyard-skills/
|   |--- skill-creator/
|   `--- user-created/
|--- 03-connectors/
|--- 04-adapters/
`--- .gitignore
```

## Where Outputs Go

Everything the agent builds for a business goes under:

```text
01-workspace/{business-slug}/{workflow-slug}/
```

The living business-level agent brief goes one level above the workflows:

```text
01-workspace/{business-slug}/AGENTS.md
```

Business-wide context, assets, and decisions live beside it:

```text
01-workspace/{business-slug}/business-context/
01-workspace/{business-slug}/brand-assets/
01-workspace/{business-slug}/decisions/
```

The connector apps may hold the live work, for example a Google Doc, ClickUp list, CRM record, Slack workflow, or Claude Project. The repo still records where those things live in:

```text
live-system-records/live-interface.md
```

## The Skills

Official Shipyard skills live here:

```text
02-skills/shipyard-skills/
|--- 01-map-workflow/
|--- 02-build-system/
`--- 03-run-review/
```

User-created reusable skills live here:

```text
02-skills/user-created/
```

Use `02-skills/skill-creator/` when you want the agent to turn a repeated task into a reusable skill.

## Completion Standard

A Work System is complete when:

- the workflow is clear from trigger to output
- the AI has the context and memory it needs
- the skills are reusable AI SOPs
- the interface fits the team's existing work habits
- human review and ownership are explicit
- feedback updates the system over time
- a new team member can run it without Shipyard in the room
