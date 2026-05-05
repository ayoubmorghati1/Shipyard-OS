---
name: build-system
description: Use when turning a Work Map into a System Blueprint, defining the six-part Work System, or preparing the build setup for an AI-assisted workflow.
---

# Build System

Use this skill during the **Build** phase.

Purpose:

> Define the AI-assisted Work System to build.

Output:

```text
01-workspace/{business-slug}/{workflow-slug}/02-system-blueprint.md
```

## When To Use

Use when the user says things like:

- build the Work System
- create the System Blueprint
- define context and memory
- define skills
- choose the interface
- set controls
- turn this Work Map into a system

## Inputs

Read available context from:

- `01-workspace/{business-slug}/{workflow-slug}/01-work-map.md`
- `01-workspace/{business-slug}/AGENTS.md` if it exists
- `01-workspace/{business-slug}/business-context/` if it exists
- `01-workspace/{business-slug}/business-context/index.md` if it exists
- `01-workspace/{business-slug}/business-context/open-questions.md` if it exists
- `01-workspace/{business-slug}/brand-assets/` index or relevant source material if needed
- `01-workspace/{business-slug}/decisions/decision-log.md` if it exists
- `01-workspace/_template-work-system/02-system-blueprint.md`
- `01-workspace/HOW-IT-WORKS.md`
- `03-connectors/connected-tools.md`
- any relevant files already inside the package folder

If no Work Map exists, run `01-map-workflow` first or ask for the workflow diagnosis.

## Level 2 File Behavior

Do not only answer in chat. Read the Work Map, interview for missing details, and write the System Blueprint.

Read:

```text
01-workspace/{business-slug}/{workflow-slug}/01-work-map.md
```

Write:

```text
01-workspace/{business-slug}/{workflow-slug}/02-system-blueprint.md
```

Make sure this folder exists:

```text
01-workspace/{business-slug}/{workflow-slug}/live-system-records/
```

If the user is building their own system and no business name is given, use:

```text
01-workspace/your-business/{workflow-slug}/
```

After writing, tell the user the file path.

## Build The Six Parts

Define:

```text
Workflow
Context
Skills
Interface
Control
Feedback
```

### Workflow

What work is being improved from trigger to outcome?

### Context

What does the AI need to know?

Include the Memory Base:

- stable company facts from `business-context/`
- offers
- audience
- tone
- rules
- examples
- source docs
- repeated preferences
- approved decisions

Business-wide memory should live in:

```text
01-workspace/{business-slug}/business-context/memory-base.md
```

Workflow-specific memory should stay inside this workflow's `02-system-blueprint.md`.

### Skills

Define reusable AI SOPs inside the workflow.

Skills can be whole procedures.

Examples:

- Sales Call Analysis Skill
- Proposal Drafting Skill
- Meeting Summary Skill
- Follow-Up Drafting Skill

If a skill should be reusable across multiple Work Systems, note that it should be created under:

```text
02-skills/user-created/
```

Also define the Skill System:

- which skill orchestrates or coordinates the workflow
- which reusable skills are used
- which workflow-specific skills are needed
- what each skill takes as input
- what each skill produces as output
- how outputs hand off between skills
- where human checkpoints happen

Do not create one giant skill for the whole workflow if smaller reusable skills can be chained cleanly.

### Interface

Where does the system live?

Examples:

- Claude
- ChatGPT
- Gemini
- Copilot
- ClickUp
- Google Drive
- CRM
- Slack
- Make/Zapier/n8n
- Codex repo/folder

The chosen interface should be recorded later in:

```text
live-system-records/live-interface.md
```

### Control

What can AI do, and what must humans approve?

### Feedback

How will the system improve?

Feedback proposes changes. The owner approves changes. Approved changes update Context, Memory, Skills, Control, or the Playbook.

## Output Format

Produce:

```markdown
# System Blueprint - {Workflow Name}

## Business Goal

## Priority Workflow

## Desired Outcome

## 1. Workflow

## 2. Context

### Memory Base

## 3. Skills

### Skill 1

Purpose:
Inputs:
Procedure:
Output:
Review points:
Reusable across other Work Systems? yes/no

## 3.1 Skill System

Orchestrator:
Skills in chain:
Reusable skills:
Workflow-specific skills:
Skills to create:

| Step | Skill | Input | Output | Hands off to | Human checkpoint |
| --- | --- | --- | --- | --- | --- |

## 4. Interface

Primary interface:
Why:
Input method:
Output destination:
Connected tools used:
Live links recorded in:

## 5. Control

Owner:
Approved uses:
Restricted uses:
Human review required:
Escalation:

## 6. Feedback

Metric:
Review rhythm:
What gets logged:
What can be updated:
Who approves updates:

## First Build Scope

## Setup Checklist
```

## Quality Standard

A good System Blueprint:

- maps directly to the Work Map
- defines all six parts
- keeps Context, Memory, Skills, Interface, Control, and Feedback in one place
- defines the Skill System when multiple skills need to chain together
- does not overbuild
- chooses the interface based on existing work habits
- names human review points clearly
- includes a feedback loop
