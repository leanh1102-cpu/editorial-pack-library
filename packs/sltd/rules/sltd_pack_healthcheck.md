# SLTD Pack Healthcheck

Use this rule to check the health of the SLTD pack after version changes.

This is a manual agent check. It does not create scripts, workflow files, issues, boards, or reports.

## Check manifest

Verify manifest version, required files, allowed tasks, source priority, and fail-closed status.

## Check source fidelity

Verify source fidelity rule and source surface prompt exist, are listed in manifest, and line-level routes require exact source surface before patching.

## Check living world and community motion

Verify:

- `rules/sltd_living_world_community_motion_gate.md` exists and is listed in manifest;
- `prompts/living_world_community_motion_check.md` exists and is listed in manifest;
- living_world_community_motion_check is listed in allowed_tasks;
- living-world route ends with node checkpoint;
- living-world route references source fidelity before patching;
- the gate checks location, world layer, community activity, custom/habit/taboo, offscreen motion, butterfly trace, environment pushback, social consequence, world iceberg trace, and setting-as-backdrop risk;
- the gate prevents setting-as-backdrop, world-pauses-for-POV, custom-as-decoration, scenery-as-mood-label, and lore replacing world life;
- the gate does not authorize new canon, large worldbuilding, geography changes, or social-history invention.

## Check routes

Verify each allowed task has a route or prompt, node-changing routes end with node checkpoint or result report, and routes reference their required gate files:

```text
source-surface routes -> sltd_source_fidelity_anti_compression.md
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
