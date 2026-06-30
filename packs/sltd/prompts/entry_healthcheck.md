# SLTD Entry Healthcheck

Use after a pack release or before adding a new skill.

Read:

```text
manifest.yml
ENTRY_FAST_PATH.md
rules/sltd_pack_healthcheck.md
rules/sltd_evidence_discipline.md
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
