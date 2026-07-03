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

## Route governance

If three or more checks compete, run:

```text
rules/sltd_entry_route_governance_gate_budget_protocol.md
prompts/entry_route_governance_check.md
prompts/node_checkpoint.md
```

## Fast paths

### Vietnamese senior editor surface / pass integrity

```text
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md
samples/vietnamese_senior_editor_surface_calibration.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if status, outline, card, packet, or border affects prose permission
rules/sltd_prose_craft_style_material_gate.md if sentence/object/material repair is needed
rules/sltd_anti_ai_composite_failure_gate.md if repeated synthetic prose appears
rules/sltd_vietnamese_register_viet_dao_gate.md if register or Vietnamese syntax is in scope
prompts/vietnamese_senior_editor_surface_check.md
prompts/node_checkpoint.md
```

### Structural spine / outline pre-prose / borderbound

```text
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md
samples/structural_spine_outline_preprose_calibration.md
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md if pass integrity affects prose permission
rules/sltd_timeline_pov_foreshadowing_folklore_gate.md if thread/reveal/POV order is in scope
rules/sltd_protagonist_advancement_growth_route_gate.md if protagonist gain must sit inside the spine
rules/sltd_supernatural_event_residue_dread_amplitude_gate.md if lore/residue must sit inside the spine
prompts/structural_spine_outline_preprose_check.md
prompts/node_checkpoint.md
```

### Supernatural event residue

```text
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_supernatural_event_residue_dread_amplitude_gate.md
samples/supernatural_event_residue_calibration.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if residue may not belong to the scene/chapter spine
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md if residue prose is overloaded or status is unclear
rules/sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md if Đại Phong must compare, test, misread, keep, or return to residue
prompts/supernatural_event_residue_check.md
prompts/node_checkpoint.md
```

### Protagonist inquiry / advancement

```text
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if inquiry or gain may not belong to scene/chapter function
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md if reasoning/gain prose sounds stiff or overloaded
rules/sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md
rules/sltd_protagonist_advancement_growth_route_gate.md
prompts/protagonist_inquiry_check.md or prompts/protagonist_advancement_check.md
prompts/node_checkpoint.md
```

### First-pass / rewrite / line work

```text
prompts/source_surface_check.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md
rules/sltd_first_pass_editorial_workflow.md
additional gates only when evidence requires them
prompts/first_pass_editorial_workflow.md or relevant prose prompt
prompts/node_checkpoint.md
```

### Chapter / packet / arc review

```text
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md
rules/sltd_supernatural_event_residue_dread_amplitude_gate.md if residue network is in scope
rules/sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md if inquiry route is in scope
rules/sltd_protagonist_advancement_growth_route_gate.md if growth route is in scope
rules/sltd_timeline_pov_foreshadowing_folklore_gate.md if thread/POV/folklore is in scope
prompts/context_brief.md
prompts/node_checkpoint.md
prompts/result_report.md
```

## Rule

If exact prose, current status, readiness, Vietnamese human surface, pass integrity, rewrite, line edit, or proofread is requested, verify source surface first.

Run `vietnamese_senior_editor_surface_check.md` when the task concerns senior Vietnamese reading, từng chữ, read-aloud friction, semantic load, repeated AI smell, pass metadata, Anti-AI Pass, Human Chapter Pass, candidate-ready, or Publication Lock.

Run `structural_spine_outline_preprose_check.md` when act/arc/hồi/chapter/scene, Story Outline, Chapter by Chapter Outline, Chapter Card, Scene Packet, borderbound, or prose permission is in scope.

Run the smallest route and stop at the first real blocker.
