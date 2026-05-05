# How It Works

Shipyard-OS has one job:

```text
Turn a repeated workflow into a useful AI-assisted Work System.
```

## The Method

```text
Map -> Build -> Run
```

## The Package

Each workflow gets one Work System Package:

```text
01-work-map.md
02-system-blueprint.md
03-workflow-playbook.md
live-system-records/
```

## The Six Parts

Every System Blueprint defines six parts:

```text
Workflow
Context
Skills
Interface
Control
Feedback
```

### Workflow

The work being improved, from trigger to output.

### Context

What the AI must know to do the work well.

This includes the Memory Base.

### Skills

Reusable AI SOPs that perform important parts of the workflow.

A skill can be a whole procedure, not just one tiny action.

### Interface

Where the system runs in practice.

Examples: Claude, ChatGPT, Gemini, ClickUp, Google Drive, Slack, CRM, Codex, Make, Zapier, n8n.

### Control

Ownership, review rules, approvals, restrictions, and escalation.

### Feedback

How usage teaches the system what to improve.

## Memory

Memory is simple:

```text
Business-wide memory lives in your-business/business-context/memory-base.md.
Workflow-specific memory lives in that workflow's System Blueprint.
Feedback proposes updates.
The owner approves updates.
live-system-records/memory-updates.md records the history.
```

So feedback is the process. Memory is the stored learning.

## Business Context And LLM Wiki

Approved business context sits above all Work Systems:

```text
01-workspace/your-business/business-context/
```

Use it for stable company context, voice, offers, audience, and business-level memory.

Each Work System can still have workflow-specific context inside its `02-system-blueprint.md`.

The AI-maintained notebook lives next to it:

```text
01-workspace/your-business/llm-wiki/
```

Use the wiki for processing sources, synthesizing notes, and tracking unresolved questions:

```text
index.md = what exists and where to look
source-log.md = what sources were processed
open-questions.md = what still needs answers
```

Promote only approved stable learnings from `llm-wiki/` into `business-context/`.

Brand files belong in `brand-assets/`. Workflow evidence belongs in `live-system-records/`.

## Decisions

Business-wide decisions live here:

```text
01-workspace/your-business/decisions/decision-log.md
```

Workflow-specific review evidence stays in:

```text
01-workspace/your-business/{workflow-slug}/live-system-records/
```

## Connectors

Connectors are global because the business has one tool environment.

Record available tools here:

```text
03-connectors/connected-tools.md
```

Then each Work System decides which connected tools it actually uses.

## User-Created Skills

User-created skills are reusable across Work Systems.

Store them here:

```text
02-skills/user-created/
```

If a workflow needs a new reusable skill, use:

```text
02-skills/skill-creator/
```

## Skill Systems

Skills should be modular, but real business workflows need sequences.

In Shipyard:

```text
Skills = reusable components
Work System Package = skill system
Workflow Playbook = orchestration layer
```

Use `03-workflow-playbook.md` to define the Skill Chain:

```text
Skill order
Input to each skill
Output from each skill
How outputs hand off
Human checkpoints
Final destination
```
