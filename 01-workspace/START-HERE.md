# Start Here

This workspace is where you build your AI-assisted Work Systems.

Do this first:

1. Fill `00-intake.md`.
2. Fill `your-business/AGENTS.md` with the business-level agent brief.
3. Pick one repeated workflow that matters.
4. Copy `_template-work-system/` into `your-business/{workflow-slug}/`.
5. Run the three Shipyard skills in order:

```text
01-map-workflow
02-build-system
03-run-review
```

Your finished package will live here:

```text
01-workspace/your-business/{workflow-slug}/
```

Your business-level agent brief lives here:

```text
01-workspace/your-business/AGENTS.md
```

## What The Agent Should Produce

The agent should not only explain the framework. It should interview you, reason through the workflow, and write the package files.

```text
01-map-workflow      -> 01-work-map.md
02-build-system     -> 02-system-blueprint.md
03-run-review       -> 03-workflow-playbook.md + live-system-records/
```

## Where Live Apps Fit

Your actual workflow may run in Claude, ChatGPT, Gemini, ClickUp, Google Drive, Slack, a CRM, or another tool.

Record those links in:

```text
live-system-records/live-interface.md
```

The repo stays the operating structure. The live apps do the live work.
