# SLTD Task Router

Map each request to a small route.

Base:

```text
boot_task -> source_preflight -> task_intake -> decision_safety
```

Routes:

```text
living world community motion check: sltd_source_fidelity_anti_compression -> sltd_living_world_community_motion_gate -> living_world_community_motion_check -> node_checkpoint
character distinctiveness check: sltd_source_fidelity_anti_compression -> sltd_character_distinctiveness_iceberg_gate -> character_distinctiveness_check -> node_checkpoint
webnovel paragraphing layout check: sltd_source_fidelity_anti_compression -> sltd_webnovel_paragraphing_layout_rhythm_gate -> webnovel_paragraphing_layout_check -> node_checkpoint
vietnamese register check: sltd_source_fidelity_anti_compression -> sltd_vietnamese_register_viet_dao_gate -> vietnamese_register_check -> node_checkpoint
chapter assembly split check: sltd_source_fidelity_anti_compression -> sltd_chapter_assembly_split_control_gate -> living_world_community_motion_check if world motion affects chapter surface -> chapter_assembly_split_check -> node_checkpoint
first-pass editorial workflow: sltd_source_fidelity_anti_compression -> sltd_first_pass_editorial_workflow -> living_world_community_motion_check if setting/community motion is unclear -> character_distinctiveness_check if character profile target is unclear -> first_pass_editorial_workflow -> node_checkpoint
scene-first prose judgment: sltd_source_fidelity_anti_compression -> sltd_scene_first_prose_judgment_gate -> living_world_community_motion_check if setting reads as backdrop -> character_distinctiveness_check if characters read as functions -> scene_first_prose_judgment -> node_checkpoint
anti-AI composite check: sltd_source_fidelity_anti_compression -> sltd_living_world_community_motion_gate if world feels staged -> sltd_character_distinctiveness_iceberg_gate if cast reads flat -> sltd_webnovel_paragraphing_layout_rhythm_gate if AI layout risk appears -> sltd_vietnamese_register_viet_dao_gate if register risk appears -> sltd_anti_ai_composite_failure_gate -> anti_ai_composite_check -> node_checkpoint
scene rewrite: source_surface_check -> first_pass_editorial_workflow -> living_world_community_motion_check if setting/community/world motion is in scope -> character_distinctiveness_check if character distinctiveness is in scope -> webnovel_paragraphing_layout_check if layout is in scope -> vietnamese_register_check if register is in scope -> scene_first_prose_judgment if checklist-first risk appears -> anti_ai_composite_check if synthetic risk appears -> character_agency_check if agency risk appears -> dynamic_range_check if cadence risk appears -> rewrite_scene -> multi_reviewer_pass -> node_checkpoint
line surgery: source_surface_check -> living_world_community_motion_check if setting/community detail is the issue -> character_distinctiveness_check if voice/body/object signature is the issue -> webnovel_paragraphing_layout_check if line breaks are the issue -> vietnamese_register_check if register is the issue -> line_surgery -> line_surgery_pass -> node_checkpoint
readiness: source_surface_check -> chapter_assembly_split_check if length/split affects readiness -> living_world_community_motion_check if static setting/community affects human read -> character_distinctiveness_check if character flatness affects human read -> webnovel_paragraphing_layout_check if layout affects human read -> vietnamese_register_check if register affects human read -> anti_ai_composite_check if false readiness risk appears -> publishing_readiness_reviewer -> chapter_readiness_check -> sltd_publishing_readiness -> node_checkpoint
```

Living world rule:

```text
If setting, community, custom, social habit, environment pushback, offscreen motion, or butterfly trace is in scope, run living world community motion check.
The world must not wait for the protagonist to enter.
A location is not ready because it is described. A custom is not ready because it is named. A community is not ready because people appear as witnesses.
Do not invent major lore, custom, institution, ritual, faction, village history, or canon geography.
If evidence is missing, mark the gap instead of inventing worldbuilding.
```

Character distinctiveness rule:

```text
If characters feel skimmed, interchangeable, function-only, same-voiced, or lacking hidden life, run character distinctiveness check.
Do not invent trauma, backstory, hidden motive, symbol, title, or canon relation.
```

Paragraphing and layout rule:

```text
If paragraphing, line breaks, short-line density, wall-text risk, or mobile readability affects reader breath, run webnovel paragraphing layout check.
Paragraph is reader breath, not decoration.
```

Vietnamese register rule:

```text
If prose is too Chinese-translated, too Hán Việt-heavy, too modern-flat, or missing Viet Dao balance, run vietnamese register check.
```

Chapter assembly rule:

```text
If scene edits are being assembled into a chapter, or chapter length/reader unit may be overloaded, run chapter assembly split check.
Scene is the edit unit. Chapter is the reader unit.
```

Source fidelity rule:

```text
If the task requires exact prose, exact status, exact patch, or current lock, verify source surface first.
Do not edit prose from digest, summary, or chat memory.
```

Gap output:

```text
SKILL GAP:
REQUEST TYPE:
MISSING ROUTE:
PROPOSED PATCH:
```
