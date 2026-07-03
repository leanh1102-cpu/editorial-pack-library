# SLTD Vietnamese Senior Editor Surface Check

Use this prompt when senior Vietnamese editor review, human prose surface, từng chữ, read-aloud friction, semantic load, pass integrity, or repeated AI-smell diagnosis is in scope.

This prompt does not authorize readiness claims from metadata alone and does not authorize rewriting without exact source excerpt.

## Read first

```text
manifest.yml
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md
rules/sltd_prose_craft_style_material_gate.md
rules/sltd_anti_ai_composite_failure_gate.md
rules/sltd_vietnamese_register_viet_dao_gate.md
```

## Output

```text
VIETNAMESE SENIOR EDITOR SURFACE / PASS INTEGRITY CHECK
SCOPE:
SOURCE USED:
SOURCE SURFACE:
CHAPTER / SCENE:
CURRENT STATUS:
PASS METADATA:
PASS CONFLICTS:
READ-ALOUD FRICTION:
WORD-CHOICE FRICTION:
SEMANTIC LOAD:
OBJECT FUNCTION VISIBILITY:
NEGATIVE EXPLANATION STACK:
DIALOGUE NATURALNESS:
BODY / ACTION BELIEVABILITY:
SENSORY THINNESS:
STATIC TALK:
VIETNAMESE RHYTHM:
OVERDENSITY:
HUMAN BREATH SPACE:
RECURRING SMELL FROM PRIOR CHAPTERS:
STATUS VERDICT:
SAFE REPAIR:
PROSE PERMISSION:
NEXT NODE:
```

## Rules

- Do not assess exact prose without exact source surface.
- Do not rewrite unless the user asks for repair and excerpt is available.
- Do not treat Anti-AI Pass, candidate-ready, or formal status update as Human Chapter Pass.
- If pass metadata conflicts, mark PASS_METADATA_CONFLICT.
- If Human Chapter Pass is NO or Publication Lock is Not Ready, do not claim publication readiness.
- Check read-aloud friction, Vietnamese word choice, dialogue naturalness, bodily plausibility, object-function visibility, semantic load, and human breath space.
- Escalate repeated smells across chapters into packet-level blocker.
- End with NEXT NODE.

## Patch output when exact source is available

```text
OLD:
SURFACE FAILURE:
WHY IT READS AI / STIFF / OVERLOADED:
NEW:
WHAT WAS REDUCED:
RISK:
NEXT NODE:
```

If exact source is missing, return SOURCE_SURFACE_REQUIRED.