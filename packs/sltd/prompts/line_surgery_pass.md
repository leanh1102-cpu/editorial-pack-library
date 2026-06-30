# SLTD Line Surgery Pass

Use this prompt when the user asks to audit or fix prose that still reads stiff, translated, over-clean, or AI-like at the line level.

This is a short-scope pass. Best scope is 300-1500 words. For a full chapter, sample the worst passage first unless the user explicitly asks for chapter-wide line surgery.

## Read first

1. `prompts/boot_task.md`
2. `rules/sltd_source_preflight.md`
3. `rules/sltd_vietnamese_line_surgery.md`
4. `core/vietnamese_prose/prose_rhythm.vi.md`
5. `core/vietnamese_prose/dialogue_voice.vi.md`
6. `core/vietnamese_prose/anti_ai_words.vi.md`
7. `packs/sltd/rules/sltd_style_rules.md`
8. `packs/sltd/AUTHOR_TASTE_EXAMPLES.md`
9. user request and source excerpt

## Source rule

If the user asks about current/latest/Notion manuscript, read current Notion source before verdict.

If the user provides an excerpt, use that excerpt as the source for local line surgery and do not claim current manuscript state.

## Modes

```text
detect = identify line issues only
patch = identify and propose minimal OLD/NEW fixes
verify = check whether a patched excerpt now reads naturally
```

Default to `patch` when the user asks why it feels AI-like or asks for improvement.

## Output

```text
LINE SURGERY PASS
SCOPE:
SOURCE USED:
MODE:
VERDICT:

LINE ISSUES:
1. OLD:
   PROBLEM TYPE:
   WHY IT READS AI:
   MINIMAL FIX PRINCIPLE:
   NEW:
   RISK:

PARAGRAPH RHYTHM:
- ...

DIALOGUE VOICE:
- ...

MOUTH-READ CHECK:
- ...

PATCH PRIORITY:
- MUST FIX:
- OPTIONAL:
- DO NOT TOUCH:

REWRITE THRESHOLD:
- under / over 30 percent line surgery load

NEXT NODE:
```

## Rules

- Do not rewrite the whole scene unless the verdict is `NEEDS_SCENE_REWRITE` and the user asks for rewrite.
- Prefer one exact sentence patch over paragraph-wide polishing.
- Do not add metaphor to hide stiffness.
- Do not replace abstract prose with another abstract phrase.
- Keep scene function and canon unchanged.
- If more than 30 percent of the excerpt needs surgery, stop patching and recommend scene rewrite.
- If speaker voice is weak, mark `VOICE_COLLAPSE` instead of polishing dialogue.
- If an object is only symbolic, mark `SYMBOL_LABEL` and make it affect action.
