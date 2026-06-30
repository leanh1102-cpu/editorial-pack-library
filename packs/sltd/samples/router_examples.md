# SLTD Router Examples

## Chapter status

Request:

```text
Check C030 blockers.
```

Route:

```text
boot_task -> source_preflight -> task_intake -> decision_safety -> chapter_readiness_check -> node_checkpoint -> result_report
```

## Packet review

Request:

```text
Check C001-C030 packet lock.
```

Route:

```text
boot_task -> source_preflight -> context_brief -> audit_story_arc -> mindmap_review -> publishing_readiness -> node_checkpoint -> result_report
```

## Scene work

Request:

```text
Work on one named scene from current Scene Bank.
```

Route:

```text
boot_task -> source_preflight -> task_intake -> editorial_hooks -> rewrite_scene -> multi_reviewer_pass -> node_checkpoint
```

## Underreach

Request:

```text
The scene is correct but too thin.
```

Route:

```text
boot_task -> task_intake -> intensity_pass -> underreach_gate -> node_checkpoint
```

## Missing source

Expected decision:

```text
STOP: EVIDENCE_MISSING
```
