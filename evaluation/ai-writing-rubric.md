# AI Writing Rubric

Evaluate correction and preservation separately. Numeric scores are diagnostic, not absolute literary quality.

Core longitudinal metrics:
- `CORRECTION_PRECISION`: how often a real problem is repaired without missing its mechanism.
- `PRESERVATION_PRECISION`: how often intentional voice/register/form/ambiguity/rhythm/etc. survives intervention.
- `CONTEXTUAL_JUDGMENT`: whether action strength matches evidence and local function.
- `REGRESSION_RATE`: how often revision creates a new material failure or damages a protected dimension.

Task-specific diagnostic when dialogue is materially involved:
- `DIALOGUE_TEXTURE`: whether adjacent turns preserve functional variation, speaker differentiation, relation/status signals, and pressure-sensitive recovery without imposing a verbosity quota or flattening stable dialect/idiolect.

For `DIALOGUE_TEXTURE`, judge the exchange as well as individual turns. A short sentence is not a defect by length alone. Many short turns are also not automatically a defect. Flag terse saturation only when accumulation materially removes relation, voice differentiation, contextual/emotional shading, or plausible recovery after pressure changes.

A dialogue repair should prefer the smallest useful intervention: preserve functional clipped turns, restore only the missing relational or syntactic variation, and do not manufacture particles, dialect markers, kinship terms, motives, or emotional certainty unsupported by the supplied context.

Hard-fail families include fabricated source/canon/evidence, claim→fact collapse, author-only knowledge granted to characters, destruction of marked voice/register/form, forced resolution of deliberate ambiguity/mystery, generic same-voice flattening, universal dialogue-length quotas, or CLEAN output leaking benchmark/evaluator commentary.

A candidate repair may improve correction only if preservation, epistemic uncertainty, voice/register variance, reader inference, and — when relevant — dialogue texture do not deteriorate.
