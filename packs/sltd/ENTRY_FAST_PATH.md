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

## Entry governance first

If a request could trigger three or more gates, or the primary route is unclear, run route governance before editorial checks.

```text
rules/sltd_entry_route_governance_gate_budget_protocol.md
prompts/entry_route_governance_check.md
```

Governance chooses one primary route, caps secondary gates, declares stop condition, and blocks gate cascade.

## Fast paths

### Structural spine / outline pre-prose / borderbound check

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md
samples/structural_spine_outline_preprose_calibration.md
rules/sltd_entry_route_governance_gate_budget_protocol.md if multiple downstream gates compete
rules/sltd_timeline_pov_foreshadowing_folklore_gate.md if thread, reveal window, POV access, or chapter order is in scope
rules/sltd_protagonist_advancement_growth_route_gate.md if protagonist gain must be mapped into the spine
rules/sltd_supernatural_event_residue_dread_amplitude_gate.md if supernatural/lore residue must be slotted into the spine
prompts/structural_spine_outline_preprose_check.md
prompts/node_checkpoint.md
```

### Supernatural event residue / dread amplitude check

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_supernatural_event_residue_dread_amplitude_gate.md
samples/supernatural_event_residue_calibration.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if the residue may not belong to the current chapter/scene spine
rules/sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md if Dai Phong should compare, test, misread, keep, or return to the residue
rules/sltd_timeline_pov_foreshadowing_folklore_gate.md if event root, reveal window, POV access, folklore truth, or thread return is in scope
prompts/supernatural_event_residue_check.md
prompts/node_checkpoint.md
```

### Protagonist inquiry / inner reasoning / clue chain check

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md
samples/protagonist_inquiry_calibration.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if the inquiry may not belong to the current scene/chapter function
rules/sltd_supernatural_event_residue_dread_amplitude_gate.md if the pressure sign needs event root or dread amplitude
rules/sltd_protagonist_advancement_growth_route_gate.md if inquiry should become protagonist gain
prompts/protagonist_inquiry_check.md
prompts/node_checkpoint.md
```

### Protagonist advancement / growth route check

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_protagonist_advancement_growth_route_gate.md
samples/protagonist_advancement_calibration.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if gain must be validated against act/arc/chapter/scene spine
rules/sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md if gain requires private question, small test, kept detail, or clue return
rules/sltd_supernatural_event_residue_dread_amplitude_gate.md if the gain depends on supernatural residue or dread pressure
prompts/protagonist_advancement_check.md
prompts/node_checkpoint.md
```

### Timeline / POV / foreshadowing / folklore check

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_timeline_pov_foreshadowing_folklore_gate.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if thread placement depends on act/arc/chapter/scene spine
rules/sltd_supernatural_event_residue_dread_amplitude_gate.md if folklore event root, supernatural residue, or dread amplitude is in scope
rules/sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md if clue access, reveal window, private question, or knowledge chain is in scope
prompts/timeline_pov_foreshadowing_folklore_check.md
prompts/node_checkpoint.md
```

### First-pass / scene rewrite

```text
prompts/task_intake.md
rules/sltd_entry_route_governance_gate_budget_protocol.md if three or more gates appear relevant
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md
rules/sltd_first_pass_editorial_workflow.md
rules/sltd_supernatural_event_residue_dread_amplitude_gate.md if supernatural residue, folklore incident, beast residue, relic trace, or dread amplitude is in scope
rules/sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md if Dai Phong's private question, small test, kept detail, clue chain, or small secret is in scope
rules/sltd_protagonist_advancement_growth_route_gate.md if Dai Phong's gain/limit/cost/forbidden gain is in scope
rules/sltd_timeline_pov_foreshadowing_folklore_gate.md if timeline, POV, planting density, folklore, or thread ledger is in scope
rules/sltd_prose_craft_style_material_gate.md if writing/editing technique, style, voice, genre, or material is in scope
rules/sltd_scene_first_prose_judgment_gate.md
rules/sltd_anti_ai_composite_failure_gate.md if synthetic risk appears
prompts/first_pass_editorial_workflow.md or prompts/rewrite_scene.md
prompts/node_checkpoint.md
```

### Chapter / packet / arc review

```text
prompts/task_intake.md
rules/sltd_entry_route_governance_gate_budget_protocol.md if broad audit risks gate cascade
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md
rules/sltd_supernatural_event_residue_dread_amplitude_gate.md if supernatural residue network, dread amplitude, folklore incident, beast residue, relic trace, or event residue ledger is in scope
rules/sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md if Dai Phong's inquiry route or clue-chain pressure is in scope
rules/sltd_protagonist_advancement_growth_route_gate.md if Dai Phong's growth route or benchmark ambition is in scope
rules/sltd_timeline_pov_foreshadowing_folklore_gate.md if timeline, POV, folklore, material thread, or planted/paid/held ledger is in scope
prompts/context_brief.md
prompts/audit_story_arc.md or prompts/webnovel_packet_benchmark.md
prompts/node_checkpoint.md
prompts/result_report.md
```

### Entry healthcheck

```text
rules/sltd_pack_healthcheck.md
rules/sltd_entry_route_governance_gate_budget_protocol.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md
rules/sltd_supernatural_event_residue_dread_amplitude_gate.md
rules/sltd_protagonist_advancement_growth_route_gate.md
rules/sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md
samples/structural_spine_outline_preprose_calibration.md
samples/supernatural_event_residue_calibration.md
samples/protagonist_advancement_calibration.md
samples/protagonist_inquiry_calibration.md
prompts/entry_healthcheck.md
```

## Rule

If exact prose, current lock, readiness, rewrite, line edit, line surgery, copyedit, or proofread is requested and source surface is not exact, run `source_surface_check.md` first.

If a task could trigger three or more gates, or primary route / secondary gates / stop condition are unclear, run `entry_route_governance_check.md` first.

If act, arc, hồi, chapter, scene, Story Outline, Chapter by Chapter Outline, Chapter Card, Scene Packet, Replacement Spine, borderbound, or prose permission is in scope, run `structural_spine_outline_preprose_check.md`.

If supernatural residue, dread amplitude, folklore incident, beast residue, relic trace, old battlefield leak, Mê Thúy Lâm, Hồn sương, Trọc khí, Cửu Thần residue, Bát Thần residue, or Event / Residue Ledger is in scope, run `supernatural_event_residue_check.md`.

If Dai Phong's private question, inner reasoning, curiosity pressure, small test, kept detail, clue chain, small secret, supernatural pressure, or inquiry route is in scope, run `protagonist_inquiry_check.md`.

If Dai Phong's development path, protagonist gain, growth route, gain type, cost, knowledge limit, forbidden gain, world-rule sensitivity, or benchmark-level protagonist appeal is in scope, run `protagonist_advancement_check.md`.

If prose work starts to satisfy gates before reading the scene as lived Vietnamese prose, run `scene_first_prose_judgment.md`.

If a scene or chapter has many correct-looking passes but still reads arranged, synthetic, or over-polished, run `anti_ai_composite_check.md`.
