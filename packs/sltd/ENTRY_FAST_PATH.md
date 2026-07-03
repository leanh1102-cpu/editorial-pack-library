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

## Spine pipeline order

Use gates as sequential gears, not as a checklist menu.

```text
0. Source Preflight
1. Spine Lock
2. Borderbound
3. Life-Task Bound
4. Story Movement
5. Scene-First Prose Judgment
6. Draft / Rewrite
7. Line / Voice / Rhythm
8. Anti-AI Composite
9. Seam / Chapter Assembly
10. Readiness / Lock
```

Rules:

```text
- Do not run later gears to hide failure in earlier gears.
- Do not draft prose before Life-Task Bound + Story Movement when the scene card risks characters serving outline labels.
- Do not claim readiness from green sub-passes without human-read prose and current source evidence.
- Use the smallest gear sequence that answers the user request, then stop.
```

Gear ownership:

```text
Source Preflight -> rules/sltd_source_preflight.md
Spine Lock / Borderbound -> rules/sltd_structural_spine_outline_preprose_borderbound_gate.md
Life-Task Bound -> rules/sltd_living_world_community_motion_gate.md + rules/sltd_character_agency_anti_ooc_gate.md
Story Movement -> rules/sltd_narrative_beat_escalation_aftershock_gate.md
Scene-First Prose Judgment -> rules/sltd_scene_first_prose_judgment_gate.md
Draft / Rewrite -> rules/sltd_first_pass_editorial_workflow.md
Line / Voice / Rhythm -> rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md + line/register gates when needed
Anti-AI Composite -> rules/sltd_anti_ai_composite_failure_gate.md
Readiness / Lock -> readiness route with current source evidence
```

## Fast paths

### Vietnamese senior editor surface / pass integrity

```text
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md
samples/vietnamese_senior_editor_surface_calibration.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if status, outline, card, packet, or border affects prose permission
rules/sltd_prose_craft_style_material_gate.md if sentence/object/material repair is needed
rules/sltd_scene_first_prose_judgment_gate.md if prose begins to satisfy gates before living pressure is found
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
rules/sltd_living_world_community_motion_gate.md if daily-life task, household work, community witness, custom, rumor, or world motion must prevent outline labels from driving characters
rules/sltd_narrative_beat_escalation_aftershock_gate.md if story movement, beat pressure, mini-payoff, aftershock, or benchmark pull is in scope
rules/sltd_character_agency_anti_ooc_gate.md if characters risk acting beyond knowledge, role, or life-task to serve scene function
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
rules/sltd_living_world_community_motion_gate.md if residue must appear through household, work, witness, animal, custom, rumor, or environment pushback before explanation
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
rules/sltd_narrative_beat_escalation_aftershock_gate.md if inquiry/gain must change pressure, cost, position, promise, or reader pull
prompts/protagonist_inquiry_check.md or prompts/protagonist_advancement_check.md
prompts/node_checkpoint.md
```

### First-pass / rewrite / line work

```text
prompts/source_surface_check.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md
rules/sltd_living_world_community_motion_gate.md if daily-life task or world motion is needed before prose
rules/sltd_narrative_beat_escalation_aftershock_gate.md if beat pressure, mini-payoff, or aftershock is needed before prose
rules/sltd_character_agency_anti_ooc_gate.md if characters risk serving scene function instead of acting from knowledge, role, and want
rules/sltd_scene_first_prose_judgment_gate.md before checklist repair when prose feels like gate compliance
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
rules/sltd_living_world_community_motion_gate.md if community motion, social trace, custom, household work, or world outside POV is in scope
rules/sltd_narrative_beat_escalation_aftershock_gate.md if beat rhythm, payoff, aftershock, or benchmark pull is in scope
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

If a scene card has correct function but risks characters acting to serve the card, run Life-Task Bound + Story Movement before prose by combining `sltd_living_world_community_motion_gate.md`, `sltd_narrative_beat_escalation_aftershock_gate.md`, and `sltd_character_agency_anti_ooc_gate.md` as capped secondary gates.

Run `scene_first_prose_judgment.md` before adding more repairs when prose looks like it is satisfying rules instead of moving as lived Vietnamese prose.

Run `anti_ai_composite_check.md` when a scene or chapter has many correct-looking passes but still reads arranged, synthetic, over-polished, or like a scene card converted into prose.

Run the smallest route and stop at the first real blocker.