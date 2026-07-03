# SLTD Editorial Harm Anticipation Check

Use this prompt for REDTEAM, PREMORTEM, readiness risk, packet risk, lock risk, or high-risk rewrite planning.

This is an AHA-style vignette matrix. It is not a prose repair pass and not a readiness pass.

## Read first

```text
manifest.yml
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
rules/sltd_narrative_claim_verification_clipper_discipline.md if a harm depends on status/canon/continuity evidence
rules/sltd_multi_constraint_instruction_ledger_suri_discipline.md if constraints control output
rules/sltd_editorial_harm_anticipation_aha_vignette_matrix.md
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md if structural AI smell may cause harm
rules/sltd_human_surface_polish_anti_synthetic_gate.md if over-polish or human surface harm is in scope
```

## Source requirement

Read current source or the user-provided current packet before making harm claims about current status, readiness, lock, canon, reveal, or exact scene function.

If source is missing, return:

```text
EDITORIAL_HARM_MATRIX_NEEDS_SOURCE
```

## Output

```text
SLTD EDITORIAL HARM ANTICIPATION MATRIX
SCOPE:
SOURCE USED:
SOURCE STATUS:
TASK TYPE:
MATRIX MODE: UPFRONT / SECONDARY-CHECK
IMPACT TARGETS:
EDITORIAL FAILURE BEHAVIORS:
VIGNETTES:
- TARGET:
  FAILURE BEHAVIOR:
  FAILURE VIGNETTE:
  LIKELY HARM:
  SOURCE / CONSTRAINT ANCHOR:
  SEVERITY: LOW / MEDIUM / HIGH / CRITICAL
  DETECTABILITY: EASY / MODERATE / HARD
  REPAIR / PREVENTION:
BLOCKERS:
ROUTE DECISION:
NEXT NODE:
```

## Rules

- No harm matrix without scope.
- Do not invent canon as a harm vignette.
- Do not use generic AI safety harms when the task needs SLTD editorial harms.
- Do not call Human Chapter Pass, readiness, or Publication Lock from this prompt.
- Use top 3 harms by severity when the matrix would become too large.
- If the harm depends on an unverified claim, hand off to Narrative Claim Verification.
- If the harm depends on multiple constraints, hand off to Multi-Constraint Ledger.
- If the harm is structural AI smell, hand off to Narrative Feature Audit.
- If the harm is over-polish, hand off to Human Surface Polish only after earlier blockers are clear.

## Minimal output

For small tasks:

```text
TOP 3 EDITORIAL HARMS
SCOPE:
SOURCE USED:
1.
2.
3.
HIGHEST-RISK ROUTE:
NEXT NODE:
```

## Source gap output

```text
EDITORIAL HARM SOURCE GAP
SCOPE:
REQUEST:
SOURCE NEEDED:
WHY NEEDED:
SAFE HARM CLAIM NOW:
NEXT NODE:
```