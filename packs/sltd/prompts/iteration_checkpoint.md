# SLTD Iteration Checkpoint

Use this prompt when a task needs controlled continuation across one or more editorial nodes.

This prompt does not authorize autonomous background work. It only structures the next loop inside the current user request.

## Read first

```text
packs/sltd/manifest.yml
packs/sltd/ENTRY_FAST_PATH.md
packs/sltd/rules/sltd_runtime_loop.md
packs/sltd/rules/sltd_source_preflight.md
packs/sltd/rules/sltd_task_router.md
packs/sltd/rules/sltd_decision_safety.md
packs/sltd/rules/sltd_agentic_iteration_loop.md
packs/sltd/ROLE_ENTRY_INDEX.md if a role is named
packs/sltd/rules/sltd_role_boundary_contracts.md if roles overlap
packs/sltd/rules/sltd_evidence_discipline.md
user request
```

## Output

```text
ITERATION CHECKPOINT
MISSION:
- request:
- scope:
- source layer:
- active role:
- output type:
- write permission:

ANALYZE:
- source read:
- blocker:
- role boundary:
- evidence need:

PLAN:
- route:
- batch size:
- patch strategy:
- verification gate:
- stop condition:

EXECUTE:
- action taken:
- action not taken:

EVALUATE:
- gate used:
- pass/fail:
- unread risk:

ADJUST:
- patch candidate:
- role handoff:
- source request:

NEXT NODE / STOP:
- next node:
- stop reason:
- user confirmation needed:
```

## Rules

- Use the smallest route that fits the task.
- Do not continue without source, scope, and role clarity.
- Do not run another role silently.
- Do not write back unless the user explicitly asked for write action.
- Do not treat a successful patch as publication readiness.
- Do not loop indefinitely; end with next node or stop.
