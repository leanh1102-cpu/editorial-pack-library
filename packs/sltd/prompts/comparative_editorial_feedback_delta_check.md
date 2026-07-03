# SLTD Comparative Editorial Feedback Delta Check

Use this prompt when user/editor feedback must be converted into a bounded revision delta before rewrite, polish, review, or readiness work.

This is a feedback-translation discipline. It is not a rewrite role by itself and does not grant readiness or Publication Lock.

## Read first

```text
manifest.yml
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
prompts/source_surface_check.md when exact span/current output is being judged
rules/sltd_multilingual_long_context_retrieval_oneruler_discipline.md if feedback depends on finding repeated or missing evidence across long source
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, reveal timing, or long-range continuity is in scope
rules/sltd_human_expert_ai_smell_explanation_discipline.md if feedback concerns synthetic reader effect or AI-smell
rules/sltd_narrative_claim_verification_clipper_discipline.md if feedback depends on factual/status/canon/continuity evidence
rules/sltd_multi_constraint_instruction_ledger_suri_discipline.md if feedback creates several controlling constraints
rules/sltd_comparative_editorial_feedback_delta_discipline.md
```

## Source requirement

If feedback touches source/canon/POV/reveal/status, read current source or the user-provided packet before converting it into rewrite permission.

If scope is missing, return:

```text
FEEDBACK_DELTA_NEEDS_SCOPE
```

If target span/scene is missing, return:

```text
FEEDBACK_DELTA_NEEDS_TARGET
```

If source is required but missing, return:

```text
FEEDBACK_DELTA_NEEDS_SOURCE
```

## Output

```text
SLTD COMPARATIVE EDITORIAL FEEDBACK DELTA CHECK
SCOPE:
SOURCE USED:
SOURCE STATUS:
FEEDBACK USED:
TARGET SPAN / SCENE / CHAPTER:
FEEDBACK TYPE: INCREASE / DECREASE / PRESERVE / PROHIBIT / COMPARE / REPAIR / MIXED
INCREASE:
DECREASE:
PRESERVE:
PROHIBIT:
COMPARE AGAINST:
IMPLICIT PREFERENCE:
SOURCE / CANON LIMIT:
POV / REVEAL LIMIT:
VOICE / CHARACTER LIMIT:
STYLE / SURFACE LIMIT:
READER EFFECT TARGET:
REVISION TEST:
REWRITE / POLISH PERMISSION: YES / NO / CANDIDATE_ONLY
BLOCKERS:
NEXT NODE:
```

## Rules

- No feedback delta without target scope.
- No rewrite from vague preference.
- No converting author feedback into generic style law.
- No changing canon, POV, reveal timing, scene outcome, or current status to satisfy a preference.
- No `better` without saying better along which dimension.
- No polish before separating increase, decrease, preserve, and prohibit.
- If feedback concerns AI-smell, run Human Expert AI-Smell Explanation before repair when span-based cause is unclear.
- If feedback creates multiple constraints, run Multi-Constraint Ledger before drafting.
- If feedback depends on current source, run Source Surface / Context Capsule first.

## Minimal output

```text
FEEDBACK DELTA BRIEF
SCOPE:
FEEDBACK:
TARGET:
INCREASE:
DECREASE:
PRESERVE:
PROHIBIT:
READER EFFECT TARGET:
REVISION TEST:
NEXT NODE:
```

## Source gap output

```text
FEEDBACK DELTA SOURCE GAP
REQUEST:
FEEDBACK USED:
SCOPE NEEDED:
TARGET NEEDED:
SOURCE NEEDED:
WHY NEEDED:
SAFE CLAIM NOW:
NEXT NODE:
```