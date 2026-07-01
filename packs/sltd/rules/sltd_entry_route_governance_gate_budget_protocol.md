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

Do not run a gate because it is adjacent.

Run a gate only when the request or evidence makes it necessary.

## Use when

- the user asks whether Entry is too large, confusing, or likely to cause route chaos;
- a task could trigger three or more gates;
- a rewrite/readiness/packet request risks becoming a full diagnostic cascade;
- the agent is unsure whether to run scene transition, timeline, craft, composition, beat, living world, character, register, layout, agency, dynamic range, or anti-AI checks;
- a prior result feels checklist-first, over-routed, slow, or over-repaired;
- source is missing and the agent is tempted to keep analyzing from memory;
- a task needs route selection before editorial work begins.

## Authority

This protocol sits below:

```text
current user instruction
current Notion source or user-provided source packet
source preflight
source fidelity gate
decision safety
evidence discipline
role boundary contracts
```

It does not override a user's explicit request to run a named mode or gate.

It does not authorize skipping source requirements, canon guard, or readiness evidence.

## Route selection order

Use this order:

```text
1. Classify request type.
2. Identify exact source requirement.
3. Choose one primary route.
4. Add at most the allowed secondary gates.
5. Stop when the stop condition is reached.
6. Report blockers and NEXT NODE instead of expanding scope.
```

If the source is missing, the primary route is source preflight or source surface check. Do not continue into creative gates.

## Primary route triggers

Use the user's strongest noun or verb as the primary route:

```text
rewrite / sửa cảnh -> scene rewrite or first-pass editorial workflow
line / câu / đoạn -> line surgery
readiness / lock / pass -> readiness route
packet / arc / C001-C030 -> chapter/packet/arc review
timeline / POV / phục bút / folklore -> timeline POV foreshadowing folklore check
chuyển cảnh / skiptime / nối cảnh -> scene transition skiptime event cluster check
beat / cao trào / hậu chấn -> narrative beat escalation check
thành phần cảnh / tỷ lệ -> scene composition balance check
world / cộng đồng / phong tục -> living world community motion check
nhân vật bị lướt / đổi tên vẫn dùng được -> character distinctiveness check
OOC / OCC / nhân vật bị ép plot -> character agency check
văn dịch Trung / Hán Việt / Việt Đạo -> Vietnamese register check
line break / mobile / đoạn ngắn -> webnovel paragraphing layout check
văn AI / checklist / đúng mà giả -> anti-AI composite or scene-first prose judgment
kỹ thuật viết / chất liệu / phong cách -> prose craft style check
```

## Gate budget

Use these budgets unless the user explicitly requests a broader audit:

```text
Simple advisory answer:
- 1 primary route
- 0-1 secondary gate

Line surgery:
- source surface check
- 1 primary blocker
- 0-1 secondary dependency

Scene rewrite:
- source surface check
- first-pass editorial workflow
- 1 primary target gate
- up to 2 secondary gates

Chapter readiness:
- source surface / current Notion if current status is asked
- chapter assembly if reader unit is in scope
- up to 3 issue-specific checks
- readiness reviewer

Packet / arc review:
- context brief
- source preflight
- 2-4 map-level checks
- no line edit unless requested

Current lock / canon / publication status:
- current Notion or exact provided source
- relevant status route only
- stop if evidence is missing
```

A secondary gate must be justified by a blocker, not by association.

## Stop conditions

Stop when:

```text
source is missing or current source was not read for a current-status claim;
primary blocker has been identified and next node is clear;
requested rewrite or patch is complete within scope;
readiness is blocked by a higher-priority gate;
additional gates would be speculative;
additional repair would invent canon, timeline, folklore, motive, or source surface;
secondary gate budget has been spent;
user asked for a specific answer and the answer is complete.
```

Do not continue for coverage after a stop condition is met.

## No-cascade rule

Do not run this chain by default:

```text
transition -> timeline -> craft -> composition -> beat -> living world -> character -> layout -> register -> scene-first -> anti-AI -> agency -> dynamic range
```

Use only the nodes required by the primary blocker.

If three or more gates seem necessary, create a context brief and ask whether the user wants a broad audit, or return a prioritized NODE LEDGER.

## Checklist-first repair prevention

Before patching, name:

```text
PRIMARY BLOCKER:
PRIMARY ROUTE:
GATE BUDGET:
STOP CONDITION:
```

If the edit begins to add body, object, silence, rumor, beat, world texture, character gesture, and line-break changes all at once, stop and run Anti-AI Composite or Scene-First Prose Judgment.

## Failure labels

Use these labels:

```text
ROUTE_OVERLOAD
GATE_CASCADE_RISK
CHECKLIST_FIRST_REPAIR_RISK
PRIMARY_ROUTE_UNCLEAR
SECONDARY_GATE_OVERUSE
STOP_CONDITION_MISSING
SOURCE_SURFACE_FORGOTTEN
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
- convert a broad request into context brief plus next node;
- mark missing source instead of running gates from memory;
- hand off to the one route that owns the primary blocker.

Safe repair must not:

- drop required source checks;
- skip canon guard when canon is at stake;
- ignore explicit user-requested review modes;
- use budget rules to avoid a necessary blocker;
- continue running gates after a stop condition;
- create scripts, workflows, reports, issues, boards, or project-management files.

## Route governance audit

Use:

```text
ENTRY ROUTE GOVERNANCE CHECK
SCOPE:
SOURCE USED:
REQUEST TYPE:
SOURCE REQUIREMENT:
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

If current status, lock, readiness, or canon is requested, hand off to current Notion/source-specific route before verdict.

If the task asks for a broad packet/arc review, hand off to Context Brief and Packet Review.

If the task asks for prose repair, hand off to First-Pass Editorial Workflow with a declared primary blocker.

## Output labels

```text
ENTRY_ROUTE_OK
ENTRY_ROUTE_PARTIAL
ROUTE_OVERLOAD_DETECTED
GATE_CASCADE_BLOCKED
CHECKLIST_FIRST_REPAIR_BLOCKED
SOURCE_REQUIRED_BEFORE_ROUTE
```