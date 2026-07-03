# SLTD Human Expert AI-Smell Explanation Discipline

This rule adapts human-expert AI-generated-text detection research for SLTD editorial work.

It does not classify authorship. It explains why a passage reads synthetic, detector-like, over-clean, same-voiced, formulaic, outline-labeled, or AI-shaped to an experienced human reader.

## Core rule

No AI-probability scoring.

No keyword-only verdict.

Every AI-smell claim needs a span, reason, false-positive risk, and repair direction.

This is an explanation and repair-routing discipline. It is not an AI detector, not source authority, not canon authority, not rewrite permission, not Human Chapter Pass, not readiness, and not Publication Lock.

## Use when

- the user says prose sounds AI-like, synthetic, over-clean, same-voiced, detector-like, generic, over-formal, too smooth, or not human;
- Vietnamese surface is technically correct but still feels fake, thin, or over-managed;
- characters speak in the same register or dialogue lacks interruption, pressure, silence, or relationship memory;
- prose exposes outline labels, theme labels, symbol labels, or abstract explanation instead of scene pressure;
- anti-AI composite, Vietnamese senior editor surface, human surface polish, narrative feature audit, or author voice comparison needs a human-reader explanation;
- the task needs repair direction without turning the result into detector scoring.

## Authority

Run after:

```text
source preflight
source surface when exact prose is being judged
multilingual long-context retrieval when the AI-smell claim depends on finding repeated patterns or absence across long source
context capsule when current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
narrative claim verification when the AI-smell claim depends on a factual/status/canon/continuity claim
narrative feature audit when story-decision AI smell may be the root cause
Vietnamese senior editor surface when exact Vietnamese surface is the judged layer
human surface polish when repair is local and source-safe
```

Run before:

```text
copyedit
proofread
readiness / Publication Lock claim
large surface rewrite acceptance
```

## Required distinction

```text
AI-SMELL EXPLANATION = why a span reads synthetic to an experienced reader
AUTHORSHIP CLAIM = claim that a human or model wrote the text
DETECTOR SCORE = probability or classifier-like label
SURFACE SMELL = line/register/rhythm/generic phrasing issue
STRUCTURAL SMELL = story-decision pattern such as tidy causality, overexplained theme, weak reveal, or decorative sensory pressure
VOICE SMELL = same-voiced dialogue or character register mismatch
STYLE-OVER-CHARACTER SMELL = author-like or polished prose flattening character pressure
FALSE POSITIVE RISK = reason the smell may be intentional, genre-typical, translated-source residue, character-specific, or source-required
REPAIR DIRECTION = next safe editorial route, not automatic rewrite
```

Do not collapse synthetic-feeling prose into an authorship verdict.

## Explanation dimensions

Assess with evidence from the span:

```text
FORMALITY / REGISTER MISMATCH
GENERIC LANGUAGE / STOCK PHRASE
OUTLINE LABEL VISIBLE ON PAGE
THEME OR SYMBOL EXPLAINED TOO EARLY
TOO-SMOOTH TRANSITION
SAME-VOICE DIALOGUE
OVER-SUMMARY
OVER-EXPLANATION
CLARITY WITHOUT PRESSURE
OBJECT / BODY DETAIL WITHOUT CONSEQUENCE
PREDICTABLE RHETORIC
LOCAL COHERENCE OR POV STRAIN
AUTHOR-VOICE OVER CHARACTER-VOICE
```

## Output schema

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

- Do not output AI percentage, detector score, or classifier confidence.
- Do not accuse the author or passage of being AI-generated.
- Do not decide from keywords alone.
- Do not use English detector heuristics as Vietnamese prose law.
- Do not polish before separating source, canon, story, voice, and surface blockers.
- Do not erase roughness that belongs to character, region, age, class, fatigue, fear, grief, or scene pressure.
- Do not replace Vietnamese rhythm with generic literary smoothness.
- Do not turn author taste into repeated phrase templates.

## False-positive risk checklist

Before repair, ask whether the suspicious span may be:

- intentionally formal because of narrator distance, ritual, official speech, or class/register;
- repetitive because the character is frightened, evasive, young, old, or hiding knowledge;
- abstract because source packet requires withheld reveal;
- smooth because the scene is transition-only and no pressure is intended;
- flat because current source lacks scene function rather than surface polish;
- familiar because webnovel convention is being used deliberately.

If false-positive risk is high, mark `SURFACE-ONLY REPAIR SAFE: NO / UNCERTAIN`.

## Repair routing

```text
story-decision smell -> narrative_feature_audit
same-voice dialogue -> character_voice_dialogue_staging_check
style-over-character -> author_writing_sheet_check or author_voice_fingerprint_check plus voice/staging
correct but synthetic surface -> human_surface_polish_pass
exact Vietnamese friction -> vietnamese_senior_editor_surface_check
claim depends on source/status/canon -> narrative_claim_verification_check
pattern claim across packet -> multilingual_long_context_retrieval_check before verdict
long draft bloat or late collapse -> reference_anchored_story_quality_check
```

## Blockers

```text
source missing
exact span missing
scope missing
current source required but unread
AI-smell claim has no span
keyword-only verdict
authorship claim requested instead of reader-effect explanation
surface repair would hide story-decision smell
voice repair would overwrite character voice
source/canon/status claim unverified
false-positive risk not checked
```

## Failure labels

```text
AI_SMELL_EXPLAINED
AI_SMELL_PARTIAL
AI_SMELL_BLOCKED
NO_AI_PROBABILITY_SCORING
KEYWORD_ONLY_VERDICT_BLOCKED
SPAN_REQUIRED
FALSE_POSITIVE_RISK_UNCHECKED
STRUCTURAL_SMELL_HANDOFF
VOICE_SMELL_HANDOFF
HUMAN_SURFACE_HANDOFF
VIETNAMESE_SURFACE_HANDOFF
AUTHORSHIP_CLAIM_NOT_ALLOWED
```

## Safe repair

Safe repair may:

- quote or point to the suspicious span;
- explain reader effect and cause;
- separate surface, structure, voice, author-style, source, and canon causes;
- identify false-positive risk;
- recommend the next editorial route;
- propose limited OLD/NEW repair only when source-safe and requested.

Safe repair must not:

- score AI probability;
- accuse authorship;
- rewrite without source and permission;
- remove source-required repetition, silence, roughness, or withholding;
- use humanization as detector bypass;
- create scripts, workflows, reports, issues, boards, databases, automations, or live manuscript copies.

## Output labels

```text
AI_SMELL_EXPLANATION_READY
AI_SMELL_EXPLANATION_NEEDS_SOURCE
AI_SMELL_EXPLANATION_NEEDS_SPAN
AI_SMELL_EXPLANATION_BLOCKED
NARRATIVE_FEATURE_HANDOFF
CHARACTER_VOICE_HANDOFF
HUMAN_SURFACE_HANDOFF
VIETNAMESE_SURFACE_HANDOFF
NO_DETECTOR_SCORE
```