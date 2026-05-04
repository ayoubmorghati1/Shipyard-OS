# Shipyard-OS

Shipyard-OS is a starter kit for building AI-assisted Work Systems.

It is designed for Shipyard's own business operations, workshops, and client delivery. It is platform-agnostic: the live interface can be Claude, ChatGPT, Gemini, Copilot, ClickUp, Notion, Google Drive, Slack, a CRM, Zapier, Make, n8n, Codex, or a custom app.

The core belief:

> AI becomes valuable when it improves real work.

The unit of value is the workflow.

---

## The Method

```text
Map -> Build -> Run
```

| Phase | Purpose | Core output |
| --- | --- | --- |
| Map | Diagnose the workflow and opportunity | Work Map |
| Build | Define the AI-assisted Work System | System Blueprint |
| Run | Install, operate, review, and improve | Workflow Playbook + Feedback Scorecard |

---

## The Six-Part Work System

Every Work System has six parts:

```text
Workflow
Context
Skills
Interface
Control
Feedback
```

Memory lives inside Context and Feedback:

```text
Context contains the Memory Base.
Feedback updates the Memory Base.
```

---

## What Ships In This Kit

```text
Shipyard-OS/
├── README.md
├── SHIPYARD.md
├── shipyard-intake.md
├── connections.md
├── framework/
├── templates/
├── work-systems/
├── clients/
├── decisions/
├── examples/
├── records/
├── references/
└── .claude/skills/
    ├── 01-map-workflow/
    ├── 02-build-system/
    └── 03-run-review/
```

Core skills:

```text
01 /map-workflow
02 /build-system
03 /run-review
```

These skills follow the method:

```text
01 /map-workflow -> Work Map
02 /build-system -> System Blueprint
03 /run-review   -> Workflow Playbook + Feedback Scorecard
```

---

## Quick Start

1. Fill `shipyard-intake.md`.
2. Run `/map-workflow` for one repeated workflow.
3. Run `/build-system` to define the six-part Work System.
4. Run `/run-review` to create the operating playbook and review rhythm.
5. Assemble the Work System Package using `templates/work-system-package.md`.

---

## Agentic File Workflow

The skills are designed to be Level 2 agentic workflows.

That means the agent should:

1. Interview the user when information is missing.
2. Read the relevant framework/templates.
3. Produce the right deliverable.
4. Save or update the deliverable in the correct package folder.

Standard package path:

```text
clients/{client-slug}/{workflow-slug}/
```

Example:

```text
clients/acme-agency/discovery-call-to-proposal/
├── 01-work-map.md
├── 02-system-blueprint.md
├── 03-workflow-playbook.md
└── live-system-records/
    ├── feedback-scorecard.md
    └── review-notes.md
```

Skill behavior:

```text
/map-workflow
-> interviews, scores, creates/updates 01-work-map.md

/build-system
-> reads 01-work-map.md, creates/updates 02-system-blueprint.md

/run-review
-> reads prior files, creates/updates 03-workflow-playbook.md and live-system-records/
```

For Shipyard's own internal workflows, use:

```text
clients/shipyard/{workflow-slug}/
```

---

## The Work System Package

The final handoff container is:

```text
Work System Package
1. Work Map
2. System Blueprint
3. Workflow Playbook
4. Live System & Records
```

Clean rule:

```text
Blueprint defines the system.
Playbook explains how to run it.
Live System & Records stores what actually happens.
```

---

## Completion Standard

A Work System is complete when:

- The workflow is clear from trigger to outcome.
- The AI has the right context and memory base.
- The required Skills are defined as reusable AI SOPs.
- The interface fits the team's existing work habits.
- Human control, review, and ownership are explicit.
- Feedback improves context, skills, rules, and examples over time.
- The team can run the workflow without Shipyard in the room.
