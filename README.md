# Shipyard-OS

A platform-agnostic starter kit for turning repeated business workflows into AI-assisted Work Systems.

Shipyard-OS is not another generic agent framework. It is a business implementation workspace: map the work, build the system, run it, review it, and improve it.

It can work with Claude, ChatGPT, Gemini, Copilot, Codex, ClickUp, Google Drive, Slack, CRMs, Make, Zapier, n8n, or custom apps.

---

## The Litmus Test

> A business can point to one repeated workflow and say: this now runs faster, with clearer ownership, better context, safer review, and a visible improvement loop.

If a folder, template, skill, or record does not help that happen, it should not be there.

---

## What This Kit Is For

| Use case | What Shipyard-OS gives you |
| --- | --- |
| Workshops | A repeatable structure participants can clone and fill while learning |
| Client delivery | A clean package for mapping, building, handing off, and reviewing systems |
| Internal ops | A workspace for your own business workflows and AI operating layer |
| Skill systems | A way to chain focused reusable skills into end-to-end workflows |
| Business memory | A clean split between approved context, AI notes, decisions, and live records |

---

## The Method

```text
Map -> Build -> Run
```

| Phase | Question | Output |
| --- | --- | --- |
| Map | What workflow is worth improving first? | `01-work-map.md` |
| Build | What system should support this workflow? | `02-system-blueprint.md` |
| Run | How does the team operate and improve it? | `03-workflow-playbook.md` + records |

---

## The Work System Anatomy

Every Work System defines six parts.

| Part | Meaning |
| --- | --- |
| Workflow | The business process from trigger to output |
| Context | What the AI must know to do useful work |
| Skills | Reusable AI SOPs used inside the workflow |
| Interface | Where the system actually runs |
| Control | Ownership, review, approvals, and risk boundaries |
| Feedback | How outputs and usage improve the system over time |

---

## What Ships

| Area | Folder | Purpose |
| --- | --- | --- |
| Workspace | `01-workspace/` | Where the business setup and Work System Packages live |
| Skills | `02-skills/` | Official Shipyard skills plus user-created reusable skills |
| Connectors | `03-connectors/` | Global registry of tools, apps, and data sources |
| Adapters | `04-adapters/` | Optional notes for specific platforms |

---

## Quick Start

1. Clone the repo.
2. Open `01-workspace/START-HERE.md`.
3. Fill `01-workspace/00-intake.md`.
4. Fill or draft `01-workspace/01-your-business/AGENTS.md`.
5. Copy `01-workspace/02-starter-kit/template-work-system/` into `01-workspace/01-your-business/{workflow-slug}/`.
6. Run the Shipyard skills in order:

```text
01-map-workflow
02-build-system
03-run-review
```

---

## Repo Layout

```text
Shipyard-OS/
|-- README.md
|-- AGENTS.md
|-- 01-workspace/
|   |-- START-HERE.md
|   |-- 00-intake.md
|   |-- 01-your-business/
|   |   |-- AGENTS.md
|   |   |-- business-context/
|   |   |-- llm-wiki/
|   |   |-- brand-assets/
|   |   |-- decisions/
|   |   `-- {workflow-slug}/
|   `-- 02-starter-kit/
|       |-- template-work-system/
|       `-- example-work-system/
|-- 02-skills/
|   |-- shipyard-skills/
|   |-- skill-creator/
|   `-- user-created/
|-- 03-connectors/
`-- 04-adapters/
```

---

## No Duplicate Templates

There is one blank package and one filled example.

| Folder | What it is | When to use |
| --- | --- | --- |
| `02-starter-kit/template-work-system/` | Blank Work System Package | Copy this when starting a new workflow |
| `02-starter-kit/example-work-system/` | Filled reference example | Read this to understand what good looks like |
| `01-your-business/{workflow-slug}/` | Your real Work System Package | This is where actual work goes |

The template and example look similar because they show the same package structure. They are not two places to work.

---

## Work System Package

Every real workflow becomes:

```text
01-workspace/01-your-business/{workflow-slug}/
|-- 01-work-map.md
|-- 02-system-blueprint.md
|-- 03-workflow-playbook.md
`-- live-system-records/
    |-- live-interface.md
    |-- feedback-scorecard.md
    |-- review-notes.md
    |-- approved-outputs.md
    `-- memory-updates.md
```

| File | Purpose |
| --- | --- |
| `01-work-map.md` | Why this workflow matters and what is broken today |
| `02-system-blueprint.md` | The system design: context, skills, interface, control, feedback |
| `03-workflow-playbook.md` | How the workflow runs every time, including the Skill Chain |
| `live-system-records/` | Links, outputs, feedback, reviews, and memory updates from real usage |

---

## Business-Level Memory

| Folder | Purpose |
| --- | --- |
| `business-context/` | Approved business context the system can rely on |
| `llm-wiki/` | AI-maintained notebook for processed sources and open questions |
| `brand-assets/` | Brand and marketing assets only |
| `decisions/` | Business-wide decisions and why they were made |

Clean rule:

```text
llm-wiki processes information.
business-context stores approved knowledge.
live-system-records stores workflow evidence.
decisions stores business-wide choices.
```

---

## Skills And Skill Systems

| Layer | Folder/file | Meaning |
| --- | --- | --- |
| Official method skills | `02-skills/shipyard-skills/` | Map, Build, Run |
| User-created skills | `02-skills/user-created/` | Reusable AI SOPs created for the business |
| Skill creator | `02-skills/skill-creator/` | Helps create new reusable skills |
| Skill System | `03-workflow-playbook.md` | Chains skills into an end-to-end workflow |

The rule:

```text
Do not build one giant skill.
Do not use skills as isolated one-off prompts.
Build focused reusable skills and chain them inside a Work System.
```

---

## Completion Standard

A Work System is complete when:

- the workflow is clear from trigger to output
- the AI has the context and memory it needs
- the skills are reusable AI SOPs
- the skill chain is documented
- the interface fits the team's existing work habits
- human review and ownership are explicit
- feedback updates the system over time
- a new team member can run it without Shipyard in the room
