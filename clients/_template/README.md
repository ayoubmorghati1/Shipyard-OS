# Client Work System Package Template

Duplicate this folder for each client or internal Work System.

Recommended naming:

```text
clients/{client-name}/{work-system-name}/
```

Core package:

```text
01-work-map.md
02-system-blueprint.md
03-workflow-playbook.md
live-system-records/
```

The three method skills should write into this package:

```text
/map-workflow  -> 01-work-map.md
/build-system  -> 02-system-blueprint.md
/run-review    -> 03-workflow-playbook.md + live-system-records/
```

Keep the package simple by default. Split supporting assets into extra files only when the Blueprint or Playbook becomes too large.
