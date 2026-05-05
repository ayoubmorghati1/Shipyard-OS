# Your Business

This is where your real Work System Packages go.

Start by filling:

```text
01-workspace/your-business/AGENTS.md
```

That file is the business-level living agent brief.

Then fill or let the agent draft:

```text
01-workspace/your-business/business-context/
```

Use:

```text
01-workspace/your-business/llm-wiki/
```

as the AI-maintained notebook for processed sources, synthesis, and open questions.

Use:

```text
01-workspace/your-business/brand-assets/
```

for raw source material like decks, logos, case studies, voice samples, and examples.

Use:

```text
01-workspace/your-business/decisions/decision-log.md
```

for business-wide decisions.

Copy:

```text
01-workspace/_template-work-system/
```

Into:

```text
01-workspace/your-business/{workflow-slug}/
```

Example:

```text
01-workspace/your-business/discovery-call-to-proposal/
```

If you want to organize by business function, use folders like:

```text
01-workspace/your-business/
|--- growth/
|--- delivery/
|--- knowledge/
|--- leadership/
|--- marketing/
`--- operations/
```

Then place workflow packages inside the relevant function.

## Folder Meaning

```text
AGENTS.md = how the agent should work with this business
business-context = approved business context
llm-wiki = AI-maintained notebook and synthesis layer
brand-assets = brand and marketing assets
decisions = business-wide decisions
{workflow-slug} = one Work System Package
```

## LLM Wiki

Use these files to keep the AI-maintained notebook navigable:

```text
llm-wiki/index.md
llm-wiki/source-log.md
llm-wiki/open-questions.md
```

The agent should update them when source material is processed or context gaps appear.

Stable approved learnings should then be promoted into `business-context/`.
