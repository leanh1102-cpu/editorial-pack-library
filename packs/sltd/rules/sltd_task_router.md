# SLTD Task Router

Map each request to a small route.

Base:

```text
boot_task -> source_preflight -> task_intake -> decision_safety
```

Routes:

```text
agentic iteration: sltd_agentic_iteration_loop -> iteration_checkpoint -> node_checkpoint
iteration checkpoint: sltd_agentic_iteration_loop -> iteration_checkpoint -> node_checkpoint
role entry: ROLE_ENTRY_INDEX -> roles/<requested_role>.md -> sltd_role_boundary_contracts -> node_checkpoint
chapter status: chapter_readiness_check -> mindmap_review -> node_checkpoint
packet review: context_brief -> audit_story_arc -> mindmap_review -> editorial_director_review -> node_checkpoint
repair priority: editorial_director -> editorial_director_review -> node_checkpoint
underreached scene: intensity_editor -> intensity_pass -> sltd_underreach_gate -> node_checkpoint
scene rewrite: canon_guard -> sltd_editorial_hooks -> rewrite_scene -> multi_reviewer_pass -> node_checkpoint
line edit: vietnamese_line_editor -> sltd_canon_guard -> vietnamese_prose rules -> sltd_copyedit_proofread
line surgery: line_surgery -> sltd_vietnamese_line_surgery -> line_surgery_pass -> node_checkpoint
copyedit: copyeditor -> sltd_copyedit_proofread -> node_checkpoint
proofread: proofreader -> sltd_copyedit_proofread -> node_checkpoint
webnovel benchmark: sltd_webnovel_momentum_benchmark -> webnovel_packet_benchmark -> node_checkpoint -> result_report
review mode: sltd_review_modes -> review_mode_pass -> node_checkpoint
role boundary check: ROLE_ENTRY_INDEX -> sltd_role_boundary_contracts -> node_checkpoint
node check: mindmap_review -> node_checkpoint
readiness: publishing_readiness_reviewer -> chapter_readiness_check -> sltd_publishing_readiness -> node_checkpoint
```

Role boundary rule:

```text
If multiple roles are active, run role boundary check before execution.
If a later role finds an earlier-layer blocker, stop and hand back.
If a user names a role directly, read the role entry card before running the task-specific route.
```

Iteration rule:

```text
If the user asks to continue, loop, iterate, batch, patch, verify, or proceed node by node, run agentic iteration.
The loop must end with NEXT NODE or STOP.
The loop may not continue indefinitely without user permission.
```

Gap output:

```text
SKILL GAP:
REQUEST TYPE:
MISSING ROUTE:
PROPOSED PATCH:
```
