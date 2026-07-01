# SLTD Entry Fast Path

Use this file to avoid reading the whole pack for every task.

## Always read

```text
packs/sltd/manifest.yml
packs/sltd/DESIGN.md
packs/sltd/PACK.md
packs/sltd/AGENT_IDENTITY.md
packs/sltd/prompts/boot_task.md
packs/sltd/rules/sltd_runtime_loop.md
packs/sltd/rules/sltd_source_preflight.md
packs/sltd/rules/sltd_decision_safety.md
```

## Fast paths

### Living world & community motion check

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_living_world_community_motion_gate.md
rules/sltd_story_momentum.md
rules/sltd_underreach_gate.md
rules/sltd_canon_guard.md if repair depends on geography, custom, social structure, or history
rules/sltd_anti_ai_composite_failure_gate.md if world repair becomes synthetic
rules/sltd_role_boundary_contracts.md
packs/sltd/AUTHOR_TASTE_EXAMPLES.md
prompts/living_world_community_motion_check.md
prompts/node_checkpoint.md
```

### Character distinctiveness & iceberg check

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_character_distinctiveness_iceberg_gate.md
rules/sltd_character_agency_anti_ooc_gate.md if plot is forcing behavior
rules/sltd_canon_guard.md if profile depends on canon or relation history
samples/dialogue_voice_calibration.md if voice collapse appears
prompts/character_distinctiveness_check.md
prompts/node_checkpoint.md
```

### First-pass / scene rewrite

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_first_pass_editorial_workflow.md
rules/sltd_living_world_community_motion_gate.md if setting/community/world motion is in scope
rules/sltd_character_distinctiveness_iceberg_gate.md if character distinctiveness is in scope
rules/sltd_webnovel_paragraphing_layout_rhythm_gate.md if paragraphing/layout is in scope
rules/sltd_vietnamese_register_viet_dao_gate.md if register is in scope
rules/sltd_scene_first_prose_judgment_gate.md
rules/sltd_anti_ai_composite_failure_gate.md if synthetic risk appears
rules/sltd_character_agency_anti_ooc_gate.md if agency risk appears
rules/sltd_dynamic_range_cadence_gate.md if cadence risk appears
prompts/first_pass_editorial_workflow.md or prompts/rewrite_scene.md
prompts/node_checkpoint.md
```

### Chapter / packet / arc review

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_chapter_assembly_split_control_gate.md if chapter length or reader unit is in scope
rules/sltd_living_world_community_motion_gate.md if world/community motion or social texture is in scope
rules/sltd_character_distinctiveness_iceberg_gate.md if cast texture or continuity is in scope
rules/sltd_webnovel_paragraphing_layout_rhythm_gate.md if layout affects reader experience
rules/sltd_vietnamese_register_viet_dao_gate.md if register affects reader texture
rules/sltd_anti_ai_composite_failure_gate.md if synthetic risk appears
prompts/context_brief.md
prompts/audit_story_arc.md or prompts/webnovel_packet_benchmark.md
prompts/node_checkpoint.md
prompts/result_report.md
```

### Line surgery

```text
prompts/task_intake.md
ROLE_ENTRY_INDEX.md
roles/line_surgery.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_living_world_community_motion_gate.md if setting/community detail is the issue
rules/sltd_character_distinctiveness_iceberg_gate.md if voice/body/object signature is the issue
rules/sltd_webnovel_paragraphing_layout_rhythm_gate.md if line breaks are the issue
rules/sltd_vietnamese_register_viet_dao_gate.md if register is the issue
rules/sltd_vietnamese_line_surgery.md
prompts/source_surface_check.md if exact excerpt is not confirmed
prompts/line_surgery_pass.md
prompts/node_checkpoint.md
```

### Entry healthcheck

```text
rules/sltd_pack_healthcheck.md
rules/sltd_living_world_community_motion_gate.md
rules/sltd_character_distinctiveness_iceberg_gate.md
rules/sltd_webnovel_paragraphing_layout_rhythm_gate.md
rules/sltd_vietnamese_register_viet_dao_gate.md
rules/sltd_chapter_assembly_split_control_gate.md
rules/sltd_first_pass_editorial_workflow.md
rules/sltd_scene_first_prose_judgment_gate.md
rules/sltd_anti_ai_composite_failure_gate.md
rules/sltd_character_agency_anti_ooc_gate.md
rules/sltd_dynamic_range_cadence_gate.md
prompts/entry_healthcheck.md
```

## Rule

If exact prose, current lock, readiness, rewrite, line edit, line surgery, copyedit, or proofread is requested and source surface is not exact, run `source_surface_check.md` first.

If setting, community, custom, social habit, environment pushback, offscreen motion, or butterfly trace is in scope, run `living_world_community_motion_check.md`.

If characters feel skimmed, interchangeable, function-only, same-voiced, or lacking hidden life, run `character_distinctiveness_check.md`.

If scene edits are being assembled into a chapter, or chapter length/reader unit may be overloaded, run `chapter_assembly_split_check.md`.

If prose is too Chinese-translated, too Hán Việt-heavy, too modern-flat, or missing Viet Dao balance, run `vietnamese_register_check.md`.

If paragraphing, line breaks, short-line density, wall-text risk, or mobile readability affects reader breath, run `webnovel_paragraphing_layout_check.md`.

If prose work starts to satisfy gates before reading the scene as lived Vietnamese prose, run `scene_first_prose_judgment.md`.

If a scene or chapter has many correct-looking passes but still reads arranged, synthetic, or over-polished, run `anti_ai_composite_check.md`.
