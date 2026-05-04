# Advanced Operating Patterns

These patterns are useful when a Work System becomes more advanced, technical, recurring, or multi-client.

They are not new framework components. They are implementation patterns inside the Shipyard Work System.

---

## Static Context

Maps to: Context / Memory Base.

Use for stable identity, brand, methodology, business knowledge, offers, ICP, and approved language.

Practical rule:

> Use AI to interview the client/founder and generate the first version of static context instead of asking them to write it from scratch.

---

## Dynamic Memory

Maps to: Feedback / Learning Memory.

Use for decisions, corrections, approved outputs, recurring preferences, and learnings.

Practical rule:

> Stable context goes in the Memory Base. New learnings enter through Feedback and are approved through Control before becoming memory.

---

## Modular Skills

Maps to: Skills.

Use when a workflow needs reusable AI SOPs.

Examples:

- Proposal Drafting Skill
- Sales Call Analysis Skill
- Meeting Summary Skill
- Client Follow-Up Skill
- Research Brief Skill
- Brand Voice Rewrite Skill

---

## Skill Systems / Pipelines

Maps to: Workflow.

Example:

```text
Transcript
-> Sales Call Analysis Skill
-> Offer Recommendation Skill
-> Proposal Drafting Skill
-> Human review
-> Follow-Up Drafting Skill
```

Practical rule:

> A workflow is the pipeline. Skills are the reusable AI SOPs inside the pipeline.

---

## Planning Levels

Maps to: Workflow Playbook / Control.

Simple work:

```text
Do the task -> check the output -> send/store it
```

Complex work:

```text
Plan -> Execute -> Verify -> Human approval -> Publish/store
```

Practical rule:

> The more risk, ambiguity, or client impact, the more explicit the planning and verification steps should be.

---

## Multi-Client Architecture

Maps to: Context / Control / Live System & Records.

Pattern:

```text
Shared Shipyard Methodology
+ Client-specific context
+ Client-specific memory
+ Client-specific outputs
+ Client-specific controls
```

Practical rule:

> Shared methodology can be reused. Client context, memory, outputs, and controls must stay separate.

---

## Predictable Output Structure

Maps to: Workflow Playbook / Live System & Records.

Practical rule:

> The Playbook defines where outputs go. Live System & Records stores or links what actually happened.

---

## Universal Access / Scheduled Workflows

Maps to: Interface.

Use only when the workflow needs to run from anywhere or on a schedule.

Examples:

- Slack/Telegram trigger
- Calendar-based workflow
- CRM-triggered follow-up
- Scheduled weekly leadership brief
- Server or automation tool running recurring tasks

Practical rule:

> Scheduled or always-on workflows are advanced interface choices, not default requirements.

