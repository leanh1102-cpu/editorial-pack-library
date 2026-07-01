# SLTD Pack Healthcheck

Use this rule to check the health of the SLTD pack after version changes.

This is a manual agent check. It does not create scripts, workflow files, issues, boards, or reports.

## Check manifest

Verify manifest version, required files, allowed tasks, source priority, and fail-closed status.

## Check source fidelity

Verify source fidelity rule and source surface prompt exist, are listed in manifest, and line-level routes require exact source surface before patching.

## Check scene composition and component balance

Verify:

- `rules/sltd_scene_composition_component_balance_gate.md` exists and is listed in manifest;
- `prompts/scene_composition_balance_check.md` exists and is listed in manifest;
- scene_composition_balance_check is listed in allowed_tasks;
- scene composition route ends with node checkpoint;
- scene composition route references source fidelity before patching;
- the gate checks dialogue, action/blocking, inner thought, setting/living world, object/clue, sensory/body, silence/pause, summary/transition, and aftershock;
- the gate uses soft diagnostic bands by scene function and blocks ratio-as-formula;
- the gate detects fake balance, overused/missing components, and dominant component mismatch;
- the gate does not authorize adding components only to satisfy percentages.

## Check routes

Verify each allowed task has a route or prompt, node-changing routes end with node checkpoint or result report, and routes reference their required gate files:

```text
source-surface routes -> sltd_source_fidelity_anti_compression.md
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
