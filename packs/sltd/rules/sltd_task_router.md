# SLTD Task Router

Map each request to a small route.

Base:

```text
boot_task -> source_preflight -> task_intake -> decision_safety
```

Routes:

```text
handoff continuity: sltd_handoff_continuity_protocol -> session_handoff -> node_checkpoint
session handoff: sltd_handoff_continuity_protocol -> session_handoff -> node_checkpoint
source surface check: sltd_source_fidelity_anti_compression -> source_surface_check -> node_checkpoint
calibration case: sltd_calibration_discipline -> relevant calibration sample -> node_checkpoint
agentic iteration: sltd_agentic_iteration_loop -> iteration_checkpoint -> node_checkpoint
iteration checkpoint: sltd_agentic_iteration_loop -> iteration_checkpoint -> node_checkpoint
role entry: ROLE_ENTRY_INDEX -> roles/<requested_role>.md -> sltd_role_boundary_contracts -> node_checkpoint
chapter status: source_surface_check if current source unclear -> chapter_readiness_check -> mindmap_review -> node_checkpoint
packet review: sltd_source_fidelity_anti_compression -> context_brief -> audit_story_arc -> mindmap_review -> editorial_director_review -> node_checkpoint
repair priority: editorial_director -> editorial_director_review -> node_checkpoint
underreached scene: source_surface_check if exact scene missing -> intensity_editor -> intensity_pass -> sltd_underreach_gate -> node_checkpoint
scene rewrite: source_surface_check -> canon_guard -> sltd_editorial_hooks -> rewrite_scene -> multi_reviewer_pass -> node_checkpoint
line edit: source_surface_check -> vietnamese_line_editor -> sltd_canon_guard -> vietnamese_prose rules -> sltd_copyedit_proofread
line surgery: source_surface_check -> line_surgery -> sltd_vietnamese_line_surgery -> line_surgery_pass -> node_checkpoint
copyedit: source_surface_check -> copyeditor -> sltd_copyedit_proofread -> node_checkpoint
proofread: source_surface_check -> proofreader -> sltd_copyedit_proofread -> node_checkpoint
webnovel benchmark: sltd_source_fidelity_anti_compression -> sltd_webnovel_momentum_benchmark -> webnovel_packet_benchmark -> node_checkpoint -> result_report
review mode: sltd_review_modes -> review_mode_pass -> node_checkpoint
role boundary check: ROLE_ENTRY_INDEX -> sltd_role_boundary_contracts -> node_checkpoint
node check: mindmap_review -> node_checkpoint
readiness: source_surface_check -> publishing_readiness_reviewer -> chapter_readiness_check -> sltd_publishing_readiness -> node_checkpoint
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

Calibration rule:

```text
If the user rejects an output or asks to learn from an error, return a calibration candidate.
Do not write calibration cases unless the user explicitly requests a write action.
Use existing calibration files before proposing new files.
```

Source fidelity rule:

```text
If the task requires exact prose, exact status, exact patch, or current lock, verify source surface first.
Do not line edit, line surgery, copyedit, proofread, rewrite, or patch from digest, summary, or chat memory.
If source surface is missing, downgrade to map/packet risk scan or request exact source.
```

Handoff rule:

```text
If context is degrading, task state must move to another AI, or the user asks for handoff, run handoff continuity.
Handoff is navigation and task state, not source truth.
The next AI must verify current source before verdict and continue only at NEXT NODE.
```

Gap output:

```text
SKILL GAP:
REQUEST TYPE:
MISSING ROUTE:
PROPOSED PATCH:
```
