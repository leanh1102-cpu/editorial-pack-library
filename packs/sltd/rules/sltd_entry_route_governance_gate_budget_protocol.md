# SLTD Entry Route Governance & Gate Budget Protocol

This protocol keeps Entry Fast Path and Task Router usable as routing tools, not diagnostic mazes.

It prevents gate cascade, checklist-first repair, false precision, map bloat, quality-score overreach, and over-editing caused by running every related gate.

## Core rule

Choose one primary route. Add only necessary secondary gates. Stop when the request is answered.

```text
PRIMARY ROUTE = the smallest route that directly answers the user's request
SECONDARY GATE = a dependent check added only when the primary route exposes a real blocker
GATE BUDGET = the maximum number of gates allowed before the task must stop, report, or ask for source/scope
STOP CONDITION = the point where enough evidence, verdict, map, quality decision, constraint decision, harm decision, or rewrite output has been produced
```

Run a gate only when the request or evidence makes it necessary.

## Primary route triggers

```text
current / latest / Notion / source status / hidden canon / POV knowledge / long-range continuity -> context capsule preflight
POLARIS / longform quality / reference anchored quality / length adherence / bloat / drift / over-summary / over-explanation / late-output collapse -> reference anchored story quality check
TopicGPT / topic map / thread discovery / motif cluster / repeated pattern cluster / packet map / arc map / series map -> corpus topic thread discovery check
claim / true false / false twin / CLIPPER / canon claim / continuity claim / source conflict -> narrative claim verification check
multi-constraint / Suri / constraint ledger / corrupted constraint / giữ nhiều điều cùng lúc -> multi-constraint instruction check
AHA / harm / REDTEAM / PREMORTEM / false readiness / reveal leak / over-polish harm / failure vignette -> editorial harm anticipation check
Author Writing Sheet / claim-evidence style memory / style claim evidence / prompt-specific story rules -> author writing sheet check
rewrite / sửa cảnh -> scene rewrite or first-pass editorial workflow, with constraint ledger, harm, and reference-quality checks only when their blockers are real
line / câu / đoạn -> line surgery
StoryScope / narrative feature / structural AI smell / theme quá rõ / nhân quả quá sạch / tuyến đơn / reread value -> narrative feature audit
author voice / voice DNA / style guide / giọng tôi / giống giọng / học cách viết -> author voice fingerprint check
human surface / humanize / polish / đúng mà giả / mượt giả / văn nghe AI nhưng đúng ý -> human surface polish pass
readiness / lock / pass -> readiness route, with claim verification, constraint ledger, harm anticipation, and optional reference-quality check only as risk evidence
packet / arc / C001-C030 -> packet/arc review, with topic/thread discovery only when map-level navigation is requested
```

## Gate budget

```text
Reference-anchored story quality:
- source preflight or source surface when exact output is judged
- context capsule when current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
- claim verification only if quality depends on factual/status/canon evidence
- multi-constraint ledger only if output constraints control the draft
- harm anticipation only if false quality/readiness harm is in scope
- corpus topic/thread discovery only if packet/arc map-level quality is in scope
- reference quality check
- narrative feature or human surface only if quality findings expose those blockers
- stop before readiness/lock; quality checks do not grant those permissions

Corpus topic / thread discovery:
- context brief for packet/arc/part/series scope
- source preflight or source surface when current/source-status topic assignment is required
- context capsule when hidden canon, POV knowledge, source-status separation, reveal timing, or long-range continuity is in scope
- topic/thread discovery
- claim verification only if a topic assignment depends on factual/status/canon evidence
- tracking ledger only if thread state/object/payoff debt is in scope
- reference quality only if map-level output quality is in scope
- stop before rewrite/readiness/lock; topic maps do not grant those permissions

Narrative claim verification:
- source/context as required
- claim verification
- reference quality only if a quality verdict depends on verified evidence
- stop with TRUE / FALSE / UNCERTAIN; do not continue into readiness, polish, or rewrite from claim verification alone

Multi-constraint instruction ledger:
- source/context as required
- claim verification only if a constraint depends on factual/status/canon evidence
- multi-constraint ledger
- reference quality only if length/quality is an output constraint
- stop before draft/rewrite/readiness if constraints conflict, corrupted constraints are missing, or output anchors are unclear

Editorial harm anticipation:
- source/context as required
- claim verification and constraint ledger only if needed
- reference quality only if harm is false longform quality or late collapse
- top 3 harms by severity unless full matrix is requested

Author-aligned drafting:
- source surface or current scene packet
- context capsule when required
- claim verification if draft depends on source claim
- multi-constraint ledger for source/canon/POV/scene/style/surface/wordcount constraints
- harm anticipation if failure cost is high
- reference quality if longform quality or length adherence is in scope
- author writing sheet if style memory is used
- bounded draft

Chapter readiness:
- source surface / current Notion if current status is asked
- context capsule before status/pass verdict when needed
- claim verification for Human Chapter Pass / Publication Lock / packet lock / source-conflict claims
- multi-constraint ledger for readiness constraints
- harm anticipation for false readiness / lock / downstream harm
- reference quality only as risk evidence, never as readiness evidence by itself
- readiness reviewer
```

A secondary gate must be justified by a blocker, not by association.

## Stop conditions

Stop when:

```text
source is missing or current source was not read for a current-status claim;
context capsule blocks because POV knowledge, hidden canon, source status, object state, or long-range context is unclear;
reference quality blocks because source, output, anchor authorization, Must Show source, or exact output is missing;
reference quality is being used as readiness, lock, canon verdict, or rewrite permission;
topic/thread discovery blocks because scope, source, quote/evidence anchor, or current assignment evidence is missing;
topic map is being used as readiness, lock, canon verdict, or rewrite permission;
claim verification returns UNCERTAIN or false on a controlling claim;
multi-constraint ledger blocks because constraints are missing, corrupted constraints are missing, output anchors are missing, or constraints conflict;
harm anticipation blocks because scope/source/impact target/failure behavior is missing, harm depends on unverified claim, vignette would invent canon, or matrix overload hides the top blocker;
author writing sheet blocks because style evidence, approved samples, category coverage, or task fit is missing;
narrative feature audit blocks because story-decision smell remains unresolved;
primary blocker has been identified and next node is clear;
additional gates would be speculative;
secondary gate budget has been spent.
```

## Safe repair

Safe repair may select one primary route, cap secondary gates, require source/context, route longform quality tasks to Reference-Anchored Story Quality, route packet/arc/series maps to Corpus Topic / Thread Discovery, route disputed claims to Narrative Claim Verification, route multi-constraint output tasks to Multi-Constraint Ledger, route high-cost failures to Editorial Harm Anticipation, and stop at the first real blocker.

Safe repair must not drop required source checks, create topic maps without evidence anchors, use quality checks or topic maps as readiness/lock/canon/rewrite permission, skip claim verification when factual claims control the route, skip constraint ledger when multiple constraints control output, skip harm anticipation when failure risk is the primary blocker, continue running gates after stop condition, or create scripts, workflows, reports, issues, boards, or project-management files.

## Route governance audit

```text
ENTRY ROUTE GOVERNANCE CHECK
SCOPE:
SOURCE USED:
REQUEST TYPE:
SOURCE REQUIREMENT:
CONTEXT CAPSULE REQUIREMENT:
REFERENCE-ANCHORED STORY QUALITY REQUIREMENT:
CORPUS TOPIC / THREAD DISCOVERY REQUIREMENT:
CLAIM VERIFICATION REQUIREMENT:
MULTI-CONSTRAINT LEDGER REQUIREMENT:
EDITORIAL HARM ANTICIPATION REQUIREMENT:
NARRATIVE FEATURE REQUIREMENT:
AUTHOR WRITING SHEET REQUIREMENT:
AUTHOR VOICE / DRAFTING REQUIREMENT:
HUMAN SURFACE POLISH REQUIREMENT:
PRIMARY BLOCKER:
PRIMARY ROUTE:
SECONDARY GATES ALLOWED:
SECONDARY GATES USED:
GATE BUDGET:
STOP CONDITION:
NO-CASCADE CHECK:
CHECKLIST-FIRST RISK:
FAILURE LABELS:
ROUTE DECISION:
NEXT NODE:
```

## Output labels

```text
ENTRY_ROUTE_OK
ENTRY_ROUTE_PARTIAL
ROUTE_OVERLOAD_DETECTED
GATE_CASCADE_BLOCKED
CHECKLIST_FIRST_REPAIR_BLOCKED
SOURCE_REQUIRED_BEFORE_ROUTE
CONTEXT_CAPSULE_REQUIRED_BEFORE_ROUTE
REFERENCE_QUALITY_REQUIRED_FOR_LONGFORM
CORPUS_TOPIC_MAP_REQUIRED_FOR_PACKET
CLAIM_VERIFICATION_REQUIRED_BEFORE_VERDICT
MULTI_CONSTRAINT_LEDGER_REQUIRED_BEFORE_DRAFT
EDITORIAL_HARM_REQUIRED_BEFORE_READINESS
AUTHOR_WRITING_SHEET_REQUIRED_BEFORE_DRAFTING
NARRATIVE_FEATURE_REQUIRED_BEFORE_SURFACE
AUTHOR_VOICE_REQUIRED_BEFORE_DRAFTING
AUTHOR_ALIGNED_DRAFT_SOURCE_REQUIRED
HUMAN_SURFACE_REQUIRED_BEFORE_COPYEDIT
```