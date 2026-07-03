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
7. Draft / Rewrite
8. Line / Voice / Rhythm
9. Composite Risk Check
10. Seam / Chapter Assembly
11. Readiness / Lock
```

Do not run later gears to hide failure in earlier gears. Do not draft prose before spine, tracking, and border are clear when logic continuity is at stake. Stop at the first real blocker.

## Fast paths

### Tracking / logic ledger / traceability

```text
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_tracking_logic_ledger_traceability_gate.md
samples/tracking_logic_ledger_calibration.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if act/arc/chapter/scene slot is unclear
rules/sltd_timeline_pov_foreshadowing_folklore_gate.md if thread/reveal/POV order is affected
rules/sltd_supernatural_event_residue_dread_amplitude_gate.md if object/residue state is affected
rules/sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md if knowledge state or kept detail is affected
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md if pass/status trace is affected
prompts/tracking_logic_ledger_check.md
prompts/node_checkpoint.md
```

### Structural spine / outline pre-prose / borderbound

```text
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md
rules/sltd_tracking_logic_ledger_traceability_gate.md if state/thread/object/knowledge tracking affects prose permission
prompts/structural_spine_outline_preprose_check.md
prompts/node_checkpoint.md
```

### Vietnamese senior editor surface / pass integrity

```text
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md
rules/sltd_tracking_logic_ledger_traceability_gate.md if pass/status trace, object logic, or downstream risk is unclear
prompts/vietnamese_senior_editor_surface_check.md
prompts/node_checkpoint.md
```

### Supernatural / protagonist / thread checks

```text
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_tracking_logic_ledger_traceability_gate.md if residue, object, knowledge, gain, or thread state must carry forward
relevant primary gate: supernatural_event_residue / protagonist_inquiry / protagonist_advancement / timeline_pov_foreshadowing_folklore
prompts/node_checkpoint.md
```

### First-pass / rewrite / line work

```text
prompts/source_surface_check.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md
rules/sltd_tracking_logic_ledger_traceability_gate.md
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md
rules/sltd_first_pass_editorial_workflow.md
additional gates only when evidence requires them
prompts/node_checkpoint.md
```

### Chapter / packet / arc review

```text
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md
rules/sltd_tracking_logic_ledger_traceability_gate.md
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md
other gates only when the primary route exposes a real blocker
prompts/context_brief.md
prompts/node_checkpoint.md
prompts/result_report.md
```

## Rule

Run `tracking_logic_ledger_check.md` when the task concerns logic continuity, state trace, knowledge state, object/residue/thread tracking, payoff debt, status/pass trace, downstream risk, or verify target.

Run `structural_spine_outline_preprose_check.md` when act/arc/hồi/chapter/scene, Story Outline, Chapter by Chapter Outline, Chapter Card, Scene Packet, borderbound, or prose permission is in scope.

Run `vietnamese_senior_editor_surface_check.md` when senior Vietnamese reading, từng chữ, semantic load, repeated AI smell, pass metadata, Human Chapter Pass, candidate-ready, or Publication Lock is in scope.
