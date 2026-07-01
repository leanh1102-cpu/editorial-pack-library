# SLTD Task Router

Map each request to a small route.

Base:

```text
boot_task -> source_preflight -> task_intake -> decision_safety
```

Routes:

```text
scene composition balance check: sltd_source_fidelity_anti_compression -> sltd_scene_composition_component_balance_gate -> scene_composition_balance_check -> node_checkpoint
narrative beat escalation check: sltd_source_fidelity_anti_compression -> sltd_narrative_beat_escalation_aftershock_gate -> scene_composition_balance_check if component mix hides beat flatness -> narrative_beat_escalation_check -> node_checkpoint
living world community motion check: sltd_source_fidelity_anti_compression -> sltd_living_world_community_motion_gate -> scene_composition_balance_check if setting/living world ratio is in scope -> living_world_community_motion_check -> node_checkpoint
character distinctiveness check: sltd_source_fidelity_anti_compression -> sltd_character_distinctiveness_iceberg_gate -> scene_composition_balance_check if dialogue/action/inner-thought balance affects cast life -> character_distinctiveness_check -> node_checkpoint
webnovel paragraphing layout check: sltd_source_fidelity_anti_compression -> sltd_webnovel_paragraphing_layout_rhythm_gate -> webnovel_paragraphing_layout_check -> node_checkpoint
vietnamese register check: sltd_source_fidelity_anti_compression -> sltd_vietnamese_register_viet_dao_gate -> vietnamese_register_check -> node_checkpoint
chapter assembly split check: sltd_source_fidelity_anti_compression -> sltd_chapter_assembly_split_control_gate -> scene_composition_balance_check if component balance affects reader unit -> narrative_beat_escalation_check if beat chain affects reader unit -> living_world_community_motion_check if world motion affects chapter surface -> chapter_assembly_split_check -> node_checkpoint
first-pass editorial workflow: sltd_source_fidelity_anti_compression -> sltd_first_pass_editorial_workflow -> scene_composition_balance_check if component mix or ratio is unclear -> narrative_beat_escalation_check if beat escalation or aftershock is unclear -> living_world_community_motion_check if setting/community motion is unclear -> character_distinctiveness_check if character profile target is unclear -> first_pass_editorial_workflow -> node_checkpoint
scene rewrite: source_surface_check -> first_pass_editorial_workflow -> scene_composition_balance_check if component mix or ratio is in scope -> narrative_beat_escalation_check if beat escalation or aftershock is in scope -> living_world_community_motion_check if setting/community/world motion is in scope -> character_distinctiveness_check if character distinctiveness is in scope -> webnovel_paragraphing_layout_check if layout is in scope -> vietnamese_register_check if register is in scope -> scene_first_prose_judgment if checklist-first risk appears -> anti_ai_composite_check if synthetic risk appears -> character_agency_check if agency risk appears -> dynamic_range_check if cadence risk appears -> rewrite_scene -> multi_reviewer_pass -> node_checkpoint
line surgery: source_surface_check -> scene_composition_balance_check if component mix is the underlying issue -> narrative_beat_escalation_check if beat flatness is the underlying issue -> living_world_community_motion_check if setting/community detail is the issue -> character_distinctiveness_check if voice/body/object signature is the issue -> webnovel_paragraphing_layout_check if line breaks are the issue -> vietnamese_register_check if register is the issue -> line_surgery -> line_surgery_pass -> node_checkpoint
readiness: source_surface_check -> chapter_assembly_split_check if length/split affects readiness -> scene_composition_balance_check if component imbalance affects human read -> narrative_beat_escalation_check if beat flatness or promise/payoff affects human read -> living_world_community_motion_check if static setting/community affects human read -> character_distinctiveness_check if character flatness affects human read -> webnovel_paragraphing_layout_check if layout affects human read -> vietnamese_register_check if register affects human read -> anti_ai_composite_check if false readiness risk appears -> publishing_readiness_reviewer -> chapter_readiness_check -> sltd_publishing_readiness -> node_checkpoint
```

Scene composition rule:

```text
If dialogue/action/blocking/inner thought/setting/object/sensory/silence/summary/aftershock ratio or component mix is in scope, run scene composition balance check.
Composition follows scene function.
Percentages are diagnostic bands, not writing formulas.
A component is valid only if it changes pressure, relation, information, cost, movement, or reader breath.
Do not add components only to fill a band.
```

Narrative beat rule:

```text
If beat rhythm, anchor point, escalation, interruption, aftershock, peak/result, off-POV conflict, parallel event, or promise/payoff is in scope, run narrative beat escalation check.
A beat is not an event. A beat must change pressure, information, position, cost, or promise.
```

Living world rule:

```text
If setting, community, custom, social habit, environment pushback, offscreen motion, or butterfly trace is in scope, run living world community motion check.
The world must not wait for the protagonist to enter.
```

Source fidelity rule:

```text
If the task requires exact prose, exact status, exact patch, or current lock, verify source surface first.
Do not edit prose from digest, summary, or chat memory.
```
