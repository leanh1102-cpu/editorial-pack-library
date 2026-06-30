# SLTD Task Router

Map each request to a small route.

Base:

```text
boot_task -> source_preflight -> task_intake -> decision_safety
```

Routes:

```text
chapter status: chapter_readiness_check -> mindmap_review -> node_checkpoint
packet review: context_brief -> audit_story_arc -> mindmap_review -> editorial_director_review -> node_checkpoint
repair priority: editorial_director_review -> node_checkpoint
underreached scene: intensity_pass -> sltd_underreach_gate -> node_checkpoint
scene rewrite: sltd_editorial_hooks -> rewrite_scene -> multi_reviewer_pass -> node_checkpoint
line edit: sltd_canon_guard -> vietnamese_prose rules -> sltd_copyedit_proofread
line surgery: sltd_vietnamese_line_surgery -> line_surgery_pass -> node_checkpoint
webnovel benchmark: sltd_webnovel_momentum_benchmark -> webnovel_packet_benchmark -> node_checkpoint -> result_report
review mode: sltd_review_modes -> review_mode_pass -> node_checkpoint
role boundary check: sltd_role_boundary_contracts -> node_checkpoint
node check: mindmap_review -> node_checkpoint
readiness: chapter_readiness_check -> sltd_publishing_readiness -> node_checkpoint
```

Role boundary rule:

```text
If multiple roles are active, run role boundary check before execution.
If a later role finds an earlier-layer blocker, stop and hand back.
```

Gap output:

```text
SKILL GAP:
REQUEST TYPE:
MISSING ROUTE:
PROPOSED PATCH:
```
