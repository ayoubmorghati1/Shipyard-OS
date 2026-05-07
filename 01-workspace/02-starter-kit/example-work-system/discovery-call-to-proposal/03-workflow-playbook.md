# Workflow Playbook - Discovery Call To Proposal

## Purpose

Turn a qualified discovery call into a proposal draft and follow-up email within 24 hours.

## When To Use

Use after every qualified discovery call.

## Owner

Sales owner or founder.

## Trigger

Discovery call ends and transcript or notes are available.

## Inputs

- Call transcript or notes
- Offer document
- Pricing notes
- Proposal example
- Brand voice notes

## Steps

```text
1. Save transcript or notes.
2. Run Sales Call Analysis.
3. Review the call brief for factual accuracy.
4. Run Proposal Drafting.
5. Draft follow-up email.
6. Human reviews scope, price, promises, and tone.
7. Send proposal and log the result.
```

## AI Role

Analyze the call, structure the opportunity, draft the proposal, and draft the follow-up email.

## Skills Used

- Sales Call Analysis
- Proposal Drafting
- Follow-Up Drafting

## Skill Chain

| Step | Skill | Input | Output | Next step | Human checkpoint |
| --- | --- | --- | --- | --- | --- |
| 1 | Sales Call Analysis | Transcript or notes | Call brief | Proposal Drafting | Confirm facts and missing details |
| 2 | Proposal Drafting | Call brief, offer document, pricing notes | Proposal draft | Follow-Up Drafting | Confirm scope, price, claims |
| 3 | Follow-Up Drafting | Proposal draft and call brief | Email draft | Human review and send | Confirm tone and CTA |

## Human Role

Review facts, commercial logic, scope, pricing, client promises, and final tone.

## Review Points

- Does the proposal reflect the call?
- Are scope and pricing accurate?
- Are promises safe?
- Is anything missing before sending?

## Output

Proposal draft and follow-up email draft.

## Destination

Proposal doc, CRM, and email thread.

## Quality Checklist

- [ ] Accurate
- [ ] Complete
- [ ] Clear
- [ ] On-brand
- [ ] Safe to send
- [ ] Reviewed by owner

## Success Metric

Proposal sent within 24 hours of qualified call.

## Review Rhythm

Weekly for the first month, monthly after stable.

## Feedback Behavior

```text
After each run: log proposal turnaround time and major edits
Where approved outputs are saved: live-system-records/approved-outputs.md
Where issues are logged: live-system-records/feedback-scorecard.md
When review happens: weekly during first month
Who approves memory/system updates: system owner
```
