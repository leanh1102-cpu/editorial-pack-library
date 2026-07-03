# SLTD Task Router

Map each request to a small route.

Base:

```text
boot_task -> source_preflight -> task_intake -> decision_safety
```

Routes:

```text
entry route governance check: sltd_entry_route_governance_gate_budget_protocol -> entry_route_governance_check -> node_checkpoint
structural spine outline pre-prose check: sltd_source_fidelity_anti_compression -> sltd_structural_spine_outline_preprose_borderbound_gate -> structural_spine_outline_preprose_check -> node_checkpoint
supernatural event residue check: sltd_source_fidelity_anti_compression -> sltd_supernatural_event_residue_dread_amplitude_gate -> structural_spine_outline_preprose_check if residue may not belong to current scene/chapter spine -> supernatural_event_residue_check -> node_checkpoint
protagonist inquiry check: sltd_source_fidelity_anti_compression -> sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate -> structural_spine_outline_preprose_check if inquiry may not belong to current scene/chapter function -> supernatural_event_residue_check if pressure sign needs event root/dread amplitude -> protagonist_inquiry_check -> node_checkpoint
protagonist advancement check: sltd_source_fidelity_anti_compression -> sltd_protagonist_advancement_growth_route_gate -> structural_spine_outline_preprose_check if gain must be validated against act/arc/chapter/scene spine -> supernatural_event_residue_check if gain depends on supernatural residue -> protagonist_inquiry_check if growth requires private question, small test, kept detail, or clue return -> protagonist_advancement_check -> node_checkpoint
timeline POV foreshadowing folklore check: sltd_source_fidelity_anti_compression -> sltd_timeline_pov_foreshadowing_folklore_gate -> structural_spine_outline_preprose_check if thread placement depends on act/arc/chapter/scene spine -> supernatural_event_residue_check if folklore event root or dread residue is in scope -> protagonist_inquiry_check if clue access, reveal window, or private reasoning is in scope -> timeline_pov_foreshadowing_folklore_check -> node_checkpoint
living world community motion check: sltd_source_fidelity_anti_compression -> sltd_living_world_community_motion_gate -> structural_spine_outline_preprose_check if community motion depends on chapter/arc spine -> supernatural_event_residue_check if social/community/animal residue is in scope -> living_world_community_motion_check -> node_checkpoint
scene rewrite: source_surface_check -> structural_spine_outline_preprose_check -> entry_route_governance_check if three or more downstream gates compete -> first_pass_editorial_workflow -> supernatural_event_residue_check if supernatural residue, folklore incident, beast residue, relic trace, or dread amplitude is in scope -> protagonist_inquiry_check if Dai Phong's private question, small test, kept detail, clue chain, or small secret is in scope -> protagonist_advancement_check if Dai Phong's gain/limit/cost/forbidden gain is in scope -> timeline_pov_foreshadowing_folklore_check if timeline/POV/thread is in scope -> prose_craft_style_check if craft/style is in scope -> rewrite_scene -> multi_reviewer_pass -> node_checkpoint
line surgery: source_surface_check -> structural_spine_outline_preprose_check if line-level change may cross scene/chapter border -> entry_route_governance_check if multiple blockers compete -> supernatural_event_residue_check if line-level supernatural sign needs event root/residue/dread pressure -> protagonist_inquiry_check if line-level thought/clue should carry private question or kept detail -> line_surgery -> line_surgery_pass -> node_checkpoint
readiness: source_surface_check -> structural_spine_outline_preprose_check if chapter/arc spine, Chapter Card, Scene Packet, or borderbound affects human read -> entry_route_governance_check if more than four checks appear relevant -> supernatural_event_residue_check if underpowered dread or missing event residue affects human read -> protagonist_inquiry_check if passive protagonist or clue-chain pressure affects human read -> protagonist_advancement_check if protagonist gain/forbidden gain affects human read -> publishing_readiness_reviewer -> chapter_readiness_check -> sltd_publishing_readiness -> node_checkpoint
```

Structural spine rule:

```text
If act, arc, hồi, chapter, scene, Story Outline, Chapter by Chapter Outline, Chapter Card, Scene Packet, Replacement Spine, borderbound, or prose permission is in scope, run structural spine outline pre-prose check.
Do not use prose to solve missing structure.
Prose is blocked when current outline, Chapter Card, Scene Packet, Canon In/Out, Must Show, Must Not Reveal, changed state, or reader effect is required but missing.
Protagonist gain, supernatural residue, lore, and clue chain must be slotted into the current scene/chapter spine before prose work.
```

Supernatural event residue rule:

```text
If supernatural residue, dread amplitude, folklore incident, beast residue, relic trace, old battlefield leak, Mê Thúy Lâm, Hồn sương, Trọc khí, Cửu Thần residue, Bát Thần residue, or Event / Residue Ledger is in scope, run supernatural event residue check.
A supernatural sign must be residue of event, ecology, wound, taboo, beast conflict, relic trace, battlefield trace, or community memory.
Canon discipline must not overclamp dread into mood-only fog, cold, silence, or vague omen.
Deep lore may appear early only as residue, not explanation.
Do not add source-unsupported lore, beast species, war facts, relics, or future reveals.
```

Protagonist inquiry rule:

```text
If Dai Phong's private question, inner reasoning, curiosity pressure, small test, kept detail, clue chain, small secret, supernatural pressure, or inquiry route is in scope, run protagonist inquiry check.
A strange sign must create private question, small test, kept detail, partial read/misread, or next return.
Inner reasoning should place concrete signs beside each other, not explain the world.
```

Protagonist advancement rule:

```text
If Dai Phong's development path, protagonist gain, growth route, gain type, cost, knowledge limit, forbidden gain, world-rule sensitivity, or benchmark-level protagonist appeal is in scope, run protagonist advancement check.
A protagonist gain must be shown through object, body, relation, witness/social trace, cost, knowledge limit, and aftershock.
```

Entry governance rule:

```text
If a task could trigger three or more gates, or primary route / secondary gates / stop condition are unclear, run entry route governance check.
Choose one primary route.
Add secondary gates only when the primary route exposes a real blocker.
Do not run a gate because it is adjacent.
Stop when the source is missing, the requested answer is complete, the patch is complete, readiness is blocked, or the gate budget is spent.
```

Source fidelity rule:

```text
If the task requires exact prose, exact status, exact patch, or current lock, verify source surface first.
Do not edit prose from digest, summary, or chat memory.
```
