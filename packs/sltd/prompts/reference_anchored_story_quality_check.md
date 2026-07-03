# SLTD Reference-Anchored Story Quality Check

Use this prompt for long rewrite, chapter assembly, packet candidate, author-aligned draft, or readiness-risk quality stress testing.

This is a POLARIS-style longform story quality check. It is not RL training, not a detector, not Human Chapter Pass, and not Publication Lock.

## Read first

```text
manifest.yml
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
rules/sltd_narrative_claim_verification_clipper_discipline.md if a quality claim depends on status/canon/continuity evidence
rules/sltd_multi_constraint_instruction_ledger_suri_discipline.md if output constraints control the draft
rules/sltd_editorial_harm_anticipation_aha_vignette_matrix.md if false quality/readiness harm is in scope
rules/sltd_corpus_topic_thread_discovery_topicgpt_discipline.md if packet/arc map-level quality is in scope
rules/sltd_reference_anchored_longform_quality_polaris_discipline.md
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md if structural AI smell or narrative diversity is in scope
rules/sltd_human_surface_polish_anti_synthetic_gate.md if correct-but-synthetic surface is in scope
```

## Source requirement

Read current source or the user-provided current packet before making quality claims about source fidelity, scene function, Must Show, reveal lock, character voice, readiness, or exact output.

If source is missing, return:

```text
LONGFORM_QUALITY_NEEDS_SOURCE
```

If output is missing, return:

```text
LONGFORM_QUALITY_NEEDS_OUTPUT
```

## Output

```text
SLTD REFERENCE-ANCHORED LONGFORM STORY QUALITY CHECK
SCOPE:
SOURCE USED:
SOURCE STATUS:
OUTPUT TYPE: SCENE / CHAPTER / PACKET / DRAFT / REWRITE
TARGET LENGTH:
ACTUAL LENGTH:
REFERENCE / ANCHOR USED:
ANCHOR STATUS:
POSITIVE DIMENSIONS:
- PROMPT / SCENE FUNCTION FULFILLMENT:
- SCENE REALIZATION:
- NARRATIVE ARC / PACING:
- CHARACTER DEPTH / AGENCY:
- VOICE / STYLE DISTINCTIVENESS:
- THEMATIC / EMOTIONAL PRESSURE:
- READER EFFECT:
NEGATIVE DIMENSIONS:
- SOURCE / PROMPT VIOLATION:
- COHERENCE / POV BREAK:
- GENERIC LANGUAGE:
- OVER-SUMMARY:
- OVER-EXPLANATION:
- DRIFT / BLOAT:
- DIALOGUE PROBLEM:
- PREDICTABILITY / CLICHE:
- OVERWROUGHT PROSE:
- LOCAL CONTRADICTION:
- LATE-OUTPUT COLLAPSE:
LENGTH ADHERENCE:
MUST SHOW PRESERVATION:
LOCAL COHERENCE CHECK:
QUALITY VERDICT: PASS / PARTIAL / FAIL / BLOCKED
DRAFT / REWRITE PERMISSION:
BLOCKERS:
NEXT NODE:
```

## Rules

- No story-quality score without source.
- No length reward if Must Show is cut.
- No reference anchor unless user-approved/current.
- Do not use legacy drafts, generated text, or chat memory as quality anchor unless explicitly approved.
- Do not train, fine-tune, scrape, or copy protected reference text.
- Do not use longform quality verdict as Human Chapter Pass, readiness, or Publication Lock.
- If quality depends on disputed source/canon/status, hand off to Narrative Claim Verification.
- If output must preserve several constraints, hand off to Multi-Constraint Ledger.
- If quality failure would create false readiness or downstream harm, hand off to Editorial Harm Anticipation.
- If quality issue is structural AI smell, hand off to Narrative Feature Audit.
- If quality issue is correct-but-synthetic surface, hand off to Human Surface Polish only after source/story constraints are clear.

## Minimal output

For quick checks:

```text
LONGFORM QUALITY BRIEF
SCOPE:
SOURCE USED:
OUTPUT USED:
TARGET / ACTUAL LENGTH:
TOP POSITIVE QUALITY:
TOP QUALITY FAILURES:
MUST SHOW PRESERVED: YES / NO / UNCERTAIN
QUALITY VERDICT:
NEXT NODE:
```

## Source gap output

```text
LONGFORM QUALITY SOURCE GAP
SCOPE:
REQUEST:
SOURCE NEEDED:
OUTPUT NEEDED:
WHY NEEDED:
SAFE QUALITY CLAIM NOW:
NEXT NODE:
```