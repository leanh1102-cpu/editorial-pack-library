# SLTD Task Router

Map each request to a small route.

Base:

```text
boot_task -> source_preflight -> task_intake -> decision_safety
```

Routes:

```text
chapter status: chapter_readiness_check -> mindmap_review -> node_checkpoint
packet review: audit_story_arc -> mindmap_review -> editorial_director_review -> node_checkpoint
repair priority: editorial_director_review -> node_checkpoint
underreached scene: intensity_pass -> sltd_underreach_gate -> node_checkpoint
scene rewrite: sltd_editorial_hooks -> rewrite_scene -> multi_reviewer_pass -> node_checkpoint
line edit: sltd_canon_guard -> vietnamese_prose rules -> sltd_copyedit_proofread
node check: mindmap_review -> node_checkpoint
readiness: chapter_readiness_check -> sltd_publishing_readiness -> node_checkpoint
```

Gap output:

```text
SKILL GAP:
REQUEST TYPE:
MISSING ROUTE:
PROPOSED PATCH:
```
