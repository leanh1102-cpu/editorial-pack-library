# SLTD Entry Healthcheck

Use after a pack release or before adding a new skill.

Read:

```text
manifest.yml
DESIGN.md
ENTRY_FAST_PATH.md
EDITORIAL_COMPETENCY_MAP.md
rules/sltd_pack_healthcheck.md
rules/sltd_evidence_discipline.md
rules/sltd_role_boundary_contracts.md
rules/sltd_task_router.md
samples/router_examples.md
CHANGELOG.md
```

Output:

```text
ENTRY HEALTHCHECK
PACK VERSION:
STATUS:
MANIFEST CHECK:
ENTRY CHECK:
ROUTE CHECK:
ROLE BOUNDARY CHECK:
EVIDENCE CHECK:
ORPHAN RISK:
SMOKE TEST RESULT:
FIX NEEDED:
```

Labels:

```text
PACK_HEALTH_OK
PACK_HEALTH_WARN
PACK_HEALTH_FAIL
```

If health fails, patch the entry before adding new skills.
