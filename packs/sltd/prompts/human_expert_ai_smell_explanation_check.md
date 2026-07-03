# SLTD Human Expert AI-Smell Explanation Check

Use this prompt when the user asks why a passage reads AI-like, synthetic, over-clean, same-voiced, formulaic, detector-like, or not human.

This is an explanation discipline, not an AI detector. It does not classify authorship and does not output AI probability.

## Read first

```text
manifest.yml
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
prompts/source_surface_check.md when exact prose/span is being judged
rules/sltd_multilingual_long_context_retrieval_oneruler_discipline.md if the claim depends on repeated patterns or absence across long source
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
rules/sltd_narrative_claim_verification_clipper_discipline.md if the smell claim depends on factual/status/canon/continuity evidence
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md if story-decision AI smell may be root cause
rules/sltd_character_voice_dialogue_relationship_location_gate.md if dialogue, voice, relationship, silence, or staging is in scope
rules/sltd_author_writing_sheet_claim_evidence_discipline.md if author-style evidence controls the explanation
rules/sltd_author_voice_fingerprint_ghostwriter_discipline.md if author voice match is in scope
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md if exact Vietnamese surface is in scope
rules/sltd_human_surface_polish_anti_synthetic_gate.md if correct-but-synthetic surface repair is in scope
rules/sltd_human_expert_ai_smell_explanation_discipline.md
```

## Source requirement

Read the exact span or user-provided excerpt before explaining why prose reads synthetic.

If source/span is missing, return:

```text
AI_SMELL_EXPLANATION_NEEDS_SPAN
```

If current source is required but unread, return:

```text
AI_SMELL_EXPLANATION_NEEDS_SOURCE
```

## Output

```text
SLTD HUMAN EXPERT AI-SMELL EXPLANATION CHECK
SCOPE:
SOURCE USED:
SOURCE STATUS:
OUTPUT / SPAN USED:
SPAN:
AI-SMELL CLAIM:
EXPLANATION DIMENSION:
WHY IT READS SYNTHETIC:
FALSE POSITIVE RISK:
SOURCE / CANON RISK:
VOICE / CHARACTER RISK:
STRUCTURAL ROOT CAUSE: YES / NO / UNCERTAIN
SURFACE-ONLY REPAIR SAFE: YES / NO / UNCERTAIN
REPAIR DIRECTION:
DO NOT DO:
VERDICT: EXPLAINED / PARTIAL / BLOCKED
BLOCKERS:
NEXT NODE:
```

## Rules

- No AI-probability scoring.
- No authorship accusation.
- No keyword-only verdict.
- No English detector heuristic as Vietnamese prose law.
- No surface polish before separating source, canon, story, voice, author-style, and surface blockers.
- Every smell claim needs span + reason + false-positive risk + repair direction.
- If story-decision smell is root cause, hand off to Narrative Feature Audit.
- If dialogue or character voice is root cause, hand off to Character Voice / Dialogue / Staging.
- If correct-but-synthetic surface is root cause and source-safe, hand off to Human Surface Polish.
- If exact Vietnamese friction is root cause, hand off to Vietnamese Senior Editor Surface.

## Minimal output

```text
AI-SMELL EXPLANATION BRIEF
SCOPE:
SPAN:
WHY IT READS SYNTHETIC:
FALSE POSITIVE RISK:
ROOT CAUSE: SURFACE / STRUCTURE / VOICE / STYLE / SOURCE / UNCERTAIN
REPAIR DIRECTION:
DO NOT DO:
NEXT NODE:
```

## Source gap output

```text
AI-SMELL SOURCE GAP
REQUEST:
SPAN NEEDED:
SOURCE NEEDED:
WHY NEEDED:
SAFE CLAIM NOW:
NEXT NODE:
```