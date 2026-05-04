# Agentic File Workflow

Shipyard-OS skills are designed to be Level 2 agentic workflows.

That means the agent does more than explain the framework. It should interview, reason, produce the deliverable, and save it into the package structure.

---

## Standard Package Path

```text
clients/{client-slug}/{workflow-slug}/
```

Example:

```text
clients/acme-agency/discovery-call-to-proposal/
├── 01-work-map.md
├── 02-system-blueprint.md
├── 03-workflow-playbook.md
└── live-system-records/
    ├── feedback-scorecard.md
    └── review-notes.md
```

For Shipyard's own internal workflows:

```text
clients/shipyard/{workflow-slug}/
```

---

## Skill Mapping

```text
/map-workflow
-> interviews, scores, creates/updates 01-work-map.md

/build-system
-> reads 01-work-map.md, creates/updates 02-system-blueprint.md

/run-review
-> reads prior files, creates/updates 03-workflow-playbook.md and live-system-records/
```

---

## Generality

This structure works for:

- Shipyard internal workflows
- workshop participants
- private clients
- corporate teams
- any business using the repo as a starter kit

The names change. The structure stays the same.

---

## Slug Rules

Use slugs for folder names:

- lowercase
- hyphens instead of spaces
- remove punctuation
- short and readable

Examples:

```text
Acme Agency -> acme-agency
Discovery Call to Proposal -> discovery-call-to-proposal
Weekly Leadership Brief -> weekly-leadership-brief
```

