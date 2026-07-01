# SLTD Task Router

Map each request to a small route.

Base:

```text
boot_task -> source_preflight -> task_intake -> decision_safety
```

Routes:

```text
webnovel paragraphing layout check: sltd_source_fidelity_anti_compression -> sltd_webnovel_paragraphing_layout_rhythm_gate -> webnovel_paragraphing_layout_check -> node_checkpoint
vietnamese register check: sltd_source_fidelity_anti_compression -> sltd_vietnamese_register_viet_dao_gate -> vietnamese_register_check -> node_checkpoint
chapter assembly split check: sltd_source_fidelity_anti_compression -> sltd_chapter_assembly_split_control_gate -> webnovel_paragraphing_layout_check if layout affects chapter surface -> chapter_assembly_split_check -> node_checkpoint
first-pass editorial workflow: sltd_source_fidelity_anti_compression -> sltd_first_pass_editorial_workflow -> webnovel_paragraphing_layout_check if paragraphing target is unclear -> vietnamese_register_check if register target is unclear -> first_pass_editorial_workflow -> node_checkpoint
scene-first prose judgment: sltd_source_fidelity_anti_compression -> sltd_scene_first_prose_judgment_gate -> webnovel_paragraphing_layout_check if layout performs emotion or breaks reader breath -> vietnamese_register_check if register is miscalibrated -> scene_first_prose_judgment -> node_checkpoint
anti-AI composite check: sltd_source_fidelity_anti_compression -> sltd_scene_first_prose_judgment_gate if checklist-first risk appears -> sltd_webnovel_paragraphing_layout_rhythm_gate if AI layout risk appears -> sltd_vietnamese_register_viet_dao_gate if translated/flat register risk appears -> sltd_anti_ai_composite_failure_gate -> anti_ai_composite_check -> node_checkpoint
character agency check: sltd_source_fidelity_anti_compression -> sltd_character_agency_anti_ooc_gate -> character_agency_check -> node_checkpoint
dynamic range check: sltd_source_fidelity_anti_compression -> sltd_dynamic_range_cadence_gate -> webnovel_paragraphing_layout_check if visible paragraph rhythm contributes to flat cadence -> dynamic_range_check -> node_checkpoint
source surface check: sltd_source_fidelity_anti_compression -> source_surface_check -> node_checkpoint
chapter status: source_surface_check if current source unclear -> chapter_assembly_split_check if chapter length/reader unit is in scope -> webnovel_paragraphing_layout_check if layout affects readiness -> chapter_readiness_check -> mindmap_review -> node_checkpoint
packet review: sltd_source_fidelity_anti_compression -> chapter_assembly_split_check if chapter split risk appears -> webnovel_paragraphing_layout_check if layout rhythm affects reader experience -> vietnamese_register_check if register drift appears -> first_pass_editorial_workflow if first edit is requested -> scene_first_prose_judgment if checklist-first risk appears -> anti_ai_composite_check if synthetic/checklist risk appears -> character_agency_check if agency risk appears -> context_brief -> audit_story_arc -> mindmap_review -> editorial_director_review -> node_checkpoint
scene rewrite: source_surface_check -> first_pass_editorial_workflow -> webnovel_paragraphing_layout_check if paragraphing/layout is in scope -> vietnamese_register_check if register/Hán Việt/Viet Dao is in scope -> scene_first_prose_judgment if checklist-first risk appears -> anti_ai_composite_check if multiple-pass AI risk appears -> character_agency_check if OOC/OCC risk appears -> dynamic_range_check if restraint/cadence risk appears -> canon_guard -> sltd_editorial_hooks -> rewrite_scene -> multi_reviewer_pass -> node_checkpoint
chapter assembly after scene edits: source_surface_check -> chapter_assembly_split_check -> webnovel_paragraphing_layout_check if chapter surface flow or mobile fatigue is in scope -> vietnamese_register_check if register drifts between scenes -> anti_ai_composite_check if assembled chapter reads synthetic -> publishing_readiness_reviewer if split affects readiness -> node_checkpoint
line edit: source_surface_check -> webnovel_paragraphing_layout_check if line breaks/paragraphing are the issue -> vietnamese_register_check if Hán Việt/register balance is the issue -> first_pass_editorial_workflow if first serious edit -> scene_first_prose_judgment if prose reads like rule performance -> anti_ai_composite_check if repair collage risk appears -> character_agency_check if dialogue/action serves plot too neatly -> dynamic_range_check if cadence flattened -> vietnamese_line_editor -> sltd_canon_guard -> vietnamese_prose rules -> sltd_copyedit_proofread
line surgery: source_surface_check -> webnovel_paragraphing_layout_check if line breaks/paragraphing are the issue -> vietnamese_register_check if Hán Việt/register balance is the issue -> first_pass_editorial_workflow if first serious edit -> scene_first_prose_judgment if prose reads like rule performance -> anti_ai_composite_check if repair collage risk appears -> character_agency_check if dialogue/action serves plot too neatly -> dynamic_range_check if cadence flattened -> line_surgery -> sltd_vietnamese_line_surgery -> line_surgery_pass -> node_checkpoint
readiness: source_surface_check -> chapter_assembly_split_check if length/split affects readiness -> webnovel_paragraphing_layout_check if layout affects human read -> vietnamese_register_check if register affects human read -> scene_first_prose_judgment if prose readiness is inferred from checklist compliance -> anti_ai_composite_check if false readiness risk appears -> publishing_readiness_reviewer -> chapter_readiness_check -> sltd_publishing_readiness -> node_checkpoint
```

Paragraphing and layout rule:

```text
If paragraphing, line breaks, short-line density, wall-text risk, or mobile readability affects reader breath, run webnovel paragraphing layout check.
Paragraph is reader breath, not decoration.
Line break is a structural signal, not artificial emphasis.
One-sentence paragraphs are emphasis tools, not default style.
Avoid both choppy short-line rhythm and wall text.
```

Vietnamese register rule:

```text
If prose is too Chinese-translated, too Hán Việt-heavy, too modern-flat, or missing Viet Dao balance, run vietnamese register check.
Use Vietnamese life for body/work/poverty/illness/debt/weather/object pressure.
Use Sino-Vietnamese for canon, law, rite, rank, taboo, old object, and Dao pressure when earned.
```

Chapter assembly rule:

```text
If scene edits are being assembled into a chapter, or chapter length/reader unit may be overloaded, run chapter assembly split check.
Scene is the edit unit. Chapter is the reader unit. Packet is the continuity and momentum unit.
Do not split mechanically by word count alone.
```

First-pass rule:

```text
If beginning a first serious rewrite, line edit, line surgery, or scene repair, run first-pass editorial workflow before targeted gates.
Edit first as a human prose editor. Verify after.
Choose the earliest failing layer and one main edit strategy before writing.
```

Source fidelity rule:

```text
If the task requires exact prose, exact status, exact patch, or current lock, verify source surface first.
Do not line edit, line surgery, copyedit, proofread, rewrite, or patch from digest, summary, or chat memory.
```

Scene-first rule:

```text
If prose work starts by satisfying gates instead of judging the scene as lived Vietnamese prose, run scene-first prose judgment.
Use checklist as later verification, not as the writing method.
```

Character agency rule:

```text
If a character seems to serve the plot, clue, scene card, or explanation instead of acting from pressure, run character agency check.
```

Anti-AI composite rule:

```text
If a scene or chapter has many correct-looking passes but still reads arranged, synthetic, over-polished, or assembled, run anti-AI composite check.
Do not claim readiness from green sub-passes alone.
```

Dynamic range rule:

```text
If restraint, moderation, line edit, anti-melodrama, or subtlety causes a scene to become cleaner but flatter, run dynamic range check.
```

Gap output:

```text
SKILL GAP:
REQUEST TYPE:
MISSING ROUTE:
PROPOSED PATCH:
```
