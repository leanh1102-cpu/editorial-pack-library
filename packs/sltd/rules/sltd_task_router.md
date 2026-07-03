# SLTD Task Router

Map each request to the smallest route.

Base:

```text
boot_task -> source_preflight -> context_capsule_preflight when current source, hidden canon, POV knowledge, source-status separation, or long-range continuity is in scope -> task_intake -> decision_safety
```

## Primary routes

```text
context capsule preflight: source fidelity -> context capsule -> claim verification if current status/canon/continuity/readiness/lock/source-conflict claim is in scope -> multi-constraint ledger if output has several controlling constraints -> editorial harm if REDTEAM/PREMORTEM/readiness/lock/large-rewrite risk is in scope -> corpus topic/thread discovery if packet/arc/series map-level navigation is in scope -> reference anchored story quality if longform quality across length is in scope -> dependent gates as evidence requires -> context_capsule_preflight -> node_checkpoint

reference anchored story quality check: source_preflight or source_surface_check when exact output is judged -> source fidelity -> context capsule when required -> claim verification if quality depends on factual/status/canon evidence -> multi-constraint ledger if output constraints control the draft -> editorial harm if false quality/readiness harm is in scope -> corpus topic/thread discovery if packet/arc map-level quality is in scope -> reference anchored quality rule -> narrative feature audit if structural AI smell or narrative diversity is in scope -> human surface polish only if surface polish is already authorized -> reference_anchored_story_quality_check -> node_checkpoint

corpus topic thread discovery check: source_preflight or source_surface_check when current map evidence is required -> context_brief for packet/arc/part/series scope -> source fidelity -> context capsule when required -> corpus topic/thread rule -> claim verification if topic assignment depends on factual/status/canon evidence -> tracking ledger if thread state/object/payoff debt is in scope -> narrative feature if repeated structural AI smell or narrative diversity is in scope -> editorial harm if topic/thread drift creates downstream harm -> reference quality if packet/arc quality across length is in scope -> corpus_topic_thread_discovery_check -> node_checkpoint

narrative claim verification: source/context -> tracking if state/object/debt/thread/claim anchor is affected -> claim verification rule -> multi-constraint if verified claim becomes output constraint -> editorial harm if false/uncertain claim creates risk -> corpus topic if claim concerns topic/thread assignment -> reference quality if quality verdict depends on verified evidence -> narrative feature or Vietnamese surface only when evidence requires -> node_checkpoint

multi-constraint instruction check: source/context -> claim verification if constraint depends on factual evidence -> editorial harm if failed constraint has high cost -> corpus topic if constraints come from packet/arc map -> reference quality if length/quality constraints affect acceptance -> multi-constraint rule -> structural/tracking/voice/style/surface gates only as evidence requires -> node_checkpoint

editorial harm anticipation check: source/context -> claim verification if harm depends on factual evidence -> multi-constraint if constraints control prevention -> corpus topic if harm is map-level topic/thread drift -> reference quality if harm is false longform quality or late collapse -> harm rule -> narrative feature / voice / author / surface only as evidence requires -> node_checkpoint

narrative feature audit: source/context -> claim verification if verdict depends on a testable claim -> multi-constraint if findings become draft constraints -> editorial harm if structural smell creates downstream risk -> corpus topic if packet/arc clusters or narrative diversity are in scope -> reference quality if bloat, over-summary, over-explanation, or late-output collapse is in scope -> narrative feature rule -> node_checkpoint

character voice dialogue staging check: source/context -> claim verification if voice/knowledge/status claim needs evidence -> multi-constraint if character voice is one of several constraints -> editorial harm if voice/relationship harm is in scope -> corpus topic if packet/arc voice or relationship clusters are in scope -> reference quality if longform dialogue/voice quality is in scope -> character voice gate -> node_checkpoint

author writing sheet check: source/taste -> claim verification if style claim depends on status/canon evidence -> multi-constraint if style is one output constraint -> harm if style-over-character risk is in scope -> corpus topic if author-style clusters are map-level -> reference quality if reference anchor or author-aligned longform quality is in scope -> author writing sheet -> node_checkpoint

author voice fingerprint check: source/taste -> author writing sheet if style claims need evidence -> context/claim/constraint/harm/topic/reference-quality gates as evidence requires -> author voice fingerprint -> node_checkpoint

author aligned draft: source_surface or current packet -> context capsule when required -> claim verification if draft depends on source claim -> multi-constraint ledger -> editorial harm when failure cost is high -> reference quality when longform quality or length adherence is in scope -> author writing sheet if style memory is used -> structural/tracking/narrative-feature/voice gates as needed -> bounded draft -> human surface polish if needed -> node_checkpoint

general chapter feedback matrix check: source/context -> corpus topic if map-level output is requested -> claim verification if packet/status/canon/continuity claims need verdict -> multi-constraint ledger if packet/readiness/audit has several constraints -> editorial harm if REDTEAM/PREMORTEM risk is in scope -> reference quality if chapter/packet longform quality is requested -> relevant gates -> matrix/report -> node_checkpoint

tracking logic ledger check: source/context -> corpus topic if thread clusters need source assignments -> claim verification if state/thread/object claim needs verdict -> multi-constraint if tracking constraints control output -> editorial harm if tracking failure creates downstream harm -> reference quality if longform output depends on stable state/thread -> tracking ledger -> node_checkpoint

structural spine outline pre-prose check: source/context -> corpus topic if arc/packet topic map affects prose permission -> claim verification if chapter card/scene packet/source claim is disputed -> multi-constraint if scene constraints must be preserved -> editorial harm if structure failure creates downstream harm -> reference quality if chapter assembly or long rewrite acceptance is in scope -> structural spine -> node_checkpoint

vietnamese senior editor surface check: source/context -> claim verification if pass/status/source claim is disputed -> multi-constraint if surface repair must preserve constraints -> editorial harm if false-surface harm is in scope -> reference quality if surface issue may be longform bloat or quality collapse -> Vietnamese senior surface -> node_checkpoint

human surface polish pass: exact source surface -> context when required -> claim verification if patch depends on factual claim -> multi-constraint if polish preserves constraints -> editorial harm if over-polish/false-surface harm is in scope -> corpus topic only if surface issue is map-level repetition/thread drift -> reference quality if issue is longform bloat, over-summary, or quality collapse rather than local polish -> narrative feature/voice/author gates as needed -> human surface polish -> node_checkpoint

readiness: source_surface -> context capsule -> claim verification for current status / Human Chapter Pass / Publication Lock / packet lock / source conflict claims -> multi-constraint ledger for readiness constraints -> editorial harm for false readiness / lock / downstream harm -> corpus topic only if packet/arc map is requested -> reference quality only as readiness-risk evidence, not readiness substitute -> structural/tracking/narrative-feature/voice/author/surface gates as needed -> publishing readiness reviewer -> node_checkpoint

packet review: source/context -> corpus topic when topic/thread discovery or series navigation is in scope -> claim verification for packet-level status/canon/continuity/readiness claims -> multi-constraint for packet constraints -> editorial harm for packet-level REDTEAM/PREMORTEM vignettes -> reference quality for packet-level longform quality/length adherence -> relevant gates -> matrix/report -> node_checkpoint
```

## Rules

```text
Run reference_anchored_story_quality_check for POLARIS-style longform story quality, reference-anchored quality, long rewrite/chapter quality, length adherence, bloat, drift, over-summary, over-explanation, late-output collapse, or sustained quality across a long scene/chapter/packet. Use as quality stress test only.
Run corpus_topic_thread_discovery_check for TopicGPT-style topic modeling, thread discovery, motif clusters, repeated AI-smell clusters, packet/arc/series map, topic gaps, thread drift, or source assignments with quote anchors. Use map-level navigation only.
Run context_capsule_preflight, narrative_claim_verification_check, multi_constraint_instruction_check, editorial_harm_anticipation_check, narrative_feature_audit, character_voice_dialogue_staging_check, author_writing_sheet_check, author_voice_fingerprint_check, general_chapter_feedback_matrix_check, tracking_logic_ledger_check, structural_spine_outline_preprose_check, vietnamese_senior_editor_surface_check, and human_surface_polish_pass only when their source/evidence scope is actually in play.
Run source_surface_check before exact prose, status, readiness, patch, line edit, topic assignment requiring current evidence, claim verification, multi-constraint ledger, harm anticipation, longform quality verdict, narrative-feature verdict, human-surface polish, author-aligned draft, or lock verdict.
Stop at the first real blocker.
```