# SLTD Pack Healthcheck

Use this rule to check the health of the SLTD pack after version changes.

This is a manual agent check. It does not create scripts, workflow files, issues, boards, or reports.

## Check manifest

Verify manifest version, required files, allowed tasks, source priority, and fail-closed status.

## Check source fidelity

Verify source fidelity rule and source surface prompt exist, are listed in manifest, and line-level routes require exact source surface before patching.

## Check protagonist advancement and growth route calibration

Verify:

- `rules/sltd_protagonist_advancement_growth_route_gate.md` exists and is listed in manifest;
- `prompts/protagonist_advancement_check.md` exists and is listed in manifest;
- `samples/protagonist_advancement_calibration.md` exists and is listed in manifest;
- protagonist_advancement_check is listed in allowed_tasks;
- protagonist advancement route ends with node checkpoint;
- protagonist advancement route references source fidelity before patching;
- the gate defines gain target, gain type, cost, knowledge limit, forbidden gain, and growth route;
- the gate requires object, body, relation, witness or social trace, cost, knowledge limit, and aftershock;
- the gate blocks Notion-label prose, lore-label gains, too-adult reasoning, too-clean upgrades, early system knowledge, and object-as-function-tag prose;
- the gate treats C030 low-layer lore as valid when it becomes world-rule sensitivity, not system knowledge;
- the gate does not authorize new source-unsupported growth.

## Check entry route governance and gate budget

Verify:

- `rules/sltd_entry_route_governance_gate_budget_protocol.md` exists and is listed in manifest;
- `prompts/entry_route_governance_check.md` exists and is listed in manifest;
- entry_route_governance_check is listed in allowed_tasks;
- entry governance route ends with node checkpoint;
- the protocol defines primary route, secondary gate, gate budget, stop condition, gate cascade, and checklist-first repair;
- the protocol requires one primary route before secondary gates;
- secondary gates require evidence, not adjacency;
- stop conditions are explicit;
- gate cascade and checklist-first repair are blocked;
- the protocol does not authorize skipping source preflight, source surface, canon guard, evidence, or user-requested modes.

## Check routes

Verify each allowed task has a route or prompt, node-changing routes end with node checkpoint or result report, and routes reference their required gate files:

```text
source-surface routes -> sltd_source_fidelity_anti_compression.md
entry governance routes -> sltd_entry_route_governance_gate_budget_protocol.md
protagonist advancement routes -> sltd_protagonist_advancement_growth_route_gate.md
transition/skiptime/event-cluster routes -> sltd_scene_transition_skiptime_event_cluster_gate.md
timeline POV routes -> sltd_timeline_pov_foreshadowing_folklore_gate.md
prose craft routes -> sltd_prose_craft_style_material_gate.md
scene composition routes -> sltd_scene_composition_component_balance_gate.md
narrative beat routes -> sltd_narrative_beat_escalation_aftershock_gate.md
living world routes -> sltd_living_world_community_motion_gate.md
first-pass routes -> sltd_first_pass_editorial_workflow.md
chapter assembly routes -> sltd_chapter_assembly_split_control_gate.md
Vietnamese register routes -> sltd_vietnamese_register_viet_dao_gate.md
webnovel paragraphing routes -> sltd_webnovel_paragraphing_layout_rhythm_gate.md
character distinctiveness routes -> sltd_character_distinctiveness_iceberg_gate.md
scene-first routes -> sltd_scene_first_prose_judgment_gate.md
anti-AI composite routes -> sltd_anti_ai_composite_failure_gate.md
character agency routes -> sltd_character_agency_anti_ooc_gate.md
dynamic range routes -> sltd_dynamic_range_cadence_gate.md
```

## Check role boundaries

Verify later roles do not overwrite earlier-layer blockers and learned taste/calibration/gates/workflows do not override current source, canon, evidence, or human lock.

## Check orphan risk

Mark a file as possible orphan when it exists but is not listed in manifest, is listed but cannot be fetched, defines a task with no route, duplicates another rule without reason, or is missing from its route.

## Output labels

```text
PACK_HEALTH_OK
PACK_HEALTH_WARN
PACK_HEALTH_FAIL
```
