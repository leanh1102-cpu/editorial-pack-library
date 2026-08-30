# DIALOGUE-TEXTURE / TERSE-SATURATION v0.1 — Evaluator

## Status
`FROZEN / EVALUATOR-ONLY`

Do not expose this file to the model during a blind run.

## Target capability
The model must distinguish functional brevity from exchange-level terse saturation. It should preserve short turns when pressure, voice, silence, or surrounding action carries their work, while revising exchanges whose repeated bare propositions flatten Vietnamese relational texture, speaker differentiation, emotional shading, or pressure-sensitive recovery.

This is not a verbosity benchmark. Longer is not automatically better.

## Scoring
Each case: 0–2 points. Maximum: 24.

- `2`: correct action class and mechanism; output preserves meaning/voice while solving the local exchange-level problem.
- `1`: correct direction but action scale is off, output over/under-corrects slightly, or adds mild unsupported texture without changing plot meaning.
- `0`: misses the core mechanism, applies a universal length rule, destroys marked voice/register, or preserves/reproduces the target failure.

Promotion gate: `24/24 + hard fail 0`.

## Hard fails
Any of the following is a hard fail:
1. inventing a universal minimum/maximum dialogue length or turn-count quota;
2. lengthening every short turn solely because it is short;
3. flattening stable dialect/idiolect or kinship/register markers into neutral prestige Vietnamese;
4. adding new plot facts, motives, lore, or emotional certainties to repair texture;
5. converting intentional hesitation/silence into polished explanatory prose;
6. treating all speakers as one generic polished or one generic terse register;
7. claiming that Vietnamese relational particles or kinship address are filler by default.

## Case keys

### DT-01
Expected: `PRESERVE`.
Full credit: recognizes emergency time compression plus surrounding physical context; no padding. Short turns are functional.

### DT-02
Expected: `REVISE`.
Full credit: diagnoses exchange-level terse saturation under low pressure; restores some relational/emotional texture and syntactic variation without adding plot information or making every turn long. A strong revision can preserve guardedness while making mother/son relation audible.

### DT-03
Expected: `PRESERVE`.
Full credit: keeps `má/con/thôi/vậy/chi` and recognizes them as relational/register-bearing, not filler.

### DT-04
Expected: `REVISE`.
Full credit: differentiates at least the three speaker voices/statuses or rewrites the exchange so their roles become audible; does not merely lengthen all six turns uniformly.

### DT-05
Expected: `MIN_EDIT` or narrowly scoped `REVISE` only if the reason explicitly confines revision to the post-alarm recovery segment. Full 2 points requires recognizing that the emergency cluster should remain clipped while some later turns should expand/recover according to aftershock/care. Broad rewrite of the entire exchange scores at most 1.

### DT-06
Expected: `PRESERVE`.
Full credit: understands that emotional context is already carried by body/action/relationship; does not inflate speech to name feelings.

### DT-07
Expected: `PRESERVE`.
Full credit: hesitation/self-repair are functional social-emotional signals; no smoothing into a flawless sentence.

### DT-08
Expected: `REVISE`.
Full credit: makes grandmother/granddaughter relation audible through address, indirectness, response shape, or particles while preserving only the given facts; avoids verbosity uniformity.

### DT-09
Expected: `PRESERVE`.
Full credit: recognizes functional mixed-length rhythm based on social role and task; does not equalize turn length.

### DT-10
Expected: `REVISE` as a composition action.
Full credit output must:
- contain exactly six dialogue turns;
- keep only the supplied conflict: sell last chicken vs keep it, medicine cost pressure, mutual fear/affection;
- make mother/daughter relation audible in natural Vietnamese;
- vary syntax/turn length for function rather than mechanically;
- include at least one indirect, softened, self-protective, or relationally marked turn;
- avoid six bare proposition-only fragments;
- avoid exposition dump or explicit emotion labels such as `con sợ`/`mẹ rất đau lòng` unless organically necessary and supported.
A six-turn exchange where all turns are terse and interchangeable scores 0.

### DT-11
Expected: `PRESERVE`.
Full credit: preserves dockworker dialect and supervisor formal contrast; no prestige normalization.

### DT-12
Expected: `PRESERVE`.
Full credit: rejects the requested eight-word minimum because sentence length alone is not a valid defect and the current variation is functionally pressure-driven.

## Diagnostic dimensions
Record misses under one primary label:
- `TERSE-SATURATION-DETECTION`
- `RELATIONAL-TEXTURE`
- `VOICE-DIFFERENTIATION`
- `PRESSURE-RECOVERY`
- `OVERLENGTHENING`
- `DIALECT-PRESERVATION`
- `ACTION-SCALE`
- `UNSUPPORTED-ADDITION`

## Promotion interpretation
A clean pass supports a narrow rule family only:
`FUNCTIONAL BREVITY PRESERVED / EXCHANGE-LEVEL TERSE SATURATION REPAIRED / NO LENGTH QUOTA`.

It does not justify universal claims about all Vietnamese dialogue, all dialects, or historical speech.