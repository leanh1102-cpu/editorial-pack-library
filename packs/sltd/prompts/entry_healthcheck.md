# SLTD Entry Healthcheck

Use after a pack release or before adding a new skill.

Read:

```text
manifest.yml
DESIGN.md
ENTRY_FAST_PATH.md
ROLE_ENTRY_INDEX.md
EDITORIAL_COMPETENCY_MAP.md
rules/sltd_pack_healthcheck.md
rules/sltd_evidence_discipline.md
rules/sltd_role_boundary_contracts.md
rules/sltd_agentic_iteration_loop.md
rules/sltd_calibration_discipline.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_first_pass_editorial_workflow.md
rules/sltd_scene_first_prose_judgment_gate.md
rules/sltd_anti_ai_composite_failure_gate.md
rules/sltd_character_agency_anti_ooc_gate.md
rules/sltd_dynamic_range_cadence_gate.md
rules/sltd_handoff_continuity_protocol.md
rules/sltd_task_router.md
prompts/source_surface_check.md
prompts/first_pass_editorial_workflow.md
prompts/scene_first_prose_judgment.md
prompts/anti_ai_composite_check.md
prompts/character_agency_check.md
prompts/dynamic_range_check.md
prompts/iteration_checkpoint.md
prompts/session_handoff.md
samples/router_examples.md
CHANGELOG.md
```

Spot-check required role cards listed in `ROLE_ENTRY_INDEX.md`.

Spot-check required calibration files:

```text
samples/line_surgery_calibration.md
samples/dialogue_voice_calibration.md
samples/underreach_calibration.md
samples/readiness_false_positive.md
```

Output:

```text
ENTRY HEALTHCHECK
PACK VERSION:
STATUS:
MANIFEST CHECK:
ENTRY CHECK:
SOURCE FIDELITY CHECK:
FIRST-PASS EDITORIAL WORKFLOW CHECK:
SCENE-FIRST PROSE JUDGMENT CHECK:
ANTI-AI COMPOSITE CHECK:
CHARACTER AGENCY CHECK:
DYNAMIC RANGE CHECK:
HANDOFF CONTINUITY CHECK:
ROLE ENTRY CHECK:
ITERATION LOOP CHECK:
CALIBRATION CHECK:
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
