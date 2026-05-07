# LLM Wiki

Use this folder as the AI-maintained notebook for the business.

This is where the agent turns scattered information into organized markdown pages, tracks what has been processed, and keeps open questions visible.

## Difference From Business Context

```text
llm-wiki = working notebook and synthesis layer
business-context = approved business context the system can rely on
brand-assets = brand and marketing assets
decisions = business-wide decisions
live-system-records = evidence from one workflow
```

The wiki can be messy while it is being developed.

`business-context/` should be cleaner, more stable, and approved.

## Core Files

```text
index.md = what exists and where to look
source-log.md = what got processed
open-questions.md = what is still unclear
```

## Workflow

When new information appears:

1. Record the source in `source-log.md`.
2. Create or update relevant wiki notes.
3. Update `index.md`.
4. Add unresolved gaps to `open-questions.md`.
5. Promote only approved learnings into `business-context/`.

## Rule

Do not centralize all raw material here.

The wiki records and organizes knowledge from wherever source material naturally lives: brand assets, workflow records, Google Drive, ClickUp, CRM, Slack, calls, meetings, or other tools.
