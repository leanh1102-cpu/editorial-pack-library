# SLTD Task Router

Map each request to a small route.

Base:

```text
boot_task -> source_preflight -> task_intake -> decision_safety
```

Routes:

```text
scene transition skiptime event cluster check: sltd_source_fidelity_anti_compression -> sltd_scene_transition_skiptime_event_cluster_gate -> scene_transition_skiptime_event_cluster_check -> node_checkpoint
timeline POV foreshadowing folklore check: sltd_source_fidelity_anti_compression -> sltd_timeline_pov_foreshadowing_folklore_gate -> scene_transition_skiptime_event_cluster_check if seam/skiptime/event cluster is in scope -> timeline_pov_foreshadowing_folklore_check -> node_checkpoint
prose craft style check: sltd_source_fidelity_anti_compression -> sltd_prose_craft_style_material_gate -> scene_transition_skiptime_event_cluster_check if sensory/material bridge or process trace is in scope -> prose_craft_style_check -> node_checkpoint
scene composition balance check: sltd_source_fidelity_anti_compression -> sltd_scene_composition_component_balance_gate -> scene_transition_skiptime_event_cluster_check if seam or skiptime affects component balance -> scene_composition_balance_check -> node_checkpoint
narrative beat escalation check: sltd_source_fidelity_anti_compression -> sltd_narrative_beat_escalation_aftershock_gate -> scene_transition_skiptime_event_cluster_check if transition/skiptime/event cluster carries beat pressure -> narrative_beat_escalation_check -> node_checkpoint
living world community motion check: sltd_source_fidelity_anti_compression -> sltd_living_world_community_motion_gate -> scene_transition_skiptime_event_cluster_check if world residue or skiptime process trace is in scope -> living_world_community_motion_check -> node_checkpoint
character distinctiveness check: sltd_source_fidelity_anti_compression -> sltd_character_distinctiveness_iceberg_gate -> scene_transition_skiptime_event_cluster_check if emotional continuity or object reset affects character read -> character_distinctiveness_check -> node_checkpoint
chapter assembly split check: sltd_source_fidelity_anti_compression -> sltd_chapter_assembly_split_control_gate -> scene_transition_skiptime_event_cluster_check if seams/skiptime/event clusters affect reader unit -> timeline_pov_foreshadowing_folklore_check if timeline/thread continuity affects reader unit -> prose_craft_style_check if craft/style drift affects reader unit -> scene_composition_balance_check if component balance affects reader unit -> narrative_beat_escalation_check if beat chain affects reader unit -> living_world_community_motion_check if world motion affects chapter surface -> chapter_assembly_split_check -> node_checkpoint
first-pass editorial workflow: sltd_source_fidelity_anti_compression -> sltd_first_pass_editorial_workflow -> scene_transition_skiptime_event_cluster_check if seam/skiptime/event cluster target is unclear -> timeline_pov_foreshadowing_folklore_check if timeline/POV/thread target is unclear -> prose_craft_style_check if craft/style/material target is unclear -> scene_composition_balance_check if component mix or ratio is unclear -> narrative_beat_escalation_check if beat escalation or aftershock is unclear -> living_world_community_motion_check if setting/community motion is unclear -> character_distinctiveness_check if character profile target is unclear -> first_pass_editorial_workflow -> node_checkpoint
scene rewrite: source_surface_check -> first_pass_editorial_workflow -> scene_transition_skiptime_event_cluster_check if transition, skiptime, or event cluster continuity is in scope -> timeline_pov_foreshadowing_folklore_check if timeline, POV, foreshadowing, folklore, or material thread is in scope -> prose_craft_style_check if writing/editing technique, genre, style, voice, or material is in scope -> scene_composition_balance_check if component mix or ratio is in scope -> narrative_beat_escalation_check if beat escalation or aftershock is in scope -> living_world_community_motion_check if setting/community/world motion is in scope -> character_distinctiveness_check if character distinctiveness is in scope -> webnovel_paragraphing_layout_check if layout is in scope -> vietnamese_register_check if register is in scope -> scene_first_prose_judgment if checklist-first risk appears -> anti_ai_composite_check if synthetic risk appears -> character_agency_check if agency risk appears -> dynamic_range_check if cadence risk appears -> rewrite_scene -> multi_reviewer_pass -> node_checkpoint
line surgery: source_surface_check -> scene_transition_skiptime_event_cluster_check if seam, skiptime, or object reset is the underlying issue -> timeline_pov_foreshadowing_folklore_check if POV leak or material thread is the underlying issue -> prose_craft_style_check if craft move selection is the underlying issue -> scene_composition_balance_check if component mix is the underlying issue -> narrative_beat_escalation_check if beat flatness is the underlying issue -> living_world_community_motion_check if setting/community detail is the issue -> character_distinctiveness_check if voice/body/object signature is the issue -> webnovel_paragraphing_layout_check if line breaks are the issue -> vietnamese_register_check if register is the issue -> line_surgery -> line_surgery_pass -> node_checkpoint
readiness: source_surface_check -> chapter_assembly_split_check if length/split affects readiness -> scene_transition_skiptime_event_cluster_check if seam break, skiptime, or fragmented event cluster affects human read -> timeline_pov_foreshadowing_folklore_check if timeline, POV, forgotten thread, or folklore risk affects human read -> prose_craft_style_check if craft/style/material failure affects human read -> scene_composition_balance_check if component imbalance affects human read -> narrative_beat_escalation_check if beat flatness or promise/payoff affects human read -> living_world_community_motion_check if static setting/community affects human read -> character_distinctiveness_check if character flatness affects human read -> webnovel_paragraphing_layout_check if layout affects human read -> vietnamese_register_check if register affects human read -> anti_ai_composite_check if false readiness risk appears -> publishing_readiness_reviewer -> chapter_readiness_check -> sltd_publishing_readiness -> node_checkpoint
```

Transition / skiptime / event cluster rule:

```text
If transition, scene seam, skiptime, process trace, sensory bridge, symbolic bridge, hard cut, object/material continuity, emotional continuity, or event cluster continuity is in scope, run scene transition skiptime event cluster check.
A transition must carry pressure, information, cost, time, POV access, material state, or aftershock.
Skiptime must leave process trace.
A sensory or symbolic bridge is valid only if it changes continuity, not just mood.
An event cluster must have start, development, result, and aftershock.
```

Timeline / POV / thread rule:

```text
If timeline, event order, POV boundary, reader knowledge, foreshadowing ledger, folklore mutation, material thread, planting density, or scene/chapter/packet thread management is in scope, run timeline POV foreshadowing folklore check.
Threads must be planted, held, paid, or retired with evidence.
```

Prose craft rule:

```text
If writing technique, editing technique, genre style, prose style, voice, material layer, or craft sample calibration is in scope, run prose craft style check.
Craft samples are calibration, not voice to imitate.
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
