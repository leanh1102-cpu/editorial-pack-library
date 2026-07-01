# SLTD Scene-First Prose Judgment

Use this prompt when AI output seems to satisfy the system before serving the scene.

This prompt is for editorial judgment before checklist application.

## Read first

```text
manifest.yml
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_scene_first_prose_judgment_gate.md
rules/sltd_anti_ai_composite_failure_gate.md
rules/sltd_character_agency_anti_ooc_gate.md
rules/sltd_dynamic_range_cadence_gate.md
rules/sltd_role_boundary_contracts.md
AUTHOR_TASTE_EXAMPLES.md
```

## Output

```text
SCENE-FIRST PROSE JUDGMENT
SCOPE:
SOURCE USED:
SOURCE SURFACE:
SCENE FUNCTION:
LIVING PRESSURE:
WHO IS UNDER PRESSURE:
PRACTICAL ACTION:
WHAT MUST STAY UNSAID:
WHAT MUST BE FELT:
ONE GOVERNING PRESSURE:
CHECKLIST VISIBLE:
PROSE LIFE STATUS:
PRIMARY FAILURE:
REPAIR LEVEL:
ROLE HANDOFF:
NEXT NODE:
```

## Patch output when exact source is available

```text
OLD:
WHY IT READS LIKE CHECKLIST:
NEW:
WHAT RULE-PERFORMANCE WAS REMOVED:
WHAT NOW DRIVES THE PROSE:
RISK:
```

## Rules

- Do not patch without exact source text.
- Do not begin by satisfying gates.
- Find one governing scene pressure before recommending repair.
- Use checklist only as later verification, not as the writing method.
- Do not add more body/object/silence/cost beats to hide checklist-first prose.
- If no governing pressure is found, hand off to Story Doctor or Anti-AI Composite Check.
- If character pressure is false, hand off to Character Agency Check.
- If cadence is flat, hand off to Dynamic Range Check.
- If only line rhythm remains after scene judgment, hand off to Line Surgery.
- End with NEXT NODE.
