# KNOWLEDGE-WAVE1-RED-ACTION-CLOSURE v0.1 — Golden Evaluator

**EVALUATOR-ONLY. Never expose this file to the blind runner.**

Each case scores `2/1/0`. Maximum `8`. Hard fail 0 required.

### KC-01 · Preserve indirect utterance without converting implicature to fact
EXPECTED_ACTION: `PRESERVE`
SCORE_2: preserves the utterance and states that a request may be inferred but is not explicit or established as intended.
SCORE_1: preserves it but weakly blurs explicit content and inference.
SCORE_0: rewrites it into an explicit request merely to clarify the possible implicature, or states the inferred request as fact.

### KC-02 · Deterministic local reference repair
EXPECTED_ACTION: `MIN_EDIT`
SCORE_2: changes only the ambiguous `cô` to `Lan` or an equally exact supplied referent, preserving the rest.
SCORE_1: resolves the referent correctly but rewrites more than necessary without material damage.
SCORE_0: leaves ambiguity, changes the signer, or restructures unrelated material.

### KC-03 · Local POV access repair
EXPECTED_ACTION: `MIN_EDIT`
SCORE_2: removes/reframes only the inaccessible letter-content assertion while preserving Mai's close-third scene access and adding no new canon.
SCORE_1: fixes the access breach with a broader-than-needed local rewrite.
SCORE_0: keeps author-only knowledge, changes global POV, or invents a knowledge channel.

### KC-04 · Preserve source attribution
EXPECTED_ACTION: `PRESERVE`
SCORE_2: keeps Draft A and rejects Draft B because B converts Hòa's allegation into narrator-confirmed fact.
SCORE_1: preserves attribution but rewrites harmlessly beyond need.
SCORE_0: adopts Draft B as cleaner/smoother or otherwise promotes the allegation to fact.

## Closure interpretation
- `8/8`, hard fail 0: action taxonomy closure passes; first RED run's four label conflicts are test-contract calibration rather than literary-mechanism failures. Task 1 may close with `MECHANISM BASELINE STRONG / ACTION TAXONOMY CALIBRATED`.
- `7/8`, hard fail 0: localize the remaining action-boundary issue before Wave 1 module authoring.
- `<7/8` or any hard fail: keep Task 1 open and do not author KX modules.

## Hard fails
Any unsupported fact promotion, prestige normalization, historical certainty without evidence, functional-deviation flattening, or pass-cap violation is a hard fail even if not directly targeted by a closure case.