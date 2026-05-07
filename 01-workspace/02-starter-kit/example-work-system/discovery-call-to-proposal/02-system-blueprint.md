# System Blueprint - Discovery Call To Proposal

## Business Goal

Increase proposal speed and quality after qualified discovery calls.

## Priority Workflow

Discovery call to proposal.

## Desired Outcome

Every qualified discovery call produces a reviewed proposal and follow-up email within 24 hours.

## 1. Workflow

```text
Trigger: qualified discovery call ends
Inputs: transcript, notes, offer details, pricing logic, proposal examples
Steps: summarize call -> extract needs -> match offer -> draft proposal -> draft follow-up -> human review -> send and log
Output: proposal draft and follow-up email
Destination: proposal doc, CRM, email thread
Success metric: proposal sent within 24 hours
```

## 2. Context

```text
Business facts: service business selling AI Work System implementation
Audience or customer: founders and teams with repeated operational workflows
Offer or service: audit, workshop, done-for-you build, optimization
Voice and tone: clear, direct, practical, premium but not inflated
Rules and constraints: do not invent prices, timelines, guarantees, or legal terms
Examples of good work: approved proposal examples
Source documents: offer doc, pricing notes, case studies
```

### Memory Base

```text
Stable facts: current offers, approved positioning, standard scope boundaries
Approved decisions: proposal must be reviewed before sending
Repeated preferences: concise executive summary first
Common corrections: remove vague AI hype, make business outcome explicit
Approved examples: final proposals that closed or got strong client feedback
```

## 3. Skills

```text
Skill name: Sales Call Analysis
Purpose: summarize the call and extract business needs, urgency, objections, and next steps
Inputs: transcript or notes
Procedure: identify business goal, pain, current workflow, buying signals, objections, decision process
Output: structured call brief
Review points: confirm facts and commercial details
Reusable across other Work Systems? yes
```

```text
Skill name: Proposal Drafting
Purpose: turn call brief into a first-pass proposal
Inputs: call brief, offer document, pricing notes, proposal example
Procedure: map problem to scope, write outcomes, define phases, flag missing info
Output: proposal draft
Review points: pricing, promises, scope, legal language
Reusable across other Work Systems? yes
```

### Skill System

```text
Orchestrator: Discovery Call To Proposal Playbook
Skills in chain: Sales Call Analysis -> Proposal Drafting -> Follow-Up Drafting
Reusable skills: Sales Call Analysis, Proposal Drafting, Follow-Up Drafting
Workflow-specific skills: none for v1
Skills to create: Follow-Up Drafting if it does not already exist
```

| Step | Skill | Input | Output | Hands off to | Human checkpoint |
| --- | --- | --- | --- | --- | --- |
| 1 | Sales Call Analysis | Transcript or notes | Call brief | Proposal Drafting | Check facts, needs, objections |
| 2 | Proposal Drafting | Call brief, offer doc, pricing notes | Proposal draft | Follow-Up Drafting | Check scope, price, promises |
| 3 | Follow-Up Drafting | Proposal draft and call brief | Follow-up email draft | Human send | Check tone and CTA |

## 4. Interface

```text
Primary interface: chosen by user
Why this interface: must sit close to transcripts, docs, CRM, and email
Input method: paste transcript or connect meeting notes
Output destination: proposal doc and email draft
Connected tools used: meeting notes, docs, CRM, email
Live links recorded in: live-system-records/live-interface.md
```

## 5. Control

```text
Owner: sales owner or founder
Approved uses: summarize calls, draft proposals, draft follow-up emails
Restricted uses: final pricing decisions, legal commitments, sending without approval
Human review required before: sending proposal or follow-up
Escalation path: founder reviews uncertain scope or pricing
```

## 6. Feedback

```text
What gets reviewed: proposal quality, edits required, turnaround time, close feedback
What gets logged: missing context, repeated edits, winning phrasing, client objections
Where feedback is recorded: live-system-records/feedback-scorecard.md
Who approves memory updates: system owner
Who updates the system: system owner or Shipyard
Review rhythm: weekly for first month, monthly after stable
```

## First Build Scope

One transcript in, proposal draft and follow-up email out.

## Setup Checklist

- [x] Work Map completed
- [x] Context gathered
- [x] Memory Base drafted
- [x] Skills defined
- [x] Interface selected
- [x] Controls defined
- [x] Feedback process defined
- [x] Live System Records folder ready
