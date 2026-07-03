# SLTD Entry Route Governance & Gate Budget Protocol

This protocol keeps Entry Fast Path and Task Router usable as routing tools, not diagnostic mazes.

It prevents gate cascade, checklist-first repair, false precision, map bloat, and over-editing caused by running every related gate.

## Core rule

Choose one primary route. Add only necessary secondary gates. Stop when the request is answered.

```text
PRIMARY ROUTE = the smallest route that directly answers the user's request
SECONDARY GATE = a dependent check added only when the primary route exposes a real blocker
GATE BUDGET = the maximum number of gates allowed before the task must stop, report, or ask for source/scope
STOP CONDITION = the point where enough evidence, verdict, map, constraint decision, harm decision, or rewrite output has been produced
GATE CASCADE = running every related gate because it is available rather than required
CHECKLIST-FIRST REPAIR = editing to satisfy gates before reading the scene as lived prose
```

Run a gate only when the request or evidence makes it necessary.

## Use when

- a task could trigger three or more gates;
- context capsule, claim verification, multi-constraint ledger, editorial harm anticipation, corpus topic/thread discovery, tracking, structural, narrative feature, voice, author writing sheet, author voice, author-aligned drafting, surface, human surface polish, readiness, or matrix routes compete for primary route;
- current source, hidden canon, POV knowledge, source-status separation, status claim, canon claim, style claim, task constraint, editorial harm, topic/thread map, readiness claim, lock claim, or long-range continuity could trigger unnecessary downstream gates;
- a prior result feels checklist-first, over-routed, slow, over-polished, map-bloated, over-stylized, structurally too clean, claim-loose, constraint-loose, harm-matrix-overloaded, topic-label-only, style-adjective-only, or over-repaired.

## Authority

This protocol sits below current user instruction, current Notion/source packet, source preflight, required context capsule, source fidelity, decision safety, evidence discipline, and role boundary contracts.

It does not authorize skipping source requirements, canon guard, context capsule, topic evidence anchors, claim evidence, multi-constraint ledger, editorial harm anticipation when REDTEAM/PREMORTEM/high-risk readiness is in scope, narrative-feature blockers, author sample requirements, author writing sheet evidence, author-aligned draft blockers, human surface polish blockers, or readiness evidence.

## Route selection order

```text
1. Classify request type.
2. Identify exact source requirement.
3. Choose one primary route.
4. Add at most the allowed secondary gates.
5. Stop when the stop condition is reached.
6. Report blockers and NEXT NODE instead of expanding scope.
```

If source is missing, the primary route is source preflight or source surface check.

If current source, hidden canon, POV knowledge, source-status separation, or long-range continuity is in scope, run context capsule preflight before later creative, topic/thread discovery, claim verification, multi-constraint ledger, harm anticipation, logic, narrative feature, author writing sheet, author voice, author-aligned drafting, surface, human surface polish, matrix, or readiness gates.

## Primary route triggers

```text
current / latest / Notion / source status / hidden canon / POV knowledge / long-range continuity -> context capsule preflight
TopicGPT / topic map / thread discovery / motif cluster / repeated AI-smell cluster / packet map / arc map / series map -> corpus topic thread discovery check
claim / true false / false twin / CLIPPER / đúng sai / canon claim / continuity claim / source conflict -> narrative claim verification check
multi-constraint / Suri / constraint ledger / corrupted constraint / ràng buộc / giữ nhiều điều cùng lúc -> multi-constraint instruction check
AHA / harm / REDTEAM / PREMORTEM / false readiness / reveal leak / over-polish harm / failure vignette -> editorial harm anticipation check
Author Writing Sheet / claim-evidence style memory / style claim evidence / prompt-specific story rules -> author writing sheet check
rewrite / sửa cảnh -> scene rewrite or first-pass editorial workflow, with multi-constraint ledger when more than one controlling constraint exists and harm anticipation when failure cost is high
line / câu / đoạn -> line surgery
StoryScope / narrative feature / structural AI smell / theme quá rõ / nhân quả quá sạch / tuyến đơn / reread value -> narrative feature audit
author voice / voice DNA / style guide / giọng tôi / giống giọng / học cách viết -> author voice fingerprint check
ghostwriter / viết thay / viết theo giọng tôi / draft như tôi -> author aligned ghostwriter draft
human surface / humanize / polish / đúng mà giả / mượt giả / văn nghe AI nhưng đúng ý -> human surface polish pass
readiness / lock / pass -> readiness route, with claim verification, multi-constraint ledger, and harm anticipation for status/lock risk
packet / arc / C001-C030 -> packet/arc review, with corpus topic/thread discovery only when map-level navigation is requested
```

## Gate budget

```text
Simple advisory answer:
- 1 primary route
- 0-1 secondary gate

Corpus topic / thread discovery:
- context brief for packet/arc/part/series scope
- source preflight or source surface when current/source-status topic assignment is required
- context capsule when hidden canon, POV knowledge, source-status separation, reveal timing, or long-range continuity is in scope
- corpus topic/thread discovery
- claim verification only if a topic assignment depends on factual/status/canon evidence
- tracking ledger only if thread state/object/payoff debt is in scope
- narrative feature audit only if repeated structural AI smell or narrative diversity is the blocker
- harm anticipation only if topic/thread drift creates downstream harm
- return top clusters/topic gaps unless user asks for full map
- stop before rewrite/readiness/lock; topic maps do not grant those permissions

Editorial harm anticipation:
- source preflight or source surface when exact/current status or output anchor is required
- context capsule when current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
- claim verification only if a harm depends on factual/status/canon evidence
- multi-constraint ledger only if constraints control output or harm prevention
- corpus topic/thread discovery only if harm is map-level topic/thread drift
- harm matrix, top 3 harms by severity unless full matrix is requested

Context capsule preflight:
- source preflight or source surface check when exact/current status is required
- context capsule preflight
- claim verification only if the capsule contains a testable current/status/canon/continuity claim
- multi-constraint ledger only if downstream output must preserve multiple constraints
- harm anticipation only if REDTEAM/PREMORTEM/readiness/lock/large rewrite harm risk is in scope
- corpus topic/thread discovery only if packet/arc/series map-level navigation is in scope
- author writing sheet only if a style claim controls the route

Narrative claim verification:
- source preflight or source surface when exact/current status is required
- context capsule preflight if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, claim anchor, or long-range continuity is in scope
- compressed source may be used only to locate evidence
- narrative claim verification
- corpus topic/thread discovery only if the claim concerns topic/thread assignment
- stop with TRUE / FALSE / UNCERTAIN; do not continue into readiness, polish, or rewrite from claim verification alone

Multi-constraint instruction ledger:
- source preflight or source surface when exact/current status or output anchor is required
- context capsule preflight when current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
- claim verification only if a constraint depends on factual/status/canon evidence
- corpus topic/thread discovery only if constraints come from packet/arc/series topic/thread map
- multi-constraint ledger

Author-aligned drafting:
- source surface or current scene packet
- context capsule preflight when current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
- claim verification if draft depends on a status/canon/continuity/POV/object/reveal claim
- multi-constraint ledger for source/canon/POV/scene/style/surface/wordcount constraints
- harm anticipation if the draft has high REDTEAM/PREMORTEM risk
- author writing sheet if style memory or prompt-specific story rules are used
- bounded draft

Chapter readiness:
- source surface / current Notion if current status is asked
- context capsule preflight before status/pass verdict when current source, hidden canon, POV knowledge, or source-status separation is in scope
- claim verification for Human Chapter Pass / Publication Lock / packet lock / source-conflict claims
- multi-constraint ledger for readiness constraints and corrupted constraints
- harm anticipation for false readiness / lock / downstream harm vignettes
- corpus topic/thread discovery only if packet/arc thread map is explicitly requested
- readiness reviewer
```

A secondary gate must be justified by a blocker, not by association.

## Stop conditions

Stop when:

```text
source is missing or current source was not read for a current-status claim;
context capsule blocks because POV knowledge, hidden canon, source status, object state, or long-range context is unclear;
topic/thread discovery blocks because scope, source, quote/evidence anchor, or current assignment evidence is missing;
topic map tries to delete low-frequency topic without canon/reveal/payoff check;
topic map is being used as readiness, lock, canon verdict, or rewrite permission;
claim verification returns UNCERTAIN because evidence, exact source, anchor, or false twin is missing;
claim verification proves a readiness/lock/status claim false;
multi-constraint ledger blocks because constraints are missing, corrupted constraints are missing, output anchors are missing, or constraints conflict;
harm anticipation blocks because scope/source/impact target/failure behavior is missing, harm depends on unverified claim, vignette would invent canon, or matrix overload hides the top blocker;
author writing sheet blocks because style evidence, approved samples, category coverage, or task fit is missing;
narrative feature audit blocks because story-decision AI smell, theme overexplicitness, causal tidiness, weak reveal, or decorative sensory pressure remains unresolved;
primary blocker has been identified and next node is clear;
additional gates would be speculative;
secondary gate budget has been spent.
```

## No-cascade rule

Do not run this chain by default:

```text
topic map -> transition -> timeline -> craft -> composition -> beat -> living world -> character -> layout -> register -> scene-first -> anti-AI -> agency -> dynamic range
```

Use only the nodes required by the primary blocker.

## Checklist-first repair prevention

Before patching, name:

```text
PRIMARY BLOCKER:
PRIMARY ROUTE:
GATE BUDGET:
STOP CONDITION:
```

If the edit begins to add topic mapping, claim verification, multi-constraint ledger, harm matrix, author writing sheet, body, object, silence, rumor, beat, world texture, character gesture, line-break changes, author voice imitation, author-aligned drafting, narrative-feature repair, and human-surface polish all at once, stop and run Anti-AI Composite or Scene-First Prose Judgment.

## Failure labels

```text
ROUTE_OVERLOAD
GATE_CASCADE_RISK
CHECKLIST_FIRST_REPAIR_RISK
PRIMARY_ROUTE_UNCLEAR
SECONDARY_GATE_OVERUSE
STOP_CONDITION_MISSING
SOURCE_SURFACE_FORGOTTEN
CONTEXT_CAPSULE_FORGOTTEN
CORPUS_TOPIC_MAP_FORGOTTEN
TOPIC_WITHOUT_EVIDENCE
SUMMARY_ONLY_TOPIC_RISK
LOW_FREQUENCY_IMPORTANT_UNCHECKED
CLAIM_VERIFICATION_FORGOTTEN
FALSE_TWIN_FORGOTTEN
MULTI_CONSTRAINT_LEDGER_FORGOTTEN
CORRUPTED_CONSTRAINT_FORGOTTEN
EDITORIAL_HARM_MATRIX_FORGOTTEN
HARM_OVERLOAD_RISK
VIGNETTE_CANON_DRIFT
CONSTRAINT_CONFLICT_IGNORED
AUTHOR_WRITING_SHEET_FORGOTTEN
STYLE_CLAIM_WITHOUT_EVIDENCE
STRUCTURAL_AI_SMELL_IGNORED
MAP_USED_AS_READINESS
MAP_USED_AS_REWRITE_PERMISSION
FALSE_PRECISION_ROUTE
PATCH_OVERFITTING
EDITORIAL_LATENCY_RISK
```

## Safe repair

Safe repair may:

- select one primary route;
- reduce route chain to the smallest useful path;
- cap secondary gates;
- state stop condition before editing;
- route TopicGPT-style packet/arc/series requests to Corpus Topic / Thread Discovery with quote/evidence anchors;
- mark low-frequency topics as important/uncertain instead of deleting them;
- route disputed status/canon/continuity claims to Narrative Claim Verification before prose, readiness, or lock;
- route multi-constraint rewrite/draft/polish/readiness tasks to Multi-Constraint Instruction Ledger before output;
- route REDTEAM/PREMORTEM/readiness/lock/large-rewrite risk to Editorial Harm Anticipation and return top 3 harms when overloaded;
- route StoryScope/narrative feature requests to Narrative Feature Audit before surface repair;
- route author-aligned drafting only after source, scene controls, claim verification when needed, multi-constraint ledger when needed, harm anticipation when needed, author writing sheet when needed, and author fingerprint are clear.

Safe repair must not:

- drop required source checks;
- skip context capsule when current source, hidden canon, POV knowledge, source-status separation, or long-range continuity is at stake;
- create topic maps without quote/evidence anchors;
- delete low-frequency topics without canon/reveal/payoff check;
- use topic map as source truth, readiness, lock, canon verdict, or rewrite permission;
- skip claim verification when a factual/canon/status/readiness claim controls the route;
- skip Multi-Constraint Instruction Ledger when multiple constraints control output;
- skip Editorial Harm Anticipation when REDTEAM/PREMORTEM/readiness/lock/high-risk failure vignette is the primary blocker;
- continue running gates after a stop condition;
- create scripts, workflows, reports, issues, boards, or project-management files.

## Route governance audit

```text
ENTRY ROUTE GOVERNANCE CHECK
SCOPE:
SOURCE USED:
REQUEST TYPE:
SOURCE REQUIREMENT:
CONTEXT CAPSULE REQUIREMENT:
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