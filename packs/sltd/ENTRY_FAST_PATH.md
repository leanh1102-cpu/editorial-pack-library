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
2. Context Memory Lifecycle when prior handoff/context brief/chat memory/source-status note may be reused
3. Multilingual Long-Context Retrieval when found/not-found/absence/aggregation over long Vietnamese source is in scope
4. Narrative Claim Verification when status/canon/continuity/lock claim is in scope
5. Comparative Editorial Feedback Delta when user/editor feedback must become increase/decrease/preserve/prohibit constraints
6. Multi-Constraint Instruction Ledger when rewrite/audit/readiness has multiple controlling constraints
7. Editorial Harm Anticipation when REDTEAM/PREMORTEM/readiness/lock/large-rewrite harm risk is in scope
8. Corpus Topic / Thread Discovery when packet/arc/series map-level navigation is in scope
9. Reference-Anchored Longform Story Quality when long rewrite/chapter/packet quality across length is in scope
10. Spine Lock
11. Tracking / Logic Ledger
12. Borderbound
13. Life-Task Bound
14. Story Movement
15. Scene-First Prose Judgment
16. Narrative Feature / Structural Idiosyncrasy Audit when story-decision AI smell is in scope
17. Human Expert AI-Smell Explanation when a span needs reader-effect explanation, not detector scoring
18. Voice / Dialogue / Staging
19. Author Writing Sheet when claim-evidence style memory is in scope
20. Author Voice Fingerprint when author style matching is in scope
21. Draft / Rewrite / Author-Aligned Ghostwriter Draft
22. Line / Voice / Rhythm
23. Human Surface Polish
24. Composite Risk Check
25. Feedback Matrix / Report
26. Seam / Chapter Assembly
27. Readiness / Lock
```

Do not run later gears to hide failure in earlier gears. Choose one primary route, add only evidence-required secondary gates, and stop at the first real blocker. Detailed gate budget and no-cascade rules live in `rules/sltd_entry_route_governance_gate_budget_protocol.md`.

## Fast paths

### Context memory lifecycle / ByteRover discipline

```text
rules/sltd_source_preflight.md if current source/status/canon/readiness may be affected
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_multilingual_long_context_retrieval_oneruler_discipline.md if the context entry depends on found/not-found/absence/aggregation evidence
rules/sltd_context_capsule_lore_retrieval_discipline.md if hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, reveal timing, or long-range continuity is in scope
rules/sltd_narrative_claim_verification_clipper_discipline.md if the context entry contains a factual/status/canon/continuity claim
rules/sltd_comparative_editorial_feedback_delta_discipline.md if the context entry captures user/editor feedback
rules/sltd_agent_native_context_memory_lifecycle_byterover_discipline.md
prompts/context_memory_lifecycle_check.md
prompts/node_checkpoint.md
```

### Multilingual long-context source retrieval / OneRuler discipline

```text
rules/sltd_source_preflight.md
prompts/source_surface_check.md if exact text/status/current source is required
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_agent_native_context_memory_lifecycle_byterover_discipline.md if prior context, handoff, stale memory, or source-status note is reused
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, reveal timing, or long-range continuity is in scope
rules/sltd_multilingual_long_context_retrieval_oneruler_discipline.md
rules/sltd_narrative_claim_verification_clipper_discipline.md if retrieval result becomes a TRUE/FALSE/UNCERTAIN claim
rules/sltd_corpus_topic_thread_discovery_topicgpt_discipline.md if retrieval result feeds topic/thread assignment
rules/sltd_reference_anchored_longform_quality_polaris_discipline.md if retrieval result controls Must Show/source preservation in long output
prompts/multilingual_long_context_retrieval_check.md
prompts/node_checkpoint.md
```

### Comparative editorial feedback delta

```text
rules/sltd_source_preflight.md
prompts/source_surface_check.md if exact span/current output is judged
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_agent_native_context_memory_lifecycle_byterover_discipline.md if prior feedback delta, handoff, or preference note is reused
rules/sltd_multilingual_long_context_retrieval_oneruler_discipline.md if feedback depends on found/not-found/aggregation across long source
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, reveal timing, or long-range continuity is in scope
rules/sltd_human_expert_ai_smell_explanation_discipline.md if feedback concerns synthetic reader effect or AI-smell and root cause is unclear
rules/sltd_narrative_claim_verification_clipper_discipline.md if feedback depends on factual/status/canon/continuity evidence
rules/sltd_multi_constraint_instruction_ledger_suri_discipline.md if feedback creates several controlling constraints
rules/sltd_comparative_editorial_feedback_delta_discipline.md
prompts/comparative_editorial_feedback_delta_check.md
prompts/node_checkpoint.md
```

### Human expert AI-smell explanation

```text
rules/sltd_source_preflight.md
prompts/source_surface_check.md if exact prose/span is judged
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_agent_native_context_memory_lifecycle_byterover_discipline.md if prior AI-smell handoff/style note is reused
rules/sltd_multilingual_long_context_retrieval_oneruler_discipline.md if the smell claim depends on repeated patterns or absence across long source
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
rules/sltd_narrative_claim_verification_clipper_discipline.md if the smell claim depends on factual/status/canon/continuity evidence
rules/sltd_comparative_editorial_feedback_delta_discipline.md if AI-smell feedback must become bounded increase/decrease/preserve/prohibit constraints
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md if story-decision AI smell may be root cause
rules/sltd_character_voice_dialogue_relationship_location_gate.md if dialogue/voice/relationship/staging is root cause
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md if exact Vietnamese surface is in scope
rules/sltd_human_surface_polish_anti_synthetic_gate.md only if correct-but-synthetic repair is source-safe and authorized
rules/sltd_human_expert_ai_smell_explanation_discipline.md
prompts/human_expert_ai_smell_explanation_check.md
prompts/node_checkpoint.md
```

### Reference-anchored longform story quality / POLARIS discipline

```text
rules/sltd_source_preflight.md
prompts/source_surface_check.md when exact output is judged
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_agent_native_context_memory_lifecycle_byterover_discipline.md if prior quality verdict, handoff, anchor note, or source-status note is reused
rules/sltd_multilingual_long_context_retrieval_oneruler_discipline.md if Must Show/source preservation or absence claim depends on long source retrieval
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
rules/sltd_narrative_claim_verification_clipper_discipline.md if a quality claim depends on factual/status/canon evidence
rules/sltd_comparative_editorial_feedback_delta_discipline.md if quality feedback must be converted into revision deltas
rules/sltd_multi_constraint_instruction_ledger_suri_discipline.md if output constraints control the draft
rules/sltd_editorial_harm_anticipation_aha_vignette_matrix.md if false quality/readiness harm is in scope
rules/sltd_corpus_topic_thread_discovery_topicgpt_discipline.md if packet/arc map-level quality is in scope
rules/sltd_reference_anchored_longform_quality_polaris_discipline.md
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md if structural AI smell or narrative diversity is in scope
rules/sltd_human_expert_ai_smell_explanation_discipline.md if sustained quality failure needs reader-facing synthetic-effect explanation
rules/sltd_human_surface_polish_anti_synthetic_gate.md only if correct-but-synthetic surface is source-safe and authorized
prompts/reference_anchored_story_quality_check.md
prompts/node_checkpoint.md
```

### Corpus topic / thread discovery map

```text
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_agent_native_context_memory_lifecycle_byterover_discipline.md if prior topic/thread map, handoff, or source-map entry is reused
rules/sltd_multilingual_long_context_retrieval_oneruler_discipline.md if topic/thread assignment, motif absence, or aggregation depends on long Vietnamese source retrieval
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, reveal timing, or long-range continuity is in scope
rules/sltd_corpus_topic_thread_discovery_topicgpt_discipline.md
rules/sltd_narrative_claim_verification_clipper_discipline.md if topic assignment depends on factual/status/canon evidence
rules/sltd_tracking_logic_ledger_traceability_gate.md if thread state, object state, or payoff debt is in scope
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md if repeated structural AI smell, narrative diversity, or thematic drift is in scope
rules/sltd_human_expert_ai_smell_explanation_discipline.md if repeated AI-smell clusters need span-based explanation
rules/sltd_comparative_editorial_feedback_delta_discipline.md if topic/thread feedback must become revision constraints
rules/sltd_editorial_harm_anticipation_aha_vignette_matrix.md if topic/thread drift creates downstream harm
prompts/corpus_topic_thread_discovery_check.md
prompts/node_checkpoint.md
```

### Context capsule / lore retrieval discipline

```text
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_context_capsule_lore_retrieval_discipline.md
rules/sltd_agent_native_context_memory_lifecycle_byterover_discipline.md if prior handoff/context entry/memory/source-status note may be reused
rules/sltd_multilingual_long_context_retrieval_oneruler_discipline.md if found/not-found/absence/aggregation across long Vietnamese source is in scope
rules/sltd_narrative_claim_verification_clipper_discipline.md if current status, canon, continuity, readiness, lock, or source conflict claim is in scope
rules/sltd_multi_constraint_instruction_ledger_suri_discipline.md if rewrite/audit/readiness has multiple controlling constraints
rules/sltd_editorial_harm_anticipation_aha_vignette_matrix.md if REDTEAM/PREMORTEM/readiness/lock/large rewrite harm risk is in scope
rules/sltd_corpus_topic_thread_discovery_topicgpt_discipline.md if packet/arc/series map-level navigation is in scope
rules/sltd_reference_anchored_longform_quality_polaris_discipline.md if long rewrite/chapter/packet quality across length is in scope
rules/sltd_human_expert_ai_smell_explanation_discipline.md if synthetic reader-effect explanation is in scope
rules/sltd_comparative_editorial_feedback_delta_discipline.md if user/editor feedback must become revision deltas
rules/sltd_tracking_logic_ledger_traceability_gate.md if state, knowledge, object, residue, thread, pass trace, or downstream risk is affected
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if scene function, chapter card, scene packet, or border is unclear
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md if story-decision AI smell, reveal value, thematic explicitness, or causal tidiness is in scope
rules/sltd_character_voice_dialogue_relationship_location_gate.md if voice, relationship, silence, presence, or location staging is affected
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md if exact Vietnamese surface, Human Chapter Pass, or Publication Lock is in scope
prompts/context_capsule_preflight.md
prompts/node_checkpoint.md
```

### Editorial harm anticipation / AHA vignette matrix

```text
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_agent_native_context_memory_lifecycle_byterover_discipline.md if prior risk/harm handoff may be stale or reused
rules/sltd_multilingual_long_context_retrieval_oneruler_discipline.md if harm depends on found/not-found/absence/aggregation evidence
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
rules/sltd_narrative_claim_verification_clipper_discipline.md if a harm depends on factual/status/canon evidence
rules/sltd_multi_constraint_instruction_ledger_suri_discipline.md if constraints control output or harm prevention
rules/sltd_corpus_topic_thread_discovery_topicgpt_discipline.md if harm comes from packet/arc/series topic/thread drift
rules/sltd_reference_anchored_longform_quality_polaris_discipline.md if harm is false longform quality or quality collapse across length
rules/sltd_human_expert_ai_smell_explanation_discipline.md if harm comes from false human-surface or AI-smell misdiagnosis
rules/sltd_comparative_editorial_feedback_delta_discipline.md if user feedback may be mistranslated into harmful revision direction
rules/sltd_editorial_harm_anticipation_aha_vignette_matrix.md
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md if structural AI smell may cause harm
rules/sltd_character_voice_dialogue_relationship_location_gate.md if voice/relationship harm is in scope
rules/sltd_author_writing_sheet_claim_evidence_discipline.md if style-over-character harm is in scope
rules/sltd_human_surface_polish_anti_synthetic_gate.md if over-polish harm is in scope
prompts/editorial_harm_anticipation_check.md
prompts/node_checkpoint.md
```

### Multi-constraint instruction ledger / Suri discipline

```text
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_agent_native_context_memory_lifecycle_byterover_discipline.md if constraints came from prior handoff/memory/feedback entry
rules/sltd_multilingual_long_context_retrieval_oneruler_discipline.md if a constraint depends on found/not-found/absence/aggregation evidence
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
rules/sltd_narrative_claim_verification_clipper_discipline.md if a constraint depends on factual/status/canon evidence
rules/sltd_comparative_editorial_feedback_delta_discipline.md if constraints originate in user/editor feedback
rules/sltd_editorial_harm_anticipation_aha_vignette_matrix.md if constraint failure needs REDTEAM/PREMORTEM harm vignette
rules/sltd_corpus_topic_thread_discovery_topicgpt_discipline.md if constraints come from packet/arc/series topic/thread map
rules/sltd_reference_anchored_longform_quality_polaris_discipline.md if length/quality constraints affect draft acceptance
rules/sltd_human_expert_ai_smell_explanation_discipline.md if synthetic-surface explanation becomes an output constraint
rules/sltd_multi_constraint_instruction_ledger_suri_discipline.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if scene/chapter function or prose permission is unclear
rules/sltd_tracking_logic_ledger_traceability_gate.md if state, object, debt, residue, thread, or downstream risk is affected
rules/sltd_character_voice_dialogue_relationship_location_gate.md if dialogue or character voice is in scope
rules/sltd_author_writing_sheet_claim_evidence_discipline.md if style constraints are in scope
rules/sltd_human_surface_polish_anti_synthetic_gate.md if surface polish is the next node
prompts/multi_constraint_instruction_check.md
prompts/node_checkpoint.md
```

### Narrative claim verification / CLIPPER discipline

```text
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_agent_native_context_memory_lifecycle_byterover_discipline.md if claim came from prior handoff/context entry/chat memory
rules/sltd_multilingual_long_context_retrieval_oneruler_discipline.md if the claim depends on source retrieval, absence, or aggregation
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
rules/sltd_tracking_logic_ledger_traceability_gate.md if state, object, debt, residue, thread, claim anchor, or downstream risk is affected
rules/sltd_narrative_claim_verification_clipper_discipline.md
rules/sltd_comparative_editorial_feedback_delta_discipline.md if verified claim changes the feedback delta
rules/sltd_multi_constraint_instruction_ledger_suri_discipline.md if the verified claim becomes a draft/rewrite constraint
rules/sltd_editorial_harm_anticipation_aha_vignette_matrix.md if a false/uncertain claim may cause readiness/canon/editorial harm
rules/sltd_corpus_topic_thread_discovery_topicgpt_discipline.md if the claim concerns topic/thread assignment
rules/sltd_reference_anchored_longform_quality_polaris_discipline.md if quality verdict depends on verified evidence
rules/sltd_human_expert_ai_smell_explanation_discipline.md if the claim concerns reader-facing AI-smell explanation
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md if the claim concerns story-decision AI smell or structural idiosyncrasy
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md if Human Chapter Pass, Publication Lock, or exact Vietnamese surface is in scope
prompts/narrative_claim_verification_check.md
prompts/node_checkpoint.md
```

### Narrative feature / structural idiosyncrasy audit

```text
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_agent_native_context_memory_lifecycle_byterover_discipline.md if prior structural-smell verdict or handoff is reused
rules/sltd_multilingual_long_context_retrieval_oneruler_discipline.md if story-decision verdict depends on long-source retrieval or repeated-pattern aggregation
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, reveal timing, or long-range continuity is in scope
rules/sltd_narrative_claim_verification_clipper_discipline.md if a story-decision verdict depends on a testable claim or false twin
rules/sltd_comparative_editorial_feedback_delta_discipline.md if story-decision findings must become bounded revision deltas
rules/sltd_multi_constraint_instruction_ledger_suri_discipline.md if story-decision findings become draft constraints
rules/sltd_editorial_harm_anticipation_aha_vignette_matrix.md if structural AI smell may create downstream harm
rules/sltd_corpus_topic_thread_discovery_topicgpt_discipline.md if packet/arc topic clusters or narrative diversity are in scope
rules/sltd_reference_anchored_longform_quality_polaris_discipline.md if bloat, over-summary, over-explanation, or late-output collapse is in scope
rules/sltd_human_expert_ai_smell_explanation_discipline.md if structural AI smell needs span-based reader explanation
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if scene/chapter function or prose permission is unclear
rules/sltd_tracking_logic_ledger_traceability_gate.md if state, object, debt, residue, thread, reveal, or downstream risk is affected
rules/sltd_character_voice_dialogue_relationship_location_gate.md if dialogue function, character presence, or relationship pressure is in scope
rules/sltd_author_voice_fingerprint_ghostwriter_discipline.md if author-style match or author-aligned draft is being evaluated
rules/sltd_human_surface_polish_anti_synthetic_gate.md if the next node may be surface polish
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md
prompts/narrative_feature_audit.md
prompts/node_checkpoint.md
```

### Character voice / dialogue / relationship / location staging

```text
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_agent_native_context_memory_lifecycle_byterover_discipline.md if prior voice/relationship/style note is reused
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, object state, relationship memory, or long-range context is in scope
rules/sltd_multilingual_long_context_retrieval_oneruler_discipline.md if voice/relationship pattern or absence claim depends on long source retrieval
rules/sltd_narrative_claim_verification_clipper_discipline.md if a voice/knowledge/status claim needs evidence
rules/sltd_comparative_editorial_feedback_delta_discipline.md if dialogue/voice feedback must be split into increase/decrease/preserve/prohibit
rules/sltd_multi_constraint_instruction_ledger_suri_discipline.md if character voice is one of several controlling constraints
rules/sltd_editorial_harm_anticipation_aha_vignette_matrix.md if voice/relationship harm is in scope
rules/sltd_corpus_topic_thread_discovery_topicgpt_discipline.md if packet/arc voice or relationship clusters are in scope
rules/sltd_reference_anchored_longform_quality_polaris_discipline.md if longform dialogue/voice quality is in scope
rules/sltd_human_expert_ai_smell_explanation_discipline.md if same-voice dialogue or register mismatch needs span-based explanation
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md if dialogue is structurally decorative, causality is too tidy, or body/sensory pressure performs without consequence
rules/sltd_character_voice_dialogue_relationship_location_gate.md
samples/character_voice_dialogue_staging_calibration.md
rules/sltd_tracking_logic_ledger_traceability_gate.md if relationship memory, knowledge state, object state, or downstream risk is affected
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if scene function or border is unclear
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md if exact Vietnamese dialogue surface is in scope
rules/sltd_author_writing_sheet_claim_evidence_discipline.md if author style may overwrite character voice or needs claim-evidence memory
rules/sltd_author_voice_fingerprint_ghostwriter_discipline.md if author voice may overwrite character voice
rules/sltd_character_distinctiveness_iceberg_gate.md if voice profile is unclear
rules/sltd_living_world_community_motion_gate.md if group presence or community motion is in scope
prompts/character_voice_dialogue_staging_check.md
prompts/node_checkpoint.md
```

### Author writing sheet / claim-evidence style memory

```text
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_agent_native_context_memory_lifecycle_byterover_discipline.md if prior author-style note or style memory is reused
AUTHOR_WORKING_PROFILE.md
AUTHOR_TASTE_EXAMPLES.md
rules/sltd_narrative_claim_verification_clipper_discipline.md if a style claim depends on a factual/status/canon claim
rules/sltd_comparative_editorial_feedback_delta_discipline.md if author-style feedback must stay task-local instead of global style law
rules/sltd_multi_constraint_instruction_ledger_suri_discipline.md if style is one of several draft constraints
rules/sltd_editorial_harm_anticipation_aha_vignette_matrix.md if style-over-character harm is in scope
rules/sltd_corpus_topic_thread_discovery_topicgpt_discipline.md if author-style topic clusters are in scope
rules/sltd_reference_anchored_longform_quality_polaris_discipline.md if reference anchor or author-aligned longform quality is in scope
rules/sltd_human_expert_ai_smell_explanation_discipline.md if style-over-character smell needs reader explanation
rules/sltd_author_writing_sheet_claim_evidence_discipline.md
rules/sltd_author_voice_fingerprint_ghostwriter_discipline.md
rules/sltd_character_voice_dialogue_relationship_location_gate.md if character voice may be affected
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md if exact Vietnamese surface is being compared
prompts/author_writing_sheet_check.md
prompts/node_checkpoint.md
```

### Author voice fingerprint / ghostwriter discipline

```text
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_agent_native_context_memory_lifecycle_byterover_discipline.md if prior author-voice fingerprint or style handoff is reused
AUTHOR_WORKING_PROFILE.md
AUTHOR_TASTE_EXAMPLES.md
rules/sltd_author_writing_sheet_claim_evidence_discipline.md if style claims need evidence or prompt-specific story rules
rules/sltd_author_voice_fingerprint_ghostwriter_discipline.md
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
rules/sltd_narrative_claim_verification_clipper_discipline.md if author-aligned draft depends on status/canon/continuity claim
rules/sltd_comparative_editorial_feedback_delta_discipline.md if author-voice feedback must be preserved as bounded revision delta
rules/sltd_multi_constraint_instruction_ledger_suri_discipline.md if author-aligned draft must preserve multiple constraints
rules/sltd_editorial_harm_anticipation_aha_vignette_matrix.md if author-aligned draft has high downstream harm risk
rules/sltd_corpus_topic_thread_discovery_topicgpt_discipline.md if author-style thread/topic clusters are in scope
rules/sltd_reference_anchored_longform_quality_polaris_discipline.md if longform author-aligned draft quality or reference anchor is in scope
rules/sltd_human_expert_ai_smell_explanation_discipline.md if author voice match is confused with AI-smell or detector-like surface
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md if author-aligned prose may be structurally AI-shaped
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if scene function or prose permission is unclear
rules/sltd_tracking_logic_ledger_traceability_gate.md if state, object, debt, residue, thread, or downstream risk is affected
rules/sltd_character_voice_dialogue_relationship_location_gate.md if dialogue, character voice, relationship, silence, presence, or staging is in scope
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md if exact Vietnamese surface is in scope
prompts/author_writing_sheet_check.md if no claim-evidence style memory exists
prompts/author_voice_fingerprint_check.md for sample/style extraction or voice match
prompts/author_aligned_ghostwriter_draft.md for bounded source-safe drafting
prompts/node_checkpoint.md
```

### General + chapter feedback matrix

```text
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_agent_native_context_memory_lifecycle_byterover_discipline.md if prior matrix/handoff/context note guides current feedback
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, packet scope, canon status, or long-range context is in scope
rules/sltd_multilingual_long_context_retrieval_oneruler_discipline.md if found/not-found/aggregation over packet source controls the review
rules/sltd_corpus_topic_thread_discovery_topicgpt_discipline.md if topic/thread discovery, motif clustering, repeated AI-smell clusters, or series navigation is in scope
rules/sltd_narrative_claim_verification_clipper_discipline.md if packet/status/canon/continuity claims need TRUE/FALSE/UNCERTAIN verdicts
rules/sltd_comparative_editorial_feedback_delta_discipline.md if general or chapter feedback must become revision deltas
rules/sltd_multi_constraint_instruction_ledger_suri_discipline.md if packet/readiness/audit has multiple controlling constraints
rules/sltd_editorial_harm_anticipation_aha_vignette_matrix.md if packet/readiness/REDTEAM/PREMORTEM harm risk is in scope
rules/sltd_reference_anchored_longform_quality_polaris_discipline.md if chapter/packet longform quality, length adherence, drift, bloat, or late-output collapse is in scope
rules/sltd_human_expert_ai_smell_explanation_discipline.md if packet feedback includes repeated AI-smell explanation
rules/sltd_general_chapter_feedback_matrix_output_protocol.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if spine/source status is in scope
rules/sltd_tracking_logic_ledger_traceability_gate.md if state/thread/object/pass/downstream logic is in scope
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md if story-decision AI smell, thematic overexplicitness, causal tidiness, or narrative diversity is a packet issue
rules/sltd_character_voice_dialogue_relationship_location_gate.md if dialogue, relationship, or staging is a packet issue
rules/sltd_author_writing_sheet_claim_evidence_discipline.md if author-style claims need evidence in packet review
rules/sltd_author_voice_fingerprint_ghostwriter_discipline.md if author voice match is a packet issue
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md if human surface or pass integrity is in scope
prompts/corpus_topic_thread_discovery_check.md if map-level topic/thread output is requested
prompts/general_chapter_feedback_matrix_check.md
prompts/node_checkpoint.md
```

### Tracking / structural / surface / prose work

```text
source_surface_check when exact prose or status is required
context_capsule_preflight when current source, hidden canon, POV knowledge, object state, relationship memory, lore retrieval, or long-range continuity is in scope
rules/sltd_agent_native_context_memory_lifecycle_byterover_discipline.md when prior handoff/context/source-status note may be reused
rules/sltd_multilingual_long_context_retrieval_oneruler_discipline.md when source retrieval, absence, or aggregation controls the route
rules/sltd_comparative_editorial_feedback_delta_discipline.md when user/editor feedback controls local repair direction
rules/sltd_human_expert_ai_smell_explanation_discipline.md when span-based synthetic-effect explanation is needed before repair
rules/sltd_reference_anchored_longform_quality_polaris_discipline.md when bloat, drift, over-summary, over-explanation, or late-output collapse is in scope
rules/sltd_corpus_topic_thread_discovery_topicgpt_discipline.md only when map-level topic/thread navigation is in scope
rules/sltd_narrative_claim_verification_clipper_discipline.md when a status/canon/continuity/source-conflict claim controls the route
rules/sltd_multi_constraint_instruction_ledger_suri_discipline.md when rewrite/audit/polish/readiness has multiple constraints
rules/sltd_editorial_harm_anticipation_aha_vignette_matrix.md when REDTEAM/PREMORTEM/harm vignettes are required
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md when spine or border is in scope
rules/sltd_tracking_logic_ledger_traceability_gate.md when logic continuity is affected
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md when story-decision AI smell, thematic overexplicitness, causal tidiness, reveal value, body/sensory overperformance, or narrative diversity is in scope
rules/sltd_character_voice_dialogue_relationship_location_gate.md when voice, relationship, or location staging is affected
rules/sltd_author_writing_sheet_claim_evidence_discipline.md when author style claims or prompt-specific story rules are in scope
rules/sltd_author_voice_fingerprint_ghostwriter_discipline.md when author voice, style match, or ghostwriter drafting is in scope
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md when human surface or pass integrity is affected
rules/sltd_human_surface_polish_anti_synthetic_gate.md when exact prose is source-safe but still reads synthetic, over-clean, same-voiced, or falsely smooth
relevant primary gate only when evidence requires it
prompts/node_checkpoint.md
```

### Human surface polish / anti-synthetic prose

```text
source_surface_check when exact prose is being patched
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_agent_native_context_memory_lifecycle_byterover_discipline.md if prior surface polish note, handoff, or feedback delta is reused
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
rules/sltd_multilingual_long_context_retrieval_oneruler_discipline.md if patch depends on locating source items or verifying absence
rules/sltd_narrative_claim_verification_clipper_discipline.md if the patch depends on a factual/canon/continuity claim
rules/sltd_comparative_editorial_feedback_delta_discipline.md if user/editor feedback controls local repair direction
rules/sltd_multi_constraint_instruction_ledger_suri_discipline.md if polish must preserve multiple constraints
rules/sltd_editorial_harm_anticipation_aha_vignette_matrix.md if over-polish or false-surface harm is in scope
rules/sltd_corpus_topic_thread_discovery_topicgpt_discipline.md only if surface issue is actually map-level repetition/thread drift
rules/sltd_reference_anchored_longform_quality_polaris_discipline.md if issue may be longform bloat, over-summary, or quality collapse rather than local polish
rules/sltd_human_expert_ai_smell_explanation_discipline.md if span-based synthetic-effect explanation is needed before repair
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if scene function or prose permission is unclear
rules/sltd_tracking_logic_ledger_traceability_gate.md if state, object, debt, residue, thread, or downstream risk is affected
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md if surface polish may hide structural AI smell or decorative body/sensory overperformance
rules/sltd_character_voice_dialogue_relationship_location_gate.md if voice, relationship, silence, presence, dialogue, or location staging is in scope
rules/sltd_author_writing_sheet_claim_evidence_discipline.md if style memory is used for polish
rules/sltd_author_voice_fingerprint_ghostwriter_discipline.md if author voice match or ghostwriter output is being polished
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md
rules/sltd_human_surface_polish_anti_synthetic_gate.md
prompts/human_surface_polish_pass.md
prompts/node_checkpoint.md
```

## Rule

Run `context_capsule_preflight.md` when the task concerns current/latest source, Notion current manuscript, lock, readiness, Human Chapter Pass, Publication Lock, packet verdict, canon conflict, hidden canon, POV knowledge, object/location/body/debt state, relationship memory, lore retrieval, legacy source risk, summary-vs-source risk, or long-range continuity.

Run `context_memory_lifecycle_check.md` when the task concerns prior handoff, context brief, node ledger, route note, source-status note, feedback delta reuse, stale chat memory risk, provenance, maturity, recency, semantic drift, or when a memory-like entry may be mistaken for source truth. Use for provenance/lifecycle discipline, not live manuscript memory.

Run `multilingual_long_context_retrieval_check.md` when the task concerns OneRuler-style long-context retrieval, multilingual/Vietnamese source retrieval, found/not-found/absence claims, aggregation across scenes/chapters/packets, exact phrase/status/object/thread/motif search, or when English instruction/query may miss Vietnamese source evidence. Use as retrieval and absence discipline only.

Run `comparative_editorial_feedback_delta_check.md` when the task concerns comparative or directional user/editor feedback, increase/decrease/preserve/prohibit deltas, A/B comparison, vague preference clarification, or turning feedback into bounded revision tests. Use as feedback translation only, not rewrite permission by itself.

Run `human_expert_ai_smell_explanation_check.md` when the task concerns human-expert AI-smell explanation, synthetic reader effect, detector-like prose, same-voice dialogue, over-clean surface, outline labels, keyword-only detector risk, false-positive risk, or repair routing without AI-probability scoring. Use as explanation only, not authorship detection.

Run `reference_anchored_story_quality_check.md` when the task concerns POLARIS-style longform story quality, reference-anchored quality, long rewrite/chapter quality, length adherence, bloat, drift, over-summary, over-explanation, late-output collapse, or sustained quality across a long scene/chapter/packet. Use as quality stress test only.

Run `corpus_topic_thread_discovery_check.md` when the task concerns TopicGPT-style topic modeling, corpus topic discovery, thread discovery, motif clusters, repeated AI-smell clusters, packet/arc/series map, topic gaps, thread drift, or source assignments with quote anchors. Use for map-level navigation, not line edit or readiness.

Run `narrative_claim_verification_check.md` when the task concerns CLIPPER-style claim verification, true/false claims, false twins, status claims, canon claims, continuity claims, POV knowledge claims, source conflicts, readiness claims, Human Chapter Pass, Publication Lock, or whether a claim is TRUE/FALSE/UNCERTAIN.

Run `multi_constraint_instruction_check.md` when rewrite, edit, audit, readiness, author-aligned drafting, line surgery, or human surface polish must preserve multiple source/canon/POV/scene/style/surface/wordcount/readiness constraints together.

Run `editorial_harm_anticipation_check.md` when the task concerns AHA-style harm anticipation, REDTEAM, PREMORTEM, readiness risk, lock risk, false readiness, reveal leak, over-polish harm, style-over-character harm, packet failure, or high-risk rewrite failure vignettes.

Run `narrative_feature_audit.md` when the task concerns StoryScope-style narrative features, structural AI smell, theme overexplained, causal tidiness, single-track plot risk, protagonist understanding as resolution, temporal flatness, weak reveal/recontextualization, decorative body/sensory detail, or narrative diversity.

Run `author_writing_sheet_check.md` when the task concerns Author Writing Sheet, claim-evidence style memory, sample-backed author profile, prompt-specific story rules, or author style claims that need evidence before author voice fingerprint or author-aligned drafting.

Run `character_voice_dialogue_staging_check.md` when the task concerns dialogue, multi-character scenes, character voice, relationship memory, silence, interruptions, location staging, usable objects, tone, comedy, grief, or physical action.

Run `author_voice_fingerprint_check.md` when the task concerns author voice, voice DNA, style guide, writing sample analysis, voice match, personal style, or prose that sounds unlike the author.

Run `author_aligned_ghostwriter_draft.md` only when source/canon/scene controls are clear and the user asks for author-aligned drafting, ghostwriter-style drafting, or writing in the author's voice.

Run `general_chapter_feedback_matrix_check.md` when the task asks for general feedback plus chapter-by-chapter feedback, packet/arc/hồi review, or matrix-style review output.

Run `tracking_logic_ledger_check.md` when the task concerns logic continuity, state trace, knowledge state, object/residue/thread tracking, payoff debt, status/pass trace, downstream risk, or verify target.

Run `structural_spine_outline_preprose_check.md` when act/arc/hồi/chapter/scene, Story Outline, Chapter by Chapter Outline, Chapter Card, Scene Packet, borderbound, or prose permission is in scope.

Run `vietnamese_senior_editor_surface_check.md` when senior Vietnamese reading, từng chữ, semantic load, repeated AI smell, pass metadata, Human Chapter Pass, candidate-ready, or Publication Lock is in scope.

Run `human_surface_polish_pass.md` when exact prose is source-safe and story/voice constraints are settled enough, but the passage still reads synthetic, over-clean, falsely smooth, same-voiced, symbol-first, or human-surface thin. Do not use it for detector bypass, structure repair, canon repair, or readiness.
