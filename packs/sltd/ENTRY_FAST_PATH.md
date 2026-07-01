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

### Character agency check

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_character_agency_anti_ooc_gate.md
rules/sltd_canon_guard.md
rules/sltd_role_boundary_contracts.md
packs/sltd/AUTHOR_TASTE_EXAMPLES.md
prompts/character_agency_check.md
prompts/node_checkpoint.md
```

### Dynamic range check

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_dynamic_range_cadence_gate.md
rules/sltd_intensity_targets.md
rules/sltd_intensity_rules.md
packs/sltd/AUTHOR_TASTE_EXAMPLES.md
prompts/dynamic_range_check.md
prompts/node_checkpoint.md
```

### Handoff continuity

```text
prompts/task_intake.md
rules/sltd_handoff_continuity_protocol.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_evidence_discipline.md
rules/sltd_role_boundary_contracts.md
prompts/node_checkpoint.md
prompts/session_handoff.md
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

### Calibration case check

```text
prompts/task_intake.md
rules/sltd_calibration_discipline.md
samples/line_surgery_calibration.md if prose smell
samples/dialogue_voice_calibration.md if dialogue voice
samples/underreach_calibration.md if underreach
samples/readiness_false_positive.md if readiness or lock
rules/sltd_evidence_discipline.md
prompts/node_checkpoint.md
```

### Agentic iteration loop

```text
prompts/task_intake.md
rules/sltd_agentic_iteration_loop.md
rules/sltd_task_router.md
rules/sltd_decision_safety.md
rules/sltd_source_fidelity_anti_compression.md when source surface may be compressed
ROLE_ENTRY_INDEX.md if a role is named
rules/sltd_role_boundary_contracts.md if roles overlap
rules/sltd_evidence_discipline.md
prompts/iteration_checkpoint.md
prompts/node_checkpoint.md
```

### Role entry

```text
ROLE_ENTRY_INDEX.md
roles/<requested_role>.md
rules/sltd_role_boundary_contracts.md
rules/sltd_decision_safety.md
prompts/node_checkpoint.md
```

### Current chapter status

```text
prompts/task_intake.md
rules/sltd_decision_safety.md
prompts/chapter_readiness_check.md
prompts/node_checkpoint.md
prompts/result_report.md
```

### Packet or arc review

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_character_agency_anti_ooc_gate.md if character agency risk appears
rules/sltd_context_window_strategy.md
prompts/context_brief.md
prompts/audit_story_arc.md
prompts/editorial_director_review.md
prompts/node_checkpoint.md
prompts/result_report.md
```

### Scene rewrite

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_character_agency_anti_ooc_gate.md
rules/sltd_dynamic_range_cadence_gate.md if restraint or cadence risk appears
rules/sltd_editorial_hooks.md
rules/sltd_canon_guard.md
rules/sltd_intensity_rules.md
prompts/rewrite_scene.md
prompts/multi_reviewer_pass.md
prompts/node_checkpoint.md
```

### Underreach fix

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md if only digest/memory is available
rules/sltd_character_agency_anti_ooc_gate.md if plot seems to force character behavior
rules/sltd_dynamic_range_cadence_gate.md if scene is clean but not sharp
rules/sltd_underreach_gate.md
rules/sltd_intensity_targets.md
prompts/intensity_pass.md
prompts/node_checkpoint.md
```

### Line surgery

```text
prompts/task_intake.md
ROLE_ENTRY_INDEX.md
roles/line_surgery.md
rules/sltd_source_fidelity_anti_compression.md
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

### Webnovel momentum benchmark

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_character_agency_anti_ooc_gate.md
rules/sltd_dynamic_range_cadence_gate.md
rules/sltd_webnovel_momentum_benchmark.md
rules/sltd_review_modes.md
prompts/webnovel_packet_benchmark.md
prompts/node_checkpoint.md
prompts/result_report.md
```

### Review mode pass

```text
prompts/task_intake.md
rules/sltd_review_modes.md
rules/sltd_evidence_discipline.md
prompts/review_mode_pass.md
prompts/node_checkpoint.md
```

### Role boundary check

```text
EDITORIAL_COMPETENCY_MAP.md
ROLE_ENTRY_INDEX.md
rules/sltd_role_boundary_contracts.md
rules/sltd_decision_safety.md
prompts/node_checkpoint.md
```

### Mindmap or node check

```text
EDITORIAL_MINDMAP.md
rules/sltd_node_traversal.md
prompts/mindmap_review.md
prompts/node_checkpoint.md
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
rules/sltd_dynamic_range_cadence_gate.md
rules/sltd_character_agency_anti_ooc_gate.md
ROLE_ENTRY_INDEX.md
prompts/entry_healthcheck.md
samples/router_examples.md
```

## Rule

If the task is unclear, run `task_intake.md` and `sltd_decision_safety.md` before opening more files.

If the task asks for prose patch, line edit, line surgery, copyedit, proofread, rewrite, readiness, or lock and source surface is not exact, run `source_surface_check.md` before proceeding.

If context is degrading or a task must move to another chat, run `session_handoff.md` with `sltd_handoff_continuity_protocol.md`.

If restraint, moderation, line edit, or anti-melodrama risks flattening scene cadence, run `dynamic_range_check.md`.

If a character appears to serve the plot, clue, scene card, or explanation rather than acting from pressure, run `character_agency_check.md`.
