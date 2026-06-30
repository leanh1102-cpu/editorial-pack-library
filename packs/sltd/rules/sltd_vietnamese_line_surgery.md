# SLTD Vietnamese Line Surgery Gate

This rule is for prose that is correct in content but still reads stiff, translated, over-clean, or AI-written.

It is a line-level repair gate, not a story rewrite tool. It must preserve canon, scene function, point of view, and current source.

## Use when

- the user says the prose reads stiff, unnatural, translated, AI-like, or not Vietnamese enough;
- `audit_scene` finds prose smell but the scene function may still be usable;
- a chapter passes broad story checks but fails human reading flow;
- `TASTELOCK`, `UNDERREACH`, or `line_edit` is requested over a short excerpt;
- a passage needs minimal patch before deciding whether full scene rewrite is necessary.

## Read with

- `core/vietnamese_prose/prose_rhythm.vi.md`
- `core/vietnamese_prose/dialogue_voice.vi.md`
- `core/vietnamese_prose/anti_ai_words.vi.md`
- `packs/sltd/rules/sltd_style_rules.md`
- `packs/sltd/AUTHOR_TASTE_EXAMPLES.md`
- current scene/chapter source or user-provided excerpt

## Hard limits

- Do not add canon.
- Do not change scene outcome.
- Do not add new beats unless the user asked for rewrite.
- Do not make prose more literary by adding abstract imagery.
- Do not replace an AI sentence with a prettier AI sentence.
- Do not continue patching if the passage needs scene reconstruction.

## Line issue labels

Use these labels when diagnosing prose.

### STIFF_TRANSLATED_SYNTAX

The sentence is grammatically understandable but its word order, modifier stack, or clause flow sounds translated or non-native.

Fix by reordering into spoken/narrative Vietnamese, cutting redundant connectors, and moving action earlier.

### ABSTRACT_PRESSURE

The line names pressure as an idea instead of making it happen through body, object, sound, position, weather, hunger, debt, illness, or risk.

Fix by replacing abstract explanation with concrete pressure.

### THESIS_SENTENCE

The line explains what the scene means.

Fix by cutting the explanation or turning it into action, refusal, silence, or object behavior.

### SYMBOL_LABEL

An object is used as a symbol label instead of a force inside the scene.

Fix by making the object change what a character can do.

### SAME_RHYTHM

Several sentences have the same length, opening shape, or rise-fall pattern.

Fix by varying sentence length and placing short sentences at pressure points.

### CLEAN_AI_TRANSITION

The paragraph transition is too smooth, explanatory, or essay-like.

Fix by entering through a physical interruption: hand, bowl, door, cough, dog, wind, tool, sound, or unfinished speech.

### DIALOGUE_TOO_CLEAN

A character speaks in complete, polished logic beyond age, class, stress, or relationship.

Fix by breaking the line, adding evasion, wrong hearing, half-sentence, silence, or object handling.

### VOICE_COLLAPSE

If speaker tags are removed, the reader cannot tell who is speaking.

Fix by restoring social position, habit, fear, age, work, or relationship pressure.

### ACTIONLESS_TALK

Characters stand still to exchange information.

Fix by letting the world move during speech.

### FALSE_LITERARY_IMAGE

The image sounds attractive but does not arise from the scene's objects, body, weather, labor, or setting.

Fix by removing it or replacing it with a scene-native image.

### OVEREXPLAINED_EMOTION

The line names fear, grief, pain, loneliness, shock, or dread before the page creates pressure.

Fix by using breath, throat, hands, eyes, stance, object contact, missed words, or bodily delay.

### MOBILE_DRAG

The sentence or paragraph is too heavy for webnovel/mobile reading.

Fix by splitting, cutting abstract padding, and moving the important action earlier.

## Minimal repair method

For each issue:

```text
OLD:
PROBLEM TYPE:
WHY IT READS AI:
MINIMAL FIX PRINCIPLE:
NEW:
RISK:
```

Do not patch a whole paragraph when one sentence is the real problem.

## Mouth-read check

After patching, silently test:

- Can a Vietnamese reader read it aloud without stumbling?
- Does the sentence sound written in Vietnamese, not translated into Vietnamese?
- Does the line carry scene action instead of commentary?
- Is the rhythm too even?
- Does the line still smell like a polished assistant sentence?

If the answer is bad, patch again or mark `NEEDS SCENE REWRITE`.

## Rewrite threshold

If more than 30 percent of the excerpt needs line surgery, do not keep patching line by line.

Return:

```text
NEEDS SCENE REWRITE
REASON:
- prose issue is structural, not local
- scene is built to explain rather than happen
- dialogue carries outline instead of pressure
- objects label meaning but do not change action
```

## Verdict labels

```text
LINE_SURGERY_PASS
NEEDS_LINE_SURGERY
NEEDS_SCENE_REWRITE
SOURCE_MISSING
```

## Output

```text
LINE SURGERY GATE
SCOPE:
SOURCE USED:
MODE: detect / patch / verify
VERDICT:

LINE ISSUES:
1. OLD:
   PROBLEM TYPE:
   WHY IT READS AI:
   MINIMAL FIX PRINCIPLE:
   NEW:
   RISK:

PARAGRAPH RHYTHM:
DIALOGUE VOICE:
MOUTH-READ CHECK:
PATCH PRIORITY:
REWRITE THRESHOLD:
NEXT NODE:
```
