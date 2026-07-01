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

### Protagonist inquiry / inner reasoning / clue chain check

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md
samples/protagonist_inquiry_calibration.md
rules/sltd_protagonist_advancement_growth_route_gate.md if inquiry should become protagonist gain
rules/sltd_timeline_pov_foreshadowing_folklore_gate.md if clue access, reveal window, folklore, or knowledge limit is in scope
rules/sltd_narrative_beat_escalation_aftershock_gate.md if inquiry lacks cost/result/aftershock
rules/sltd_prose_craft_style_material_gate.md if inner reasoning becomes explanation or object tag
rules/sltd_anti_ai_composite_failure_gate.md if clue chain becomes checklist prose
prompts/protagonist_inquiry_check.md
prompts/node_checkpoint.md
```

### Protagonist advancement / growth route check

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_protagonist_advancement_growth_route_gate.md
samples/protagonist_advancement_calibration.md
rules/sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md if gain requires private question, small test, kept detail, or clue return
rules/sltd_character_agency_anti_ooc_gate.md if behavior is forced by plot
rules/sltd_character_distinctiveness_iceberg_gate.md if growth depends on voice/body/iceberg profile
rules/sltd_timeline_pov_foreshadowing_folklore_gate.md if knowledge limit, lore access, thread, or C030 low-lore context is in scope
rules/sltd_narrative_beat_escalation_aftershock_gate.md if gain lacks cost/result/aftershock
rules/sltd_prose_craft_style_material_gate.md if object/body/relation/witness becomes prose tag
rules/sltd_anti_ai_composite_failure_gate.md if Notion labels become checklist prose
prompts/protagonist_advancement_check.md
prompts/node_checkpoint.md
```

### Entry route governance check

```text
prompts/task_intake.md
rules/sltd_entry_route_governance_gate_budget_protocol.md
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md if exact source may be needed
rules/sltd_decision_safety.md
rules/sltd_evidence_discipline.md
rules/sltd_role_boundary_contracts.md
prompts/entry_route_governance_check.md
prompts/node_checkpoint.md
```

### Scene transition / skiptime / event cluster check

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_scene_transition_skiptime_event_cluster_gate.md
rules/sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md if seam/skiptime breaks or carries Dai Phong inquiry
rules/sltd_protagonist_advancement_growth_route_gate.md if seam/skiptime changes protagonist gain
rules/sltd_timeline_pov_foreshadowing_folklore_gate.md if time cut, POV access, or thread continuity is in scope
rules/sltd_narrative_beat_escalation_aftershock_gate.md if aftershock, payoff, or beat result is in scope
rules/sltd_living_world_community_motion_gate.md if offscreen motion or world residue is in scope
rules/sltd_prose_craft_style_material_gate.md if sensory/material bridge is in scope
rules/sltd_chapter_assembly_split_control_gate.md if chapter flow or event cluster continuity is in scope
prompts/scene_transition_skiptime_event_cluster_check.md
prompts/node_checkpoint.md
```

### Timeline / POV / foreshadowing / folklore check

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_timeline_pov_foreshadowing_folklore_gate.md
rules/sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md if clue access, reveal window, private question, or knowledge chain is in scope
rules/sltd_protagonist_advancement_growth_route_gate.md if protagonist knowledge limit or growth route is in scope
rules/sltd_scene_transition_skiptime_event_cluster_gate.md if seam/skiptime/event cluster is in scope
rules/sltd_story_momentum.md
rules/sltd_narrative_beat_escalation_aftershock_gate.md if promise/payoff or off-POV return is in scope
rules/sltd_living_world_community_motion_gate.md if folklore/community behavior is in scope
rules/sltd_prose_craft_style_material_gate.md if material layer is in scope
rules/sltd_chapter_assembly_split_control_gate.md if chapter/packet continuity is in scope
rules/sltd_canon_guard.md if event order, folklore truth, geography, or custom is unclear
prompts/timeline_pov_foreshadowing_folklore_check.md
prompts/node_checkpoint.md
```

### Prose craft / style / material check

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_prose_craft_style_material_gate.md
samples/prose_craft_style_material_calibration.md
packs/sltd/AUTHOR_TASTE_EXAMPLES.md
rules/sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md if inner reasoning/clue comparison must be converted into lived prose
rules/sltd_protagonist_advancement_growth_route_gate.md if craft must carry protagonist gain
rules/sltd_scene_transition_skiptime_event_cluster_gate.md if sensory/material bridge or process trace is in scope
rules/sltd_timeline_pov_foreshadowing_folklore_gate.md if material thread or folklore planting is in scope
rules/sltd_vietnamese_line_surgery.md if sentence-level craft is in scope
rules/sltd_vietnamese_register_viet_dao_gate.md if register/style is in scope
rules/sltd_scene_composition_component_balance_gate.md if component mix is in scope
rules/sltd_narrative_beat_escalation_aftershock_gate.md if genre beat/cost/promise is in scope
rules/sltd_living_world_community_motion_gate.md if material/world texture is in scope
rules/sltd_character_distinctiveness_iceberg_gate.md if voice/character craft is in scope
prompts/prose_craft_style_check.md
prompts/node_checkpoint.md
```

### Scene composition & component balance check

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_scene_composition_component_balance_gate.md
rules/sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md if component mix hides inquiry or makes Dai Phong passive
rules/sltd_protagonist_advancement_growth_route_gate.md if component mix hides protagonist gain
rules/sltd_scene_transition_skiptime_event_cluster_gate.md if seam or skiptime affects component balance
rules/sltd_timeline_pov_foreshadowing_folklore_gate.md if planting density affects composition
rules/sltd_prose_craft_style_material_gate.md if craft move selection is in scope
rules/sltd_first_pass_editorial_workflow.md if scene function is unclear
rules/sltd_scene_first_prose_judgment_gate.md if checklist balance risk appears
rules/sltd_narrative_beat_escalation_aftershock_gate.md if fake balance comes from missing beat escalation
rules/sltd_living_world_community_motion_gate.md if setting/living world is decorative
rules/sltd_webnovel_paragraphing_layout_rhythm_gate.md if paragraphing creates false rhythm
prompts/scene_composition_balance_check.md
prompts/node_checkpoint.md
```

### Narrative beat escalation & aftershock check

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_narrative_beat_escalation_aftershock_gate.md
rules/sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md if beat should produce private question, test, clue, or small secret
rules/sltd_protagonist_advancement_growth_route_gate.md if beat should produce protagonist gain
rules/sltd_scene_transition_skiptime_event_cluster_gate.md if transition, skiptime, or event cluster carries beat pressure
rules/sltd_timeline_pov_foreshadowing_folklore_gate.md if planted/paid/held thread or POV access is in scope
rules/sltd_story_momentum.md
rules/sltd_prose_craft_style_material_gate.md if genre technique or craft move is in scope
rules/sltd_scene_composition_component_balance_gate.md if component mix hides beat flatness
rules/sltd_dynamic_range_cadence_gate.md if cadence rather than beat structure is the blocker
rules/sltd_living_world_community_motion_gate.md if off-POV or butterfly trace is in scope
rules/sltd_character_agency_anti_ooc_gate.md if beat depends on forced character choice
prompts/narrative_beat_escalation_check.md
prompts/node_checkpoint.md
```

### Living world & community motion check

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_living_world_community_motion_gate.md
rules/sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md if world pressure should provoke private question or small test
rules/sltd_protagonist_advancement_growth_route_gate.md if living-world pressure should change protagonist reading method
rules/sltd_scene_transition_skiptime_event_cluster_gate.md if world residue or skiptime process trace is in scope
rules/sltd_timeline_pov_foreshadowing_folklore_gate.md if folklore thread or material planting is in scope
rules/sltd_prose_craft_style_material_gate.md if material layer or world-texture craft is in scope
rules/sltd_scene_composition_component_balance_gate.md if setting ratio or component role is in scope
rules/sltd_story_momentum.md
rules/sltd_underreach_gate.md
rules/sltd_canon_guard.md if repair depends on geography, custom, social structure, or history
rules/sltd_anti_ai_composite_failure_gate.md if world repair becomes synthetic
prompts/living_world_community_motion_check.md
prompts/node_checkpoint.md
```

### Character distinctiveness & iceberg check

```text
prompts/task_intake.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_character_distinctiveness_iceberg_gate.md
rules/sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md if Dai Phong's private reasoning, curiosity, or silence profile is in scope
rules/sltd_protagonist_advancement_growth_route_gate.md if protagonist route/voice/body/signature method is in scope
rules/sltd_scene_transition_skiptime_event_cluster_gate.md if emotional continuity or object reset affects character read
rules/sltd_timeline_pov_foreshadowing_folklore_gate.md if character knowledge or thread access is in scope
rules/sltd_prose_craft_style_material_gate.md if voice/body/iceberg craft move is in scope
rules/sltd_scene_composition_component_balance_gate.md if dialogue/action/inner-thought balance affects cast life
rules/sltd_character_agency_anti_ooc_gate.md if plot is forcing behavior
rules/sltd_canon_guard.md if profile depends on canon or relation history
samples/dialogue_voice_calibration.md if voice collapse appears
prompts/character_distinctiveness_check.md
prompts/node_checkpoint.md
```

### First-pass / scene rewrite

```text
prompts/task_intake.md
rules/sltd_entry_route_governance_gate_budget_protocol.md if three or more gates appear relevant
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_first_pass_editorial_workflow.md
rules/sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md if Dai Phong's private question, small test, kept detail, clue chain, or small secret is in scope
rules/sltd_protagonist_advancement_growth_route_gate.md if Dai Phong's gain/limit/cost/forbidden gain is in scope
rules/sltd_scene_transition_skiptime_event_cluster_gate.md if transition, skiptime, or event cluster continuity is in scope
rules/sltd_timeline_pov_foreshadowing_folklore_gate.md if timeline, POV, planting density, folklore, or thread ledger is in scope
rules/sltd_prose_craft_style_material_gate.md if writing/editing technique, style, voice, genre, or material is in scope
samples/prose_craft_style_material_calibration.md if craft calibration is needed
rules/sltd_scene_composition_component_balance_gate.md if component mix or ratio is in scope
rules/sltd_narrative_beat_escalation_aftershock_gate.md if beat escalation, conflict peak, or aftershock is in scope
rules/sltd_living_world_community_motion_gate.md if setting/community/world motion is in scope
rules/sltd_character_distinctiveness_iceberg_gate.md if character distinctiveness is in scope
rules/sltd_webnovel_paragraphing_layout_rhythm_gate.md if paragraphing/layout is in scope
rules/sltd_vietnamese_register_viet_dao_gate.md if register is in scope
rules/sltd_scene_first_prose_judgment_gate.md
rules/sltd_anti_ai_composite_failure_gate.md if synthetic risk appears
rules/sltd_character_agency_anti_ooc_gate.md if agency risk appears
rules/sltd_dynamic_range_cadence_gate.md if cadence risk appears
prompts/first_pass_editorial_workflow.md or prompts/rewrite_scene.md
prompts/node_checkpoint.md
```

### Chapter / packet / arc review

```text
prompts/task_intake.md
rules/sltd_entry_route_governance_gate_budget_protocol.md if broad audit risks gate cascade
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md if Dai Phong's inquiry route or clue-chain pressure is in scope
rules/sltd_protagonist_advancement_growth_route_gate.md if Dai Phong's growth route or benchmark ambition is in scope
rules/sltd_scene_transition_skiptime_event_cluster_gate.md if seam continuity, skiptime, or event cluster affects packet quality
rules/sltd_timeline_pov_foreshadowing_folklore_gate.md if timeline, POV, folklore, material thread, or planted/paid/held ledger is in scope
rules/sltd_prose_craft_style_material_gate.md if craft/style/material drift affects packet quality
rules/sltd_scene_composition_component_balance_gate.md if component balance affects scene/chapter read
rules/sltd_narrative_beat_escalation_aftershock_gate.md if beat map, promise/payoff, or off-POV conflict is in scope
rules/sltd_chapter_assembly_split_control_gate.md if chapter length or reader unit is in scope
rules/sltd_living_world_community_motion_gate.md if world/community motion or social texture is in scope
rules/sltd_character_distinctiveness_iceberg_gate.md if cast texture or continuity is in scope
rules/sltd_webnovel_paragraphing_layout_rhythm_gate.md if layout affects reader experience
rules/sltd_vietnamese_register_viet_dao_gate.md if register affects reader texture
rules/sltd_anti_ai_composite_failure_gate.md if synthetic risk appears
prompts/context_brief.md
prompts/audit_story_arc.md or prompts/webnovel_packet_benchmark.md
prompts/node_checkpoint.md
prompts/result_report.md
```

### Line surgery

```text
prompts/task_intake.md
ROLE_ENTRY_INDEX.md
roles/line_surgery.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md if line-level thought/clue should carry private question or kept detail
rules/sltd_protagonist_advancement_growth_route_gate.md if line-level object/body/relation should carry protagonist gain
rules/sltd_scene_transition_skiptime_event_cluster_gate.md if seam, skiptime, or object reset is the underlying issue
rules/sltd_timeline_pov_foreshadowing_folklore_gate.md if POV leak or material thread is the underlying issue
rules/sltd_prose_craft_style_material_gate.md if craft move selection is the underlying issue
samples/prose_craft_style_material_calibration.md if a sample-guided move is needed
rules/sltd_scene_composition_component_balance_gate.md if component mix is the underlying issue
rules/sltd_narrative_beat_escalation_aftershock_gate.md if beat flatness is the underlying issue
rules/sltd_living_world_community_motion_gate.md if setting/community detail is the issue
rules/sltd_character_distinctiveness_iceberg_gate.md if voice/body/object signature is the issue
rules/sltd_webnovel_paragraphing_layout_rhythm_gate.md if line breaks are the issue
rules/sltd_vietnamese_register_viet_dao_gate.md if register is the issue
rules/sltd_vietnamese_line_surgery.md
prompts/source_surface_check.md if exact excerpt is not confirmed
prompts/line_surgery_pass.md
prompts/node_checkpoint.md
```

### Entry healthcheck

```text
rules/sltd_pack_healthcheck.md
rules/sltd_entry_route_governance_gate_budget_protocol.md
rules/sltd_protagonist_advancement_growth_route_gate.md
rules/sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md
samples/protagonist_advancement_calibration.md
samples/protagonist_inquiry_calibration.md
rules/sltd_scene_transition_skiptime_event_cluster_gate.md
rules/sltd_timeline_pov_foreshadowing_folklore_gate.md
rules/sltd_prose_craft_style_material_gate.md
rules/sltd_scene_composition_component_balance_gate.md
rules/sltd_narrative_beat_escalation_aftershock_gate.md
rules/sltd_living_world_community_motion_gate.md
rules/sltd_character_distinctiveness_iceberg_gate.md
rules/sltd_webnovel_paragraphing_layout_rhythm_gate.md
rules/sltd_vietnamese_register_viet_dao_gate.md
rules/sltd_chapter_assembly_split_control_gate.md
rules/sltd_first_pass_editorial_workflow.md
rules/sltd_scene_first_prose_judgment_gate.md
rules/sltd_anti_ai_composite_failure_gate.md
rules/sltd_character_agency_anti_ooc_gate.md
rules/sltd_dynamic_range_cadence_gate.md
prompts/entry_healthcheck.md
```

## Rule

If exact prose, current lock, readiness, rewrite, line edit, line surgery, copyedit, or proofread is requested and source surface is not exact, run `source_surface_check.md` first.

If a task could trigger three or more gates, or primary route / secondary gates / stop condition are unclear, run `entry_route_governance_check.md` first.

If Dai Phong's private question, inner reasoning, curiosity pressure, small test, kept detail, clue chain, small secret, supernatural pressure, or inquiry route is in scope, run `protagonist_inquiry_check.md`.

If Dai Phong's development path, protagonist gain, growth route, gain type, cost, knowledge limit, forbidden gain, world-rule sensitivity, or benchmark-level protagonist appeal is in scope, run `protagonist_advancement_check.md`.

If transition, scene seam, skiptime, process trace, sensory bridge, symbolic bridge, hard cut, object/material continuity, emotional continuity, or event cluster continuity is in scope, run `scene_transition_skiptime_event_cluster_check.md`.

If timeline, event order, POV boundary, reader knowledge, foreshadowing ledger, folklore mutation, material thread, planting density, or scene/chapter/packet thread management is in scope, run `timeline_pov_foreshadowing_folklore_check.md`.

If writing technique, editing technique, genre style, prose style, voice, material layer, or craft sample calibration is in scope, run `prose_craft_style_check.md`.

If dialogue/action/blocking/inner thought/setting/object/sensory/silence/summary/aftershock ratio or component mix is in scope, run `scene_composition_balance_check.md`.

If beat rhythm, anchor point, escalation, interruption, aftershock, peak/result, off-POV conflict, parallel event, or promise/payoff is in scope, run `narrative_beat_escalation_check.md`.

If setting, community, custom, social habit, environment pushback, offscreen motion, or butterfly trace is in scope, run `living_world_community_motion_check.md`.

If characters feel skimmed, interchangeable, function-only, same-voiced, or lacking hidden life, run `character_distinctiveness_check.md`.

If scene edits are being assembled into a chapter, or chapter length/reader unit may be overloaded, run `chapter_assembly_split_check.md`.

If prose is too Chinese-translated, too Hán Việt-heavy, too modern-flat, or missing Viet Dao balance, run `vietnamese_register_check.md`.

If paragraphing, line breaks, short-line density, wall-text risk, or mobile readability affects reader breath, run `webnovel_paragraphing_layout_check.md`.

If prose work starts to satisfy gates before reading the scene as lived Vietnamese prose, run `scene_first_prose_judgment.md`.

If a scene or chapter has many correct-looking passes but still reads arranged, synthetic, or over-polished, run `anti_ai_composite_check.md`.
