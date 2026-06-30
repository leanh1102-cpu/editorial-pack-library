# SLTD Intensity Pass

Use this prompt when a scene is correct but too thin.

## Required files

1. `AI_ENTRY.md`
2. `packs/sltd/manifest.yml`
3. `packs/sltd/PACK.md`
4. `packs/sltd/rules/sltd_canon_guard.md`
5. `packs/sltd/rules/sltd_intensity_rules.md`
6. `packs/sltd/rules/sltd_intensity_targets.md`
7. source text from the user

If source text is missing, stop and ask for it.

## Method

1. Rate current intensity from 0 to 5.
2. Set target intensity from 0 to 5.
3. Identify missing force.
4. List what may be strengthened.
5. List what must stay locked.
6. Provide a patch or rewrite only inside scope.

## Output

```text
STATUS: PASS / UNDERREACHED / OVERREACHED
SCOPE:
PACK: sltd@1.3.0
CURRENT INTENSITY: 0-5
TARGET INTENSITY: 0-5

MISSING FORCE:
- ...

MAY STRENGTHEN:
- ...

LOCKED:
- ...

LEDGER:
SOURCE BASIS:
EXPANSION:
CONSEQUENCE:
ROLLBACK RISK:

PATCH OR REWRITE:
...
```

## Rule

A stronger scene must add pressure, cost, question, or changed state. It must not add new canon.
