# SLTD Task Router

Map each request to a small route.

Base:

```text
boot_task -> source_preflight -> task_intake -> decision_safety
```

Routes:

```text
chapter assembly split check: sltd_source_fidelity_anti_compression -> sltd_chapter_assembly_split_control_gate -> chapter_assembly_split_check -> node_checkpoint
first-pass editorial workflow: sltd_source_fidelity_anti_compression -> sltd_first_pass_editorial_workflow -> first_pass_editorial_workflow -> node_checkpoint
scene-first prose judgment: sltd_source_fidelity_anti_compression -> sltd_scene_first_prose_judgment_gate -> scene_first_prose_judgment -> node_checkpoint
anti-AI composite check: sltd_source_fidelity_anti_compression -> sltd_scene_first_prose_judgment_gate if checklist-first risk appears -> sltd_anti_ai_composite_failure_gate -> anti_ai_composite_check -> node_checkpoint
character agency check: sltd_source_fidelity_anti_compression -> sltd_character_agency_anti_ooc_gate -> character_agency_check -> node_checkpoint
dynamic range check: sltd_source_fidelity_anti_compression -> sltd_dynamic_range_cadence_gate -> dynamic_range_check -> node_checkpoint
handoff continuity: sltd_handoff_continuity_protocol -> session_handoff -> node_checkpoint
session handoff: sltd_handoff_continuity_protocol -> session_handoff -> node_checkpoint
source surface check: sltd_source_fidelity_anti_compression -> source_surface_check -> node_checkpoint
calibration case: sltd_calibration_discipline -> relevant calibration sample -> node_checkpoint
agentic iteration: sltd_agentic_iteration_loop -> iteration_checkpoint -> node_checkpoint
iteration checkpoint: sltd_agentic_iteration_loop -> iteration_checkpoint -> node_checkpoint
role entry: ROLE_ENTRY_INDEX -> roles/<requested_role>.md -> sltd_role_boundary_contracts -> node_checkpoint
chapter status: source_surface_check if current source unclear -> chapter_assembly_split_check if chapter length/reader unit is in scope -> chapter_readiness_check -> mindmap_review -> node_checkpoint
packet review: sltd_source_fidelity_anti_compression -> chapter_assembly_split_check if chapter split risk appears -> first_pass_editorial_workflow if first edit is requested -> scene_first_prose_judgment if checklist-first risk appears -> anti_ai_composite_check if synthetic/checklist risk appears -> character_agency_check if agency risk appears -> context_brief -> audit_story_arc -> mindmap_review -> editorial_director_review -> node_checkpoint
repair priority: editorial_director -> editorial_director_review -> node_checkpoint
underreached scene: source_surface_check if exact scene missing -> first_pass_editorial_workflow for initial repair -> scene_first_prose_judgment if prose feels like checklist compliance -> anti_ai_composite_check if scene is correct but synthetic -> character_agency_check if plot forces behavior -> dynamic_range_check if clean but not sharp -> intensity_editor -> intensity_pass -> sltd_underreach_gate -> node_checkpoint
scene rewrite: source_surface_check -> first_pass_editorial_workflow -> scene_first_prose_judgment if checklist-first risk appears -> anti_ai_composite_check if multiple-pass AI risk appears -> character_agency_check if OOC/OCC risk appears -> dynamic_range_check if restraint/cadence risk appears -> canon_guard -> sltd_editorial_hooks -> rewrite_scene -> multi_reviewer_pass -> node_checkpoint
chapter assembly after scene edits: source_surface_check -> chapter_assembly_split_check -> anti_ai_composite_check if assembled chapter reads synthetic -> publishing_readiness_reviewer if split affects readiness -> node_checkpoint
line edit: source_surface_check -> first_pass_editorial_workflow if first serious edit -> scene_first_prose_judgment if prose reads like rule performance -> anti_ai_composite_check if repair collage risk appears -> character_agency_check if dialogue/action serves plot too neatly -> dynamic_range_check if cadence flattened -> vietnamese_line_editor -> sltd_canon_guard -> vietnamese_prose rules -> sltd_copyedit_proofread
line surgery: source_surface_check -> first_pass_editorial_workflow if first serious edit -> scene_first_prose_judgment if prose reads like rule performance -> anti_ai_composite_check if repair collage risk appears -> character_agency_check if dialogue/action serves plot too neatly -> dynamic_range_check if cadence flattened -> line_surgery -> sltd_vietnamese_line_surgery -> line_surgery_pass -> node_checkpoint
copyedit: source_surface_check -> copyeditor -> sltd_copyedit_proofread -> node_checkpoint
proofread: source_surface_check -> proofreader -> sltd_copyedit_proofread -> node_checkpoint
webnovel benchmark: sltd_source_fidelity_anti_compression -> sltd_chapter_assembly_split_control_gate if chapter-level benchmark is in scope -> sltd_first_pass_editorial_workflow if assessing first-pass quality -> sltd_scene_first_prose_judgment_gate -> sltd_anti_ai_composite_failure_gate -> sltd_character_agency_anti_ooc_gate -> sltd_dynamic_range_cadence_gate -> sltd_webnovel_momentum_benchmark -> webnovel_packet_benchmark -> node_checkpoint -> result_report
review mode: sltd_review_modes -> review_mode_pass -> node_checkpoint
role boundary check: ROLE_ENTRY_INDEX -> sltd_role_boundary_contracts -> node_checkpoint
node check: mindmap_review -> node_checkpoint
readiness: source_surface_check -> chapter_assembly_split_check if length/split affects readiness -> scene_first_prose_judgment if prose readiness is being inferred from checklist compliance -> anti_ai_composite_check if false readiness risk appears -> publishing_readiness_reviewer -> chapter_readiness_check -> sltd_publishing_readiness -> node_checkpoint
```

Role boundary rule:

```text
If multiple roles are active, run role boundary check before execution.
If a later role finds an earlier-layer blocker, stop and hand back.
If a user names a role directly, read the role entry card before running the task-specific route.
```

Chapter assembly rule:

```text
If scene edits are being assembled into a chapter, or chapter length/reader unit may be overloaded, run chapter assembly split check.
Scene is the edit unit. Chapter is the reader unit. Packet is the continuity and momentum unit.
Do not split mechanically by word count alone.
Do not silently split or renumber live manuscript without explicit user permission.
```

First-pass rule:

```text
If beginning a first serious rewrite, line edit, line surgery, or scene repair, run first-pass editorial workflow before targeted gates.
Edit first as a human prose editor. Verify after.
Choose the earliest failing layer and one main edit strategy before writing.
Run only the targeted gate that matches the remaining blocker.
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

Scene-first rule:

```text
If prose work starts by satisfying gates instead of judging the scene as lived Vietnamese prose, run scene-first prose judgment.
Find one governing scene pressure before repair.
Use checklist as later verification, not as the writing method.
Do not add required-looking details to hide checklist-first prose.
```

Character agency rule:

```text
If a character seems to serve the plot, clue, scene card, or explanation instead of acting from pressure, run character agency check.
Do not treat a scene as ready when character want, fear, knowledge limit, pressure, choice, or visible cost is missing.
Do not add canon or change locked outcome to restore agency.
```

Anti-AI composite rule:

```text
If a scene or chapter has many correct-looking passes but still reads arranged, synthetic, over-polished, or assembled, run anti-AI composite check.
Do not add more texture to hide synthetic structure.
Choose one governing scene pressure before repair.
Do not claim readiness from green sub-passes alone.
```

Handoff rule:

```text
If context is degrading, task state must move to another AI, or the user asks for handoff, run handoff continuity.
Handoff is navigation and task state, not source truth.
The next AI must verify current source before verdict and continue only at NEXT NODE.
```

Dynamic range rule:

```text
If restraint, moderation, line edit, anti-melodrama, or subtlety causes a scene to become cleaner but flatter, run dynamic range check.
Preserve what must stay quiet, but restore pressure, cadence, turn, and aftershock when scene function requires it.
Do not add canon or change locked outcome to create force.
```

Gap output:

```text
SKILL GAP:
REQUEST TYPE:
MISSING ROUTE:
PROPOSED PATCH:
```
