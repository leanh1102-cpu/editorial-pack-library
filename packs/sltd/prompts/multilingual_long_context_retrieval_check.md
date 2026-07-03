# SLTD Multilingual Long-Context Source Retrieval Check

Use this prompt when a task depends on finding, not finding, or aggregating evidence across long Vietnamese source.

This is a OneRuler-style retrieval and absence discipline. It is not canon authority, readiness, Publication Lock, or rewrite permission.

## Read first

```text
manifest.yml
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, reveal timing, or long-range continuity is in scope
rules/sltd_multilingual_long_context_retrieval_oneruler_discipline.md
rules/sltd_narrative_claim_verification_clipper_discipline.md if retrieval result becomes a TRUE/FALSE/UNCERTAIN claim
rules/sltd_corpus_topic_thread_discovery_topicgpt_discipline.md if retrieval result feeds topic/thread assignment
rules/sltd_reference_anchored_longform_quality_polaris_discipline.md if retrieval result controls source preservation or longform quality
rules/sltd_tracking_logic_ledger_traceability_gate.md if retrieval target involves object/thread/state/payoff debt
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md if exact Vietnamese surface or status field is in scope
```

## Source requirement

Read current source or the user-provided source packet when the user asks current/latest/Notion/current manuscript/lock/readiness/Human Chapter Pass/Publication Lock/canon conflict/status field, or when the answer requires a current absence claim.

If source is missing, return:

```text
LONG_CONTEXT_RETRIEVAL_NEEDS_SOURCE
```

If scope is missing, return:

```text
LONG_CONTEXT_RETRIEVAL_NEEDS_SCOPE
```

If target is missing, return:

```text
LONG_CONTEXT_RETRIEVAL_NEEDS_TARGET
```

## Output

```text
SLTD MULTILINGUAL LONG-CONTEXT SOURCE RETRIEVAL CHECK
SCOPE:
SOURCE USED:
SOURCE STATUS:
SOURCE LANGUAGE:
INSTRUCTION LANGUAGE:
CONTEXT LENGTH TIER:
RETRIEVAL TARGET:
TARGET TYPE: EXACT PHRASE / CANON CLAIM / STATUS FIELD / OBJECT STATE / POV KNOWLEDGE / RELATIONSHIP MEMORY / THREAD / MOTIF / REVEAL / FORESHADOWING / VOICE PATTERN / AI-SMELL PATTERN / ABSENCE CLAIM / AGGREGATION
SOURCE SEGMENTS CHECKED:
EVIDENCE ANCHORS:
FOUND:
NOT FOUND:
UNCERTAIN:
ABSENCE CLAIM STATUS: ALLOWED / NOT ALLOWED / UNCERTAIN
AGGREGATION REQUIRED: YES / NO
AGGREGATION METHOD:
CROSS-LINGUAL RISK:
TOKENIZATION / LENGTH RISK:
VERDICT: FOUND / NOT FOUND / UNCERTAIN / BLOCKED
BLOCKERS:
NEXT NODE:
```

## Rules

- No absence claim without source check.
- No not-found verdict from compressed source alone.
- No aggregation verdict from memory.
- No current-status verdict without current Notion/source.
- No English summary replacing Vietnamese source.
- Split source by scene/chapter/packet/arc/part/source node when scope is too large.
- Return FOUND, NOT FOUND, and UNCERTAIN separately.
- If retrieval result becomes a canon/status/readiness claim, hand off to Narrative Claim Verification.
- If retrieval result becomes topic/thread map evidence, hand off to Corpus Topic / Thread Discovery.
- If retrieval result affects source preservation in a long draft, hand off to Reference-Anchored Longform Story Quality.

## Minimal output

```text
LONG-CONTEXT RETRIEVAL BRIEF
SCOPE:
SOURCE USED:
TARGET:
SEGMENTS CHECKED:
FOUND WITH ANCHOR:
NOT FOUND STATUS:
UNCERTAIN:
ABSENCE CLAIM ALLOWED: YES / NO / UNCERTAIN
NEXT NODE:
```

## Source gap output

```text
LONG-CONTEXT RETRIEVAL SOURCE GAP
SCOPE:
REQUEST:
SOURCE NEEDED:
TARGET NEEDED:
WHY NEEDED:
SAFE CLAIM NOW:
NEXT NODE:
```