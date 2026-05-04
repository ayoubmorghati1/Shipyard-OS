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
System Blueprint
```

---

## When To Use

Use when the user says things like:

- build the Work System
- create the System Blueprint
- define context and skills
- choose the interface
- set controls
- turn this Work Map into a system

---

## Inputs

Read available context from:

- `templates/system-blueprint.md`
- `templates/context-pack.md`
- `templates/skill-card.md`
- `templates/control-rules.md`
- `framework/shipyard-work-system.md`
- the relevant Work Map

If no Work Map exists, run `/map-workflow` first or ask for the workflow diagnosis.

---

## Level 2 File Behavior

This skill should not only answer in chat. It should create or update the Work System Package files whenever filesystem access is available.

Use this standard path:

```text
clients/{client-slug}/{workflow-slug}/02-system-blueprint.md
```

Read the Work Map from:

```text
clients/{client-slug}/{workflow-slug}/01-work-map.md
```

If the user is building Shipyard's own system, use:

```text
clients/shipyard/{workflow-slug}/02-system-blueprint.md
```

If the package folder does not exist, create it and ask for or reconstruct the Work Map first.

The System Blueprint should define:

```text
Workflow
Context
Skills
Interface
Control
Feedback
```

If Context Pack, Skill Cards, or Control Rules become too large for the Blueprint, create optional supporting files under:

```text
clients/{client-slug}/{workflow-slug}/supporting-assets/
```

Do not create supporting files by default. Keep the first package simple unless complexity justifies splitting.

After writing, tell the user the file path.

---

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

- company facts
- offers
- audience
- tone
- rules
- examples
- source docs

### Skills

Define reusable AI SOPs inside the workflow.

Examples:

- Sales Call Analysis Skill
- Proposal Drafting Skill
- Meeting Summary Skill
- Follow-Up Drafting Skill

### Interface

Where does the system live?

Examples:

- Claude Project
- Custom GPT
- Gemini
- Copilot
- ClickUp
- Notion
- Google Drive
- CRM
- Slack
- Make/Zapier/n8n
- Codex repo/folder

### Control

What can AI do, and what must humans approve?

### Feedback

How will the system improve?

---

## Output Format

Produce:

```markdown
# System Blueprint — {Workflow Name}

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

### Skill 2

## 4. Interface

Recommended interface:
Why:
Input method:
Output destination:

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

---

## Quality Standard

A good System Blueprint:

- maps directly to the Work Map
- defines all six parts
- does not overbuild
- chooses the interface based on existing work habits
- names human review points clearly
- includes a feedback loop
