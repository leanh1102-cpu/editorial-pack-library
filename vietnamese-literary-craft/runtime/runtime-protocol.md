# Runtime Protocol

`TASK → CLASSIFY → DIAGNOSE → DECIDE → EXECUTE → PRESERVATION CHECK → STOP`

## TASK
Read the literal request and supplied source. Do not silently broaden scope.

## CLASSIFY
Identify only dimensions that materially affect the task: form/genre, register/historical layer, POV/speech condition, epistemic status, intentional deviation vs probable error, local pressure/function. If a necessary classification lacks evidence, do not guess.

## DIAGNOSE
Name a concrete failure mechanism supported by the text, or `NO MATERIAL FAILURE`. Frequency, smoothness, modernity, explicitness, or rule conformity alone are not evidence of failure.

## DECIDE
Choose exactly one:
- `PRESERVE` — no material failure, or intervention would damage function.
- `MIN_EDIT` — local repair without changing larger structure/voice/register/uncertainty/pressure.
- `REVISE` — structural craft problem supported by evidence.
- `HOLD-INSUFFICIENT_EVIDENCE` — responsible judgment requires missing source/context/form/canon/verification.

The action labels describe the disposition of the **requested task**, not only whether source text changes.

Use `PRESERVE` when the supplied evidence is sufficient to judge that the material should remain unchanged or that the proposed intervention would damage an established function.

Use `HOLD-INSUFFICIENT_EVIDENCE` when the literal request itself requires an unsupported determination, certainty, motive, future state, canon fact, or verification. In that case the safest textual handling may still be to leave the source untouched, but `LEAVE TEXT UNCHANGED` does not convert an evidence-blocked task into `PRESERVE`.

Use the smallest action that solves the demonstrated problem. A defect confined to one sentence is `MIN_EDIT` when the surrounding structure already works; do not label it `REVISE` merely because the wording changes substantially inside that sentence.

## EXECUTE
Apply only the chosen action. Do not use an edit as permission to add canon, explanatory recap, ornamental imagery, standardized voice, or generic transitions.

## PRESERVATION CHECK
When relevant, protect meaning/factual status, voice/direct thought, form/register, productive ambiguity, reader inference, pressure-shaped rhythm, functional repetition, causal debt, deliberate roughness/asymmetry/telling/latency/unreliability. Reject an edit whose regression is larger than the original problem.

## Narrow stable note: SENSORY-MEDIATION v0.1
For sentence-level bodily sensation, check whether redundant perception/nominalization/causal packaging such as `cảm thấy`, `một cảm giác`, `một luồng`, or `khiến...` remains. If lexical cleanup still leaves a generic unsupported propagation pattern such as `lạnh/buốt/nóng lan/len lỏi khắp người/cơ thể`, remove that unsupported propagation. Then use only one of the following, in priority order:
1. a concrete contact/body response already supplied by the packet;
2. an equally direct non-mediated sensation bounded to facts already supplied;
3. `HOLD-INSUFFICIENT_EVIDENCE` only when the literal task specifically requires a bodily/contact realization the packet does not support.

Do not invent a body site, garment, wetness, contact point, posture, movement, reflex, or other sensory fact merely to make the line more concrete. Treat the target sentence as material under repair: wording such as `len lỏi trong cơ thể`, `lan khắp người`, or similar body-wide propagation inside that defective sentence is not independent evidence that the whole-body effect is true. Preserve it only when surrounding packet evidence independently establishes it.

Do not apply this note when abstraction, metaphor, distortion, direct thought, register, or surrounding context already supplies the intended function/grounding.

## STOP
Stop once the demonstrated failure is repaired and preservation checks pass. No polish for polish's sake.
