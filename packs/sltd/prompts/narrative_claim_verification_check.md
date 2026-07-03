# SLTD Narrative Claim Verification Check

Use this prompt when a claim about SLTD status, canon, continuity, POV knowledge, object state, reveal timing, readiness, or lock needs evidence-backed verification.

This adapts CLIPPER-style claim verification for editorial source discipline. It is not a dataset-generation prompt and not a readiness pass.

## Read first

```text
manifest.yml
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
rules/sltd_tracking_logic_ledger_traceability_gate.md if state, object, debt, residue, thread, claim anchor, or downstream risk is affected
rules/sltd_narrative_claim_verification_clipper_discipline.md
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md if the claim concerns story-decision AI smell or structural idiosyncrasy
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md if Human Chapter Pass, Publication Lock, or exact Vietnamese surface is in scope
```

## Source requirement

Use compressed source only to locate evidence.

Before final TRUE/FALSE verdict, read current Notion source or the user-provided current packet that directly supports the claim.

If source is missing, return:

```text
CLAIM_UNCERTAIN_SOURCE_NEEDED
```

If exact wording matters, read exact scene/chapter surface before verdict.

## Output

```text
SLTD NARRATIVE CLAIM VERIFICATION
SCOPE:
SOURCE USED:
SOURCE STATUS:
COMPRESSED SOURCE USED:
CLAIM:
CLAIM TYPE:
TRUE / FALSE / UNCERTAIN:
EVIDENCE:
COUNTERCLAIM / FALSE TWIN:
CHAPTER / SCENE ANCHOR:
LOW-LEVEL DETAIL RISK:
MISATTRIBUTION RISK:
CANON / CONTINUITY IMPACT:
VERDICT:
PROSE / READINESS PERMISSION:
NEXT NODE:
```

## Rules

- Do not guess when evidence is missing.
- Do not use chat memory as current source.
- Do not use old Workdeck/raw draft as current source unless named current.
- Do not let a summary/capsule/chapter outline substitute for exact source when exact source is required.
- Build a false twin when the claim is easy to agree with lazily.
- Separate TRUE/FALSE/UNCERTAIN from readiness and publication lock.
- Do not call Human Chapter Pass, readiness, or Publication Lock from claim verification alone.

## Minimal output

For a simple claim:

```text
CLAIM:
VERDICT: TRUE / FALSE / UNCERTAIN
EVIDENCE:
FALSE TWIN:
RISK:
NEXT NODE:
```

## Source gap output

```text
CLAIM VERIFICATION SOURCE GAP
SCOPE:
CLAIM:
SOURCE NEEDED:
WHY NEEDED:
SAFE CLAIM NOW:
NEXT NODE:
```