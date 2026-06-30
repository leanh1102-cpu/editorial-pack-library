# SLTD Multi Reviewer Pass

Use this prompt when one answer should not trust a single reviewer voice.

## Required files

1. `AI_ENTRY.md`
2. `packs/sltd/manifest.yml`
3. `packs/sltd/PACK.md`
4. `packs/sltd/rules/sltd_source_preflight.md`
5. `packs/sltd/rules/sltd_editorial_hooks.md`
6. `packs/sltd/rules/sltd_canon_guard.md`
7. `packs/sltd/rules/sltd_underreach_gate.md`
8. task-specific rule or prompt
9. current user-provided source or Notion source

## Method

Run four separate reviewer lenses. Do not merge them into one vague verdict.

### 1. Canon Guard Reviewer

Checks:

- source priority;
- current vs legacy source;
- new canon;
- reveal timing;
- locked outcome.

### 2. Vietnamese Prose Reviewer

Checks:

- AI smell;
- stiff sentence rhythm;
- same-voice dialogue;
- summary where scene should act;
- object list without lived use.

### 3. Story Momentum Reviewer

Checks:

- hook;
- changed state;
- promise/payoff;
- residue;
- reader question.

### 4. Intensity Reviewer

Checks:

- underreach;
- missing cost;
- missing consequence;
- soft choice;
- mystery without pressure.

## Output

```text
SCOPE:
SOURCE USED:
PACK: sltd@1.4.0

CANON GUARD REVIEWER:
STATUS:
FINDINGS:

VIETNAMESE PROSE REVIEWER:
STATUS:
FINDINGS:

STORY MOMENTUM REVIEWER:
STATUS:
FINDINGS:

INTENSITY REVIEWER:
STATUS:
FINDINGS:

FINAL VERDICT:
PASS / NEEDS REVISION / STOP

NEXT ACTION:
```

## Rule

If any reviewer says STOP, final verdict must be STOP.

If the source is unclear, stop before reviewing.
