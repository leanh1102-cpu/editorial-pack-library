# SLTD Entry Fast Path

Use this file to choose the smallest SLTD route.

## Always read

```text
manifest.yml
DESIGN.md
PACK.md
AGENT_IDENTITY.md
rules/sltd_runtime_loop.md
rules/sltd_source_preflight.md
rules/sltd_decision_safety.md
```

## Pipeline order

```text
0. Source Preflight
1. Spine Lock
2. Tracking / Logic Ledger
3. Borderbound
4. Life-Task Bound
5. Story Movement
6. Scene-First Prose Judgment
7. Voice / Dialogue / Staging
8. Draft / Rewrite
9. Line / Voice / Rhythm
10. Composite Risk Check
11. Feedback Matrix / Report
12. Seam / Chapter Assembly
13. Readiness / Lock
```

Do not run later gears to hide failure in earlier gears. Do not draft prose before spine, tracking, border, and scene staging are clear when continuity or dialogue is at stake. Stop at the first real blocker.

## Fast paths

### Character voice / dialogue / relationship / location staging

```text
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_character_voice_dialogue_relationship_location_gate.md
samples/character_voice_dialogue_staging_calibration.md
rules/sltd_tracking_logic_ledger_traceability_gate.md if relationship memory, knowledge state, object state, or downstream risk is affected
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if scene function or border is unclear
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md if exact Vietnamese dialogue surface is in scope
rules/sltd_character_distinctiveness_iceberg_gate.md if voice profile is unclear
rules/sltd_living_world_community_motion_gate.md if group presence or community motion is in scope
prompts/character_voice_dialogue_staging_check.md
prompts/node_checkpoint.md
```

### General + chapter feedback matrix

```text
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_general_chapter_feedback_matrix_output_protocol.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if spine/source status is in scope
rules/sltd_tracking_logic_ledger_traceability_gate.md if state/thread/object/pass/downstream logic is in scope
rules/sltd_character_voice_dialogue_relationship_location_gate.md if dialogue, relationship, or staging is a packet issue
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md if human surface or pass integrity is in scope
prompts/general_chapter_feedback_matrix_check.md
prompts/node_checkpoint.md
```

### Tracking / structural / surface / prose work

```text
source_surface_check when exact prose or status is required
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md when spine or border is in scope
rules/sltd_tracking_logic_ledger_traceability_gate.md when logic continuity is affected
rules/sltd_character_voice_dialogue_relationship_location_gate.md when voice, relationship, or location staging is affected
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md when human surface or pass integrity is affected
relevant primary gate only when evidence requires it
prompts/node_checkpoint.md
```

## Rule

Run `character_voice_dialogue_staging_check.md` when the task concerns dialogue, multi-character scenes, character voice, relationship memory, silence, interruptions, location staging, usable objects, tone, comedy, grief, or physical action.

Run `general_chapter_feedback_matrix_check.md` when the task asks for general feedback plus chapter-by-chapter feedback, packet/arc/hồi review, or matrix-style review output.

Run `tracking_logic_ledger_check.md` when the task concerns logic continuity, state trace, knowledge state, object/residue/thread tracking, payoff debt, status/pass trace, downstream risk, or verify target.

Run `structural_spine_outline_preprose_check.md` when act/arc/hồi/chapter/scene, Story Outline, Chapter by Chapter Outline, Chapter Card, Scene Packet, borderbound, or prose permission is in scope.

Run `vietnamese_senior_editor_surface_check.md` when senior Vietnamese reading, từng chữ, semantic load, repeated AI smell, pass metadata, Human Chapter Pass, candidate-ready, or Publication Lock is in scope.
