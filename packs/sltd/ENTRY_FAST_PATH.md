# SLTD Entry Fast Path

Use this file to avoid reading the whole pack for every task.

It does not replace `manifest.yml`, `PACK.md`, `DESIGN.md`, or `boot_task.md`. It only gives the smallest safe route.

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

### Character distinctiveness & iceberg check

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_character_distinctiveness_iceberg_gate.md
rules/sltd_character_agency_anti_ooc_gate.md if plot is forcing behavior
rules/sltd_canon_guard.md if profile depends on canon or relation history
samples/dialogue_voice_calibration.md if voice collapse appears
rules/sltd_role_boundary_contracts.md
packs/sltd/AUTHOR_TASTE_EXAMPLES.md
prompts/character_distinctiveness_check.md
prompts/node_checkpoint.md
```

### Character agency check

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_character_agency_anti_ooc_gate.md
rules/sltd_character_distinctiveness_iceberg_gate.md if character remains interchangeable after agency check
rules/sltd_canon_guard.md
rules/sltd_role_boundary_contracts.md
packs/sltd/AUTHOR_TASTE_EXAMPLES.md
prompts/character_agency_check.md
prompts/node_checkpoint.md
```

### Webnovel paragraphing & layout check

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_webnovel_paragraphing_layout_rhythm_gate.md
rules/sltd_dynamic_range_cadence_gate.md if short-line rhythm flattens cadence
rules/sltd_vietnamese_line_surgery.md if line rhythm is the blocker
rules/sltd_role_boundary_contracts.md
prompts/webnovel_paragraphing_layout_check.md
prompts/node_checkpoint.md
```

### Vietnamese register check

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_vietnamese_register_viet_dao_gate.md
rules/sltd_vietnamese_line_surgery.md
samples/viet_dao_prose_calibration.md
rules/sltd_role_boundary_contracts.md
packs/sltd/AUTHOR_TASTE_EXAMPLES.md
prompts/vietnamese_register_check.md
prompts/node_checkpoint.md
```

### Chapter assembly & split check

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_chapter_assembly_split_control_gate.md
rules/sltd_webnovel_paragraphing_layout_rhythm_gate.md if chapter surface flow or mobile fatigue is in scope
rules/sltd_first_pass_editorial_workflow.md if governing chapter pressure is unclear
rules/sltd_anti_ai_composite_failure_gate.md if assembled chapter reads synthetic
rules/sltd_role_boundary_contracts.md
prompts/chapter_assembly_split_check.md
prompts/node_checkpoint.md
```

### First-pass editorial workflow

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_first_pass_editorial_workflow.md
rules/sltd_character_distinctiveness_iceberg_gate.md if character profile target is unclear
rules/sltd_webnovel_paragraphing_layout_rhythm_gate.md if paragraphing/layout target is unclear
rules/sltd_vietnamese_register_viet_dao_gate.md if register target is unclear
rules/sltd_scene_first_prose_judgment_gate.md
rules/sltd_role_boundary_contracts.md
packs/sltd/AUTHOR_TASTE_EXAMPLES.md
prompts/first_pass_editorial_workflow.md
prompts/node_checkpoint.md
```

### Scene-first prose judgment

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_scene_first_prose_judgment_gate.md
rules/sltd_character_distinctiveness_iceberg_gate.md if characters read as scene functions
rules/sltd_webnovel_paragraphing_layout_rhythm_gate.md if layout performs emotion or breaks reader breath
rules/sltd_vietnamese_register_viet_dao_gate.md if Vietnamese register is miscalibrated
rules/sltd_anti_ai_composite_failure_gate.md if synthetic/checklist risk remains
rules/sltd_character_agency_anti_ooc_gate.md if character pressure is false
rules/sltd_dynamic_range_cadence_gate.md if cadence is flat
rules/sltd_role_boundary_contracts.md
packs/sltd/AUTHOR_TASTE_EXAMPLES.md
prompts/scene_first_prose_judgment.md
prompts/node_checkpoint.md
```

### Anti-AI composite check

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_scene_first_prose_judgment_gate.md if checklist-first risk appears
rules/sltd_character_distinctiveness_iceberg_gate.md if cast reads flat or interchangeable
rules/sltd_webnovel_paragraphing_layout_rhythm_gate.md if layout has AI signature
rules/sltd_vietnamese_register_viet_dao_gate.md if prose smells translated or flat
rules/sltd_character_agency_anti_ooc_gate.md
rules/sltd_dynamic_range_cadence_gate.md
rules/sltd_anti_ai_composite_failure_gate.md
rules/sltd_role_boundary_contracts.md
packs/sltd/AUTHOR_TASTE_EXAMPLES.md
prompts/anti_ai_composite_check.md
prompts/node_checkpoint.md
```

### Source surface check

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_source_preflight.md
rules/sltd_decision_safety.md
rules/sltd_evidence_discipline.md
rules/sltd_context_window_strategy.md
prompts/source_surface_check.md
prompts/node_checkpoint.md
```

### Scene rewrite

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_first_pass_editorial_workflow.md
rules/sltd_character_distinctiveness_iceberg_gate.md if character distinctiveness is in scope
rules/sltd_webnovel_paragraphing_layout_rhythm_gate.md if paragraphing/layout is in scope
rules/sltd_vietnamese_register_viet_dao_gate.md if Hán Việt / Viet Dao register is in scope
rules/sltd_scene_first_prose_judgment_gate.md
rules/sltd_anti_ai_composite_failure_gate.md if scene is synthetic after multiple passes
rules/sltd_character_agency_anti_ooc_gate.md
rules/sltd_dynamic_range_cadence_gate.md if restraint or cadence risk appears
rules/sltd_editorial_hooks.md
rules/sltd_canon_guard.md
rules/sltd_intensity_rules.md
prompts/rewrite_scene.md
prompts/multi_reviewer_pass.md
prompts/node_checkpoint.md
```

### Line surgery

```text
prompts/task_intake.md
ROLE_ENTRY_INDEX.md
roles/line_surgery.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_character_distinctiveness_iceberg_gate.md if voice/body/object signature is the issue
samples/dialogue_voice_calibration.md if cast voice collapse appears
rules/sltd_webnovel_paragraphing_layout_rhythm_gate.md if paragraphing/line breaks are the issue
rules/sltd_vietnamese_register_viet_dao_gate.md if register/Hán Việt balance is the issue
samples/viet_dao_prose_calibration.md if register patching is needed
rules/sltd_first_pass_editorial_workflow.md if this is the first serious edit
rules/sltd_scene_first_prose_judgment_gate.md if prose reads like rule performance
rules/sltd_anti_ai_composite_failure_gate.md if prior passes created repair collage
rules/sltd_character_agency_anti_ooc_gate.md if dialogue or action serves plot too neatly
rules/sltd_dynamic_range_cadence_gate.md if line edit has flattened cadence
rules/sltd_vietnamese_line_surgery.md
samples/line_surgery_calibration.md
core/vietnamese_prose/prose_rhythm.vi.md
core/vietnamese_prose/dialogue_voice.vi.md
core/vietnamese_prose/anti_ai_words.vi.md
packs/sltd/AUTHOR_TASTE_EXAMPLES.md
prompts/source_surface_check.md if exact excerpt is not confirmed
prompts/line_surgery_pass.md
prompts/node_checkpoint.md
```

### Chapter assembly after scene edits

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_chapter_assembly_split_control_gate.md
rules/sltd_character_distinctiveness_iceberg_gate.md if cast continuity or side-character function drifts between scenes
rules/sltd_webnovel_paragraphing_layout_rhythm_gate.md if chapter surface flow or mobile fatigue is in scope
rules/sltd_vietnamese_register_viet_dao_gate.md if register drift appears between scenes
rules/sltd_first_pass_editorial_workflow.md if governing chapter pressure is unclear
rules/sltd_anti_ai_composite_failure_gate.md if assembled chapter reads synthetic
prompts/chapter_assembly_split_check.md
prompts/node_checkpoint.md
```

### Packet / arc / webnovel benchmark

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_chapter_assembly_split_control_gate.md if chapter-level length or split risk appears
rules/sltd_character_distinctiveness_iceberg_gate.md if cast texture or character continuity is in scope
rules/sltd_webnovel_paragraphing_layout_rhythm_gate.md if layout rhythm affects reader experience
rules/sltd_vietnamese_register_viet_dao_gate.md if register affects reader texture
rules/sltd_first_pass_editorial_workflow.md if assessing first-pass quality
rules/sltd_scene_first_prose_judgment_gate.md
rules/sltd_anti_ai_composite_failure_gate.md
rules/sltd_character_agency_anti_ooc_gate.md
rules/sltd_dynamic_range_cadence_gate.md
rules/sltd_webnovel_momentum_benchmark.md
rules/sltd_review_modes.md
prompts/webnovel_packet_benchmark.md
prompts/node_checkpoint.md
prompts/result_report.md
```

### Entry healthcheck

```text
rules/sltd_pack_healthcheck.md
rules/sltd_evidence_discipline.md
rules/sltd_role_boundary_contracts.md
rules/sltd_agentic_iteration_loop.md
rules/sltd_calibration_discipline.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_handoff_continuity_protocol.md
rules/sltd_first_pass_editorial_workflow.md
rules/sltd_chapter_assembly_split_control_gate.md
rules/sltd_vietnamese_register_viet_dao_gate.md
rules/sltd_webnovel_paragraphing_layout_rhythm_gate.md
rules/sltd_character_distinctiveness_iceberg_gate.md
rules/sltd_scene_first_prose_judgment_gate.md
rules/sltd_dynamic_range_cadence_gate.md
rules/sltd_character_agency_anti_ooc_gate.md
rules/sltd_anti_ai_composite_failure_gate.md
ROLE_ENTRY_INDEX.md
prompts/entry_healthcheck.md
samples/router_examples.md
samples/viet_dao_prose_calibration.md
samples/dialogue_voice_calibration.md
```

## Rule

If the task is unclear, run `task_intake.md` and `sltd_decision_safety.md` before opening more files.

If the task asks for prose patch, line edit, line surgery, copyedit, proofread, rewrite, readiness, or lock and source surface is not exact, run `source_surface_check.md` before proceeding.

If beginning a first serious rewrite, line edit, or scene repair, run `first_pass_editorial_workflow.md` before targeted gates.

If characters feel skimmed, interchangeable, function-only, same-voiced, or lacking hidden life, run `character_distinctiveness_check.md`.

If scene edits are being assembled into a chapter, or chapter length/reader unit may be overloaded, run `chapter_assembly_split_check.md`.

If prose is too Chinese-translated, too Hán Việt-heavy, too modern-flat, or missing Viet Dao balance, run `vietnamese_register_check.md`.

If paragraphing, line breaks, short-line density, wall-text risk, or mobile readability affects reader breath, run `webnovel_paragraphing_layout_check.md`.

If prose work starts to satisfy gates before reading the scene as lived Vietnamese prose, run `scene_first_prose_judgment.md`.

If restraint, moderation, line edit, or anti-melodrama risks flattening scene cadence, run `dynamic_range_check.md`.

If a character appears to serve the plot, clue, scene card, or explanation rather than acting from pressure, run `character_agency_check.md`.

If a scene or chapter has many correct-looking passes but still reads arranged, synthetic, or over-polished, run `anti_ai_composite_check.md`.
