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
The Memory Base lives in the System Blueprint.
Feedback proposes updates.
The owner approves updates.
live-system-records/memory-updates.md records the history.
```

So feedback is the process. Memory is the stored learning.

## Connectors

Connectors are global because the business has one tool environment.

Record available tools here:

```text
connectors/connected-tools.md
```

Then each Work System decides which connected tools it actually uses.

## User-Created Skills

User-created skills are reusable across Work Systems.

Store them here:

```text
skills/user-created/
```

If a workflow needs a new reusable skill, use:

```text
skills/skill-creator/
```
