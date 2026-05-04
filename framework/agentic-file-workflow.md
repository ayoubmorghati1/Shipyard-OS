# Agentic File Workflow

Shipyard-OS skills are designed to be Level 2 agentic workflows.

That means the agent does more than explain the framework. It should interview, reason, produce the deliverable, and save it into the package structure.

---

## Standard Package Path

```text
clients/{client-slug}/{workflow-slug}/
```

Each skill writes its own phase file into that package folder.

The full package eventually looks like this after the method has run:

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
-> interviews, scores, creates/updates:
   clients/{client-slug}/{workflow-slug}/01-work-map.md

/build-system
-> reads 01-work-map.md, creates/updates:
   clients/{client-slug}/{workflow-slug}/02-system-blueprint.md

/run-review
-> reads prior files, creates/updates:
   clients/{client-slug}/{workflow-slug}/03-workflow-playbook.md
   clients/{client-slug}/{workflow-slug}/live-system-records/feedback-scorecard.md
   clients/{client-slug}/{workflow-slug}/live-system-records/review-notes.md
```

Important:

```text
/map-workflow does not create the Blueprint.
/build-system does not create the Playbook.
/run-review creates the Playbook and records what happens when the system runs.
```

---

## Work System Package Template

The reusable package template lives at:

```text
templates/work-system-package.md
```

That file explains the final deliverable container:

```text
1. Work Map
2. System Blueprint
3. Workflow Playbook
4. Live System & Records
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
