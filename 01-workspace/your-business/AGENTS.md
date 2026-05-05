# Your Business Agent Brief

This is the living brief for the agent working with this business.

Use this for business-wide context. Put workflow-specific instructions inside each Work System Package.

## Business

Name:

What we do:

Who we serve:

Current priority:

## Operator Preferences

How I like to work:

How I like answers:

What to avoid:

Decision style:

## Voice

Internal tone:

External tone:

Words or phrases to use:

Words or phrases to avoid:

## Knowledge Base

Primary context folder:

```text
01-workspace/your-business/business-context/
```

For approved context, read `business-context/`.

For source processing history, synthesis, and open questions, read:

```text
01-workspace/your-business/llm-wiki/index.md
```

Stable facts:

Important offers:

Audience notes:

Positioning:

Useful source files:

## Global Memory

Primary memory file:

```text
01-workspace/your-business/business-context/memory-base.md
```

Approved decisions:

Repeated preferences:

Important corrections:

Things the agent should remember:

## Active Work Systems

| Work System | Folder | Owner | Status | Notes |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |

## Connected Tools

Use `03-connectors/connected-tools.md` as the global registry.

Tools this business actually uses:

| Tool | Purpose | Notes |
| --- | --- | --- |
|  |  |  |

## Brand Assets

Raw source material lives here:

```text
01-workspace/your-business/brand-assets/
```

Use it as reference material. Do not treat it as approved memory until it is summarized or approved into `business-context/`.

When source material is integrated, update:

```text
01-workspace/your-business/llm-wiki/source-log.md
```

When context is missing or contradictory, update:

```text
01-workspace/your-business/llm-wiki/open-questions.md
```

## Decisions

Business-wide decisions live here:

```text
01-workspace/your-business/decisions/decision-log.md
```

When I make a meaningful business-wide decision, suggest logging it.

## How The Agent Should Work With Me

- Be direct and practical.
- Ask for missing context only when it blocks useful work.
- When a workflow repeats, suggest turning it into a Work System.
- When a reusable process appears, suggest creating a skill in `02-skills/user-created/`.
- When feedback reveals a stable learning, propose a memory update.
- Do not update memory, context, skills, or control rules without approval.
- Keep workflow-specific evidence inside that workflow's `live-system-records/`.
- When a workflow uses multiple skills, document the Skill Chain in its `03-workflow-playbook.md`.

## Update Log

| Date | What changed | Why |
| --- | --- | --- |
|  |  |  |
