# SLTD Entry Fast Path

Use this file to choose the smallest SLTD route.

## Always read

```text
manifest.yml
DESIGN.md
PACK.md
AGENT_IDENTITY.md
rules/sltd_runtime_loop.md
rules/sltd_source_preflight.md
rules/sltd_decision_safety.md
```

## Pipeline order

```text
0. Source Preflight
1. Context Capsule
2. Narrative Claim Verification when status/canon/continuity/lock claim is in scope
3. Multi-Constraint Instruction Ledger when rewrite/audit/readiness has multiple controlling constraints
4. Editorial Harm Anticipation when REDTEAM/PREMORTEM/readiness/lock/large-rewrite harm risk is in scope
5. Corpus Topic / Thread Discovery when packet/arc/series map-level navigation is in scope
6. Reference-Anchored Longform Story Quality when long rewrite/chapter/packet quality across length is in scope
7. Spine Lock
8. Tracking / Logic Ledger
9. Borderbound
10. Life-Task Bound
11. Story Movement
12. Scene-First Prose Judgment
13. Narrative Feature / Structural Idiosyncrasy Audit when story-decision AI smell is in scope
14. Voice / Dialogue / Staging
15. Author Writing Sheet when claim-evidence style memory is in scope
16. Author Voice Fingerprint when author style matching is in scope
17. Draft / Rewrite / Author-Aligned Draft
18. Line / Voice / Rhythm
19. Human Surface Polish
20. Composite Risk Check
21. Feedback Matrix / Report
22. Seam / Chapter Assembly
23. Readiness / Lock
```

Do not run later gears to hide failure in earlier gears. Stop at the first real blocker.

## Fast paths

### Reference-anchored longform story quality / POLARIS discipline

```text
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
source_surface_check when exact prose/output is being judged
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
rules/sltd_narrative_claim_verification_clipper_discipline.md if a quality claim depends on factual/status/canon evidence
rules/sltd_multi_constraint_instruction_ledger_suri_discipline.md if output constraints control the draft
rules/sltd_editorial_harm_anticipation_aha_vignette_matrix.md if false quality/readiness harm is in scope
rules/sltd_corpus_topic_thread_discovery_topicgpt_discipline.md if packet/arc map-level quality is in scope
rules/sltd_reference_anchored_longform_quality_polaris_discipline.md
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md if structural AI smell or narrative diversity is in scope
rules/sltd_human_surface_polish_anti_synthetic_gate.md if correct-but-synthetic surface is in scope
prompts/reference_anchored_story_quality_check.md
prompts/node_checkpoint.md
```

### Corpus topic / thread discovery map

```text
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, reveal timing, or long-range continuity is in scope
rules/sltd_corpus_topic_thread_discovery_topicgpt_discipline.md
rules/sltd_narrative_claim_verification_clipper_discipline.md if topic assignment depends on factual/status/canon evidence
rules/sltd_tracking_logic_ledger_traceability_gate.md if thread state, object state, or payoff debt is in scope
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md if repeated structural AI smell, narrative diversity, or thematic drift is in scope
rules/sltd_editorial_harm_anticipation_aha_vignette_matrix.md if topic/thread drift creates downstream harm
rules/sltd_reference_anchored_longform_quality_polaris_discipline.md if packet/arc output quality across length is in scope
prompts/corpus_topic_thread_discovery_check.md
prompts/node_checkpoint.md
```

### Context capsule / lore retrieval discipline

```text
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_context_capsule_lore_retrieval_discipline.md
rules/sltd_narrative_claim_verification_clipper_discipline.md if current status, canon, continuity, readiness, lock, or source conflict claim is in scope
rules/sltd_multi_constraint_instruction_ledger_suri_discipline.md if rewrite/audit/readiness has multiple controlling constraints
rules/sltd_editorial_harm_anticipation_aha_vignette_matrix.md if REDTEAM/PREMORTEM/readiness/lock/large rewrite harm risk is in scope
rules/sltd_corpus_topic_thread_discovery_topicgpt_discipline.md if packet/arc/series map-level navigation is in scope
rules/sltd_reference_anchored_longform_quality_polaris_discipline.md if long rewrite/chapter/packet quality across length is in scope
rules/sltd_tracking_logic_ledger_traceability_gate.md if state, knowledge, object, residue, thread, pass trace, or downstream risk is affected
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if scene function, chapter card, scene packet, or border is unclear
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md if story-decision AI smell, reveal value, thematic explicitness, or causal tidiness is in scope
rules/sltd_character_voice_dialogue_relationship_location_gate.md if voice, relationship, silence, presence, or location staging is affected
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md if exact Vietnamese surface, Human Chapter Pass, or Publication Lock is in scope
prompts/context_capsule_preflight.md
prompts/node_checkpoint.md
```

### Narrative claim / constraint / harm gates

```text
narrative claim verification: source/context -> tracking if state/thread/object is affected -> claim verification -> multi-constraint if verified claim becomes output constraint -> harm if false/uncertain claim creates risk -> corpus topic if claim concerns topic/thread assignment -> longform quality if quality verdict depends on verified evidence -> node_checkpoint
multi-constraint instruction ledger: source/context -> claim verification if needed -> harm if constraint failure needs vignette -> corpus topic if constraints come from map -> longform quality if length/quality constraints affect acceptance -> multi-constraint ledger -> structural/tracking/voice/style/surface gates as evidence requires -> node_checkpoint
editorial harm anticipation: source/context -> claim verification if needed -> multi-constraint if needed -> corpus topic if harm is map-level drift -> longform quality if harm is false longform quality or quality collapse -> harm matrix -> node_checkpoint
```

### Narrative feature / structural idiosyncrasy audit

```text
source/context -> claim verification if needed -> multi-constraint if findings become draft constraints -> harm if structural smell creates downstream risk -> corpus topic if packet/arc clusters or narrative diversity are in scope -> longform quality if bloat, over-summary, or late-output collapse is in scope -> structural/tracking/voice gates as evidence requires -> narrative_feature_audit -> node_checkpoint
```

### Character voice / dialogue / relationship / location staging

```text
rules/sltd_source_fidelity_anti_compression.md
context_capsule_preflight if current source, hidden canon, POV knowledge, object state, relationship memory, or long-range context is in scope
narrative_claim_verification_check if a voice/knowledge/status claim needs evidence
multi_constraint_instruction_check if character voice is one of several constraints
editorial_harm_anticipation_check if voice/relationship harm is in scope
corpus_topic_thread_discovery_check if packet/arc voice or relationship clusters are in scope
reference_anchored_story_quality_check if longform dialogue/voice quality is in scope
rules/sltd_character_voice_dialogue_relationship_location_gate.md
prompts/character_voice_dialogue_staging_check.md
prompts/node_checkpoint.md
```

### Author writing sheet / author voice / author-aligned draft

```text
author_writing_sheet_check: source/taste -> claim verification if needed -> multi-constraint if style is an output constraint -> harm if style-over-character risk exists -> corpus topic if style clusters are map-level -> longform quality if reference anchor or longform quality is in scope -> author writing sheet -> node_checkpoint
author_voice_fingerprint_check: source/taste -> author writing sheet if style evidence is needed -> context/claim/constraint/harm/topic/quality gates as evidence requires -> author voice fingerprint -> node_checkpoint
author_aligned_draft: source surface or current packet -> context capsule when required -> claim verification if draft depends on source claim -> multi-constraint ledger -> harm check when failure cost is high -> author writing sheet if style memory is used -> structural/tracking/narrative-feature/voice gates as needed -> bounded draft -> human surface polish if needed -> node_checkpoint
```

### General + chapter feedback matrix / packet route

```text
source/context -> corpus_topic_thread_discovery_check if map-level topic/thread output is requested -> claim verification if packet/status/canon/continuity claims need verdict -> multi-constraint ledger if packet/readiness/audit has multiple constraints -> harm anticipation if REDTEAM/PREMORTEM risk is in scope -> reference_anchored_story_quality_check if chapter/packet longform quality, length adherence, drift, bloat, or late-output collapse is in scope -> general feedback matrix or result report -> node_checkpoint
```

### Tracking / structural / surface / prose work

```text
source_surface_check when exact prose or status is required
context_capsule_preflight when current source, hidden canon, POV knowledge, object state, relationship memory, lore retrieval, or long-range continuity is in scope
corpus_topic_thread_discovery_check only when map-level topic/thread navigation is in scope
reference_anchored_story_quality_check when longform draft/chapter quality across length is in scope
narrative_claim_verification_check when a status/canon/continuity/source-conflict claim controls the route
multi_constraint_instruction_check when rewrite/audit/polish/readiness has multiple constraints
editorial_harm_anticipation_check when REDTEAM/PREMORTEM/harm vignettes are required
structural/tracking/narrative-feature/voice/author/surface gates only when evidence requires them
prompts/node_checkpoint.md
```

### Human surface polish / anti-synthetic prose

```text
source_surface_check when exact prose is being patched
context_capsule_preflight when required
narrative_claim_verification_check if the patch depends on a factual/canon/continuity claim
multi_constraint_instruction_check if polish must preserve multiple constraints
editorial_harm_anticipation_check if over-polish or false-surface harm is in scope
corpus_topic_thread_discovery_check only if the surface issue is actually map-level repetition/thread drift
reference_anchored_story_quality_check if the issue may be longform bloat, over-summary, over-explanation, or quality collapse rather than local polish
narrative_feature_audit / voice / author / Vietnamese surface / human surface gates as evidence requires
prompts/human_surface_polish_pass.md
prompts/node_checkpoint.md
```

## Rule

Run `reference_anchored_story_quality_check.md` when the task concerns POLARIS-style longform story quality, reference-anchored quality, long rewrite/chapter quality, length adherence, bloat, drift, over-summary, over-explanation, late-output collapse, or sustained quality across a long scene/chapter/packet. Use it as a quality stress test, not readiness or lock.

Run `corpus_topic_thread_discovery_check.md` when the task concerns TopicGPT-style topic modeling, corpus topic discovery, thread discovery, motif clusters, repeated AI-smell clusters, packet/arc/series map, topic gaps, thread drift, or source assignments with quote anchors. Use for map-level navigation, not line edit or readiness.

Run `narrative_claim_verification_check.md`, `multi_constraint_instruction_check.md`, `editorial_harm_anticipation_check.md`, `narrative_feature_audit.md`, `author_writing_sheet_check.md`, `author_voice_fingerprint_check.md`, `general_chapter_feedback_matrix_check.md`, `tracking_logic_ledger_check.md`, `structural_spine_outline_preprose_check.md`, `vietnamese_senior_editor_surface_check.md`, and `human_surface_polish_pass.md` only when their source/evidence scope is actually in play.

Run `source_surface_check` before exact prose, status, readiness, patch, line edit, topic assignment requiring current evidence, claim verification, multi-constraint ledger, harm anticipation, longform quality verdict, narrative-feature verdict, human-surface polish, author-aligned drafting, or lock verdict.
