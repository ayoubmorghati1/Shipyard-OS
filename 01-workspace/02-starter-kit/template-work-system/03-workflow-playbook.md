# Workflow Playbook

Use this during **Run**.

Purpose: show the team how to operate the workflow every time.

## Workflow Name

## Purpose

Why this workflow exists.

## When To Use

What event triggers this playbook?

## Owner

Who owns the system?

## Trigger

What starts the workflow?

## Inputs

What must be provided?

## Steps

What happens each time?

```text
1.
2.
3.
4.
5.
```

## AI Role

What the AI does.

## Skills Used

Which reusable skills are used in this workflow?

## Skill Chain

How do skill outputs hand off into the next skill?

| Step | Skill | Input | Output | Next step | Human checkpoint |
| --- | --- | --- | --- | --- | --- |
| 1 |  |  |  |  |  |

Rules:

```text
Each skill gets only the context it needs.
Each output should be clean enough to feed the next step.
Human checkpoints should happen before risky or irreversible actions.
```

## Human Role

What the human does.

## Review Points

What must be checked before the output is used?

## Output

What gets produced?

## Destination

Where does the output go?

## Quality Checklist

- [ ] Accurate
- [ ] Complete
- [ ] Clear
- [ ] On-brand
- [ ] Safe to use
- [ ] Reviewed by the right person

## Success Metric

How will we know this is working?

## Review Rhythm

How often is the system reviewed?

## Feedback Behavior

```text
After each run:
Where approved outputs are saved:
Where issues are logged:
When review happens:
Who approves memory/system updates:
```

Important rule:

```text
Feedback does not automatically change the system.
Feedback proposes changes.
The owner approves changes.
Approved changes update Context, Memory, Skills, Control, or the Playbook.
```
