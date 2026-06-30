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
rules/sltd_vietnamese_line_surgery.md
core/vietnamese_prose/prose_rhythm.vi.md
core/vietnamese_prose/dialogue_voice.vi.md
core/vietnamese_prose/anti_ai_words.vi.md
packs/sltd/AUTHOR_TASTE_EXAMPLES.md
prompts/line_surgery_pass.md
prompts/node_checkpoint.md
```

### Webnovel momentum benchmark

```text
prompts/task_intake.md
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
ROLE_ENTRY_INDEX.md
prompts/entry_healthcheck.md
samples/router_examples.md
```

## Rule

If the task is unclear, run `task_intake.md` and `sltd_decision_safety.md` before opening more files.
