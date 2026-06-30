# SLTD Task Intake

Use this prompt right after boot and source preflight.

## Read first

1. `prompts/boot_task.md`
2. `rules/sltd_source_preflight.md`
3. `rules/sltd_task_router.md`
4. `rules/sltd_decision_safety.md`
5. user request

## Classify

```text
REQUEST TYPE:
SCOPE:
SOURCE NEEDED:
CURRENT SOURCE LAYER:
OUTPUT TYPE:
SKILL ROUTE:
STOP CONDITIONS:
```

## Request types

```text
chapter_status
packet_review
repair_priority
underreach_fix
scene_rewrite
line_edit
mindmap_review
readiness_review
skill_gap
```

## Rule

If request type, source, or scope is unclear, return STOP with the missing item.
