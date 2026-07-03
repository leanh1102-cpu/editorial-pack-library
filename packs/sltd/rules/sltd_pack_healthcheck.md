# SLTD Pack Healthcheck

Use this rule to check the health of the SLTD pack after version changes.

This is a manual agent check. It does not create scripts, workflow files, issues, boards, or reports.

## Check manifest

Verify manifest version, required files, allowed tasks, source priority, and fail-closed status.

## Check source fidelity

Verify source fidelity rule and source surface prompt exist, are listed in manifest, and line-level routes require exact source surface before patching.

## Check structural spine, outline pre-prose, and borderbound

Verify:

- `rules/sltd_structural_spine_outline_preprose_borderbound_gate.md` exists and is listed in manifest;
- `prompts/structural_spine_outline_preprose_check.md` exists and is listed in manifest;
- `samples/structural_spine_outline_preprose_calibration.md` exists and is listed in manifest;
- structural_spine_outline_preprose_check is listed in allowed_tasks;
- structural spine route ends with node checkpoint;
- rewrite, line surgery, readiness, and chapter/packet/arc routes reference structural spine when prose permission or borderbound is at stake;
- the gate defines structural spine, outline preflight, borderbound, Chapter Card lock, Scene Packet lock, prose permission, and outline repair required;
- the gate blocks prose before outline, incomplete chapter cards, incomplete scene packets, missing borderbound, thin detailed outline, missing chapter/scene question, unclear changed state, and unsupported gain/lore/residue slots;
- the gate does not authorize new source-unsupported outline, canon, scene, chapter purpose, lore, or payoff.

## Check supernatural event residue and dread amplitude

Verify supernatural residue rule/prompt/sample, allowed task, source fidelity route, node checkpoint, and blockers for mood-only fog/cold/silence, underpowered dread, folklore without incident, generic beast threat, relic decoration, and early deep-lore reveal.

## Check protagonist inquiry and clue-chain pressure

Verify protagonist inquiry rule/prompt/sample, allowed task, source fidelity route, node checkpoint, and blockers for passive protagonist, missing inner reasoning, broken clue chain, and adult system reasoning.

## Check protagonist advancement and growth route calibration

Verify protagonist advancement rule/prompt/sample, allowed task, source fidelity route, node checkpoint, gain target/type/cost/knowledge limit/forbidden gain, and blockers for Notion-label prose and source-unsupported growth.

## Check entry route governance and gate budget

Verify entry governance rule/prompt, allowed task, node checkpoint route, one primary route before secondary gates, evidence-backed secondary gates, explicit stop conditions, and no gate cascade.

## Check routes

Verify each allowed task has a route or prompt, node-changing routes end with node checkpoint or result report, and routes reference their required gate files:

```text
source-surface routes -> sltd_source_fidelity_anti_compression.md
entry governance routes -> sltd_entry_route_governance_gate_budget_protocol.md
structural spine routes -> sltd_structural_spine_outline_preprose_borderbound_gate.md
supernatural residue routes -> sltd_supernatural_event_residue_dread_amplitude_gate.md
protagonist inquiry routes -> sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md
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
