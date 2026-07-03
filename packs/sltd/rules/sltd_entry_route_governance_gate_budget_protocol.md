# SLTD Entry Route Governance & Gate Budget Protocol

This protocol keeps Entry Fast Path and Task Router usable as routing tools, not diagnostic mazes.

It prevents gate cascade, checklist-first repair, false precision, and over-editing caused by running every related gate.

## Core rule

Choose one primary route. Add only necessary secondary gates. Stop when the request is answered.

```text
PRIMARY ROUTE = the smallest route that directly answers the user's request
SECONDARY GATE = a dependent check added only when the primary route exposes a real blocker
GATE BUDGET = the maximum number of gates allowed before the task must stop, report, or ask for source/scope
STOP CONDITION = the point where enough evidence, verdict, or rewrite output has been produced
GATE CASCADE = running every related gate because it is available rather than required
CHECKLIST-FIRST REPAIR = editing to satisfy gates before reading the scene as lived prose
```

Run a gate only when the request or evidence makes it necessary.

## Use when

- the user asks whether Entry is too large, confusing, or likely to cause route chaos;
- a task could trigger three or more gates;
- context capsule, claim verification, tracking, structural, narrative feature, voice, author writing sheet, author voice, author-aligned drafting, surface, human surface polish, readiness, or matrix routes compete for primary route;
- current source, hidden canon, POV knowledge, source-status separation, status claim, canon claim, style claim, readiness claim, lock claim, or long-range continuity could trigger unnecessary downstream gates;
- a prior result feels checklist-first, over-routed, slow, over-polished, over-stylized, structurally too clean, claim-loose, style-adjective-only, or over-repaired;
- source is missing and the agent is tempted to keep analyzing from memory.

## Authority

This protocol sits below:

```text
current user instruction
current Notion source or user-provided source packet
source preflight
context capsule preflight when current source, hidden canon, POV knowledge, source-status separation, or long-range continuity is in scope
source fidelity gate
decision safety
evidence discipline
role boundary contracts
```

It does not authorize skipping source requirements, canon guard, context capsule, claim evidence, narrative-feature blockers, author sample requirements, author writing sheet evidence, author-aligned draft blockers, human surface polish blockers, or readiness evidence.

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

If current source, hidden canon, POV knowledge, source-status separation, or long-range continuity is in scope, run context capsule preflight before later creative, claim verification, logic, narrative feature, author writing sheet, author voice, author-aligned drafting, surface, human surface polish, matrix, or readiness gates.

## Primary route triggers

```text
current / latest / Notion / source status / hidden canon / POV knowledge / long-range continuity -> context capsule preflight
claim / true false / false twin / CLIPPER / đúng sai / canon claim / continuity claim / source conflict -> narrative claim verification check
Author Writing Sheet / claim-evidence style memory / style claim evidence / prompt-specific story rules -> author writing sheet check
rewrite / sửa cảnh -> scene rewrite or first-pass editorial workflow
line / câu / đoạn -> line surgery
StoryScope / narrative feature / structural AI smell / theme quá rõ / nhân quả quá sạch / tuyến đơn / reread value -> narrative feature audit
author voice / voice DNA / style guide / giọng tôi / giống giọng / học cách viết -> author voice fingerprint check
ghostwriter / viết thay / viết theo giọng tôi / draft như tôi -> author aligned ghostwriter draft
human surface / humanize / polish / đúng mà giả / mượt giả / văn nghe AI nhưng đúng ý -> human surface polish pass
readiness / lock / pass -> readiness route, with claim verification for status claims
packet / arc / C001-C030 -> chapter/packet/arc review
```

## Gate budget

```text
Simple advisory answer:
- 1 primary route
- 0-1 secondary gate

Context capsule preflight:
- source preflight or source surface check when exact/current status is required
- context capsule preflight
- claim verification only if the capsule contains a testable current/status/canon/continuity claim
- author writing sheet only if a style claim controls the route
- 0-2 dependent gates only when capsule exposes a real blocker

Narrative claim verification:
- source preflight or source surface when exact/current status is required
- context capsule preflight if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, claim anchor, or long-range continuity is in scope
- compressed source may be used only to locate evidence
- narrative claim verification
- stop with TRUE / FALSE / UNCERTAIN; do not continue into readiness, polish, or rewrite from claim verification alone

Author writing sheet:
- approved/current author samples or AUTHOR_TASTE_EXAMPLES / AUTHOR_WORKING_PROFILE
- author writing sheet check
- 0-1 dependent gate only if a style claim depends on source/canon evidence, character voice, or exact Vietnamese surface
- stop if samples are missing, unapproved, generated-only, legacy-only, chat-memory-only, or style-adjective-only

Author voice fingerprint:
- approved/current author samples or AUTHOR_TASTE_EXAMPLES / AUTHOR_WORKING_PROFILE
- author writing sheet first if style claims need evidence
- author voice fingerprint check
- 0-1 dependent gate only if dialogue/character voice or Vietnamese surface is the comparison issue

Author-aligned drafting:
- source surface or current scene packet
- context capsule preflight when current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
- claim verification if draft depends on a status/canon/continuity/POV/object/reveal claim
- author writing sheet if style memory or prompt-specific story rules are used
- narrative feature audit only if draft risk includes theme overexplained, causal tidiness, single-track plot, weak reveal, or decorative sensory pressure
- structural/tracking/voice gate only if scene function, state, or character voice is unclear
- bounded draft
- human surface polish only if synthetic-surface risk remains
- stop before draft if source/canon/scene controls or author samples are missing

Human surface polish:
- source surface check when exact prose is patched
- context capsule preflight if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
- claim verification if patch depends on a factual/canon/continuity claim
- narrative feature audit if polish may hide structural AI smell or decorative body/sensory overperformance
- author writing sheet only if style memory is used for polish
- stop before copyedit/readiness if repair load exceeds 30 percent, source is missing, story-decision smell remains, or polishing would change scene function/canon/outcome

Chapter readiness:
- source surface / current Notion if current status is asked
- context capsule preflight before status/pass verdict when current source, hidden canon, POV knowledge, or source-status separation is in scope
- claim verification for Human Chapter Pass / Publication Lock / packet lock / source-conflict claims
- narrative feature audit if false readiness may come from clean-but-AI-shaped story structure
- author writing sheet only as style evidence, never as readiness evidence
- readiness reviewer
```

A secondary gate must be justified by a blocker, not by association.

## Stop conditions

Stop when:

```text
source is missing or current source was not read for a current-status claim;
context capsule blocks because POV knowledge, hidden canon, source status, object state, or long-range context is unclear;
claim verification returns UNCERTAIN because evidence, exact source, anchor, or false twin is missing;
claim verification proves a readiness/lock/status claim false;
author writing sheet blocks because style evidence, approved samples, category coverage, or task fit is missing;
narrative feature audit blocks because story-decision AI smell, theme overexplicitness, causal tidiness, weak reveal, or decorative sensory pressure remains unresolved;
author samples are missing, unapproved, generated-only, legacy-only, or chat-memory-only;
author-aligned drafting would invent canon, scene function, object, relation, route, payoff, or reveal timing;
primary blocker has been identified and next node is clear;
requested rewrite or patch is complete within scope;
readiness is blocked by a higher-priority gate;
additional gates would be speculative;
additional repair would invent canon, timeline, folklore, motive, or source surface;
human surface polish would smooth away body/object pressure, relationship memory, or useful roughness;
secondary gate budget has been spent.
```

## No-cascade rule

Do not run this chain by default:

```text
transition -> timeline -> craft -> composition -> beat -> living world -> character -> layout -> register -> scene-first -> anti-AI -> agency -> dynamic range
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

If the edit begins to add claim verification, author writing sheet, body, object, silence, rumor, beat, world texture, character gesture, line-break changes, author voice imitation, author-aligned drafting, narrative-feature repair, and human-surface polish all at once, stop and run Anti-AI Composite or Scene-First Prose Judgment.

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
CLAIM_VERIFICATION_FORGOTTEN
FALSE_TWIN_FORGOTTEN
AUTHOR_WRITING_SHEET_FORGOTTEN
STYLE_CLAIM_WITHOUT_EVIDENCE
STRUCTURAL_AI_SMELL_IGNORED
AUTHOR_SAMPLE_FORGOTTEN
AUTHOR_ALIGNED_DRAFT_PERMISSION_FORGOTTEN
AUTHOR_VOICE_OVER_CHARACTER_VOICE
HUMAN_SURFACE_OVERPOLISH_RISK
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
- require context capsule before downstream gates when current source, hidden canon, POV knowledge, or long-range continuity is in scope;
- route disputed status/canon/continuity claims to Narrative Claim Verification before prose, readiness, or lock;
- route StoryScope/narrative feature requests to Narrative Feature Audit before surface repair;
- route author-style claim requests to Author Writing Sheet before fingerprint/drafting;
- route author voice requests to fingerprint check after style evidence is clear;
- route author-aligned drafting only after source, scene controls, claim verification when needed, author writing sheet when needed, and author fingerprint are clear;
- route correct-but-synthetic prose to Human Surface Polish only after source, claim verification, narrative feature, style evidence when used, and prose permission are clear.

Safe repair must not:

- drop required source checks;
- skip context capsule when current source, hidden canon, POV knowledge, source-status separation, or long-range continuity is at stake;
- skip claim verification when a factual/canon/status/readiness claim controls the route;
- skip Author Writing Sheet when author-style claims control the route;
- skip narrative feature audit when story-decision AI smell is the primary blocker;
- use author style match to invent source truth, override character voice, or call readiness;
- use human surface polish to hide story failure or smooth away survival pressure;
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
CLAIM VERIFICATION REQUIREMENT:
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

## Handoff

If source is missing, hand off to Source Preflight or Source Surface Check.

If current source, hidden canon, POV knowledge, source-status separation, or long-range continuity is in scope, hand off to Context Capsule Preflight before downstream gates.

If a claim is true/false/current/canon/ready/locked, hand off to Narrative Claim Verification before prose/readiness/lock.

If the task asks for Author Writing Sheet, claim-evidence style memory, sample-backed author profile, or prompt-specific story rules, hand off to Author Writing Sheet Check.

If the task asks for author voice, voice DNA, style guide, or voice match, hand off to Author Voice Fingerprint Check after evidence/source gaps are clear.

If the task asks for author-aligned drafting, hand off to Author-Aligned Draft only after current source, scene controls, claim verification when relevant, narrative feature blockers when relevant, author writing sheet when relevant, and author fingerprint are clear.

## Output labels

```text
ENTRY_ROUTE_OK
ENTRY_ROUTE_PARTIAL
ROUTE_OVERLOAD_DETECTED
GATE_CASCADE_BLOCKED
CHECKLIST_FIRST_REPAIR_BLOCKED
SOURCE_REQUIRED_BEFORE_ROUTE
CONTEXT_CAPSULE_REQUIRED_BEFORE_ROUTE
CLAIM_VERIFICATION_REQUIRED_BEFORE_VERDICT
AUTHOR_WRITING_SHEET_REQUIRED_BEFORE_DRAFTING
NARRATIVE_FEATURE_REQUIRED_BEFORE_SURFACE
AUTHOR_VOICE_REQUIRED_BEFORE_DRAFTING
AUTHOR_ALIGNED_DRAFT_SOURCE_REQUIRED
HUMAN_SURFACE_REQUIRED_BEFORE_COPYEDIT
```