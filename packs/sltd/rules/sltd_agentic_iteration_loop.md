# SLTD Agentic Iteration Loop

This rule turns agentic looping into a controlled editorial node cycle.

It does not create automation, scripts, workflows, reports, boards, or self-running agents.

The loop helps the AI continue only inside a named task, named source, named role, and named node.

## Loop shape

```text
MISSION
ANALYZE
PLAN
EXECUTE
EVALUATE
ADJUST
NEXT NODE / STOP
```

## Authority order

The loop sits below:

```text
user current instruction
Notion live source or user-provided current packet
manifest
source preflight
task router
decision safety
role entry card
role boundary contracts
evidence discipline
node checkpoint
```

The loop must not override source, canon, human pass, publication lock, or user write permission.

## MISSION

Define the task before acting.

Required fields:

```text
REQUEST:
SCOPE:
SOURCE LAYER:
ACTIVE ROLE:
OUTPUT TYPE:
WRITE PERMISSION: YES / NO
```

If source, scope, role, or output is unclear, stop and run task intake or role entry check.

## ANALYZE

Read only the sources needed for the smallest safe route.

Check:

- source read;
- current vs legacy status;
- canon risk;
- role boundary;
- evidence requirement;
- context window size;
- blocker scan.

Do not infer current status from memory.

## PLAN

Choose the smallest route.

Required fields:

```text
ROUTE:
BATCH SIZE:
PATCH STRATEGY:
VERIFICATION GATE:
STOP CONDITION:
```

Batch guidance:

```text
1 scene = rewrite unit
1 excerpt = line surgery unit
1 chapter = readiness or rhythm unit
3-10 chapters = packet check
30 chapters = arc check
100+ chapters = map-level review only
```

## EXECUTE

Run the selected task-specific prompt or role route.

Rules:

- execute only the scoped task;
- do not switch roles silently;
- do not write back unless user requested write action;
- do not continue beyond the planned node.

## EVALUATE

Evaluate against the correct gate.

Use:

```text
Evidence gate for source/status/canon/readiness claims
Role boundary gate for role overlap
Line surgery gate for prose smell
Mouth-read check for Vietnamese line naturalness
Webnovel benchmark for pull and momentum
Readiness gate for Human Chapter Pass / Publication Lock
Node checkpoint for handoff and continuation
```

A pass in one gate is not a pass in another.

## ADJUST

If the result fails, choose the smallest safe adjustment:

```text
PATCH_CANDIDATE
ROLE_HANDOFF
SOURCE_REQUEST
REWRITE_RECOMMENDATION
VERIFY_AGAIN
STOP
```

Do not keep patching if a higher-layer failure is found.

Examples:

- Story failure discovered during line edit -> hand back to Story Doctor.
- Canon risk discovered during rewrite -> stop at Canon Guard.
- More than 30 percent line surgery load -> recommend scene rewrite.
- Readiness lacks current lock source -> evidence missing.

## NEXT NODE / STOP

End every loop with one of:

```text
NEXT NODE:
STOP REASON:
USER CONFIRMATION NEEDED:
```

The AI may propose the next node. It may not keep running indefinitely without user permission.

## Fail-closed rules

Stop when:

```text
SOURCE_MISSING
SCOPE_MISSING
ROLE_MISSING
CURRENT_LEGACY_CONFUSION
CANON_CONFLICT_WITHOUT_CURRENT_DECISION
SCENE_BANK_REQUIRED_BUT_MISSING
CHAPTER_LOCK_STATUS_UNCLEAR
PACKET_BLOCKED_BY_UNREADY_CHAPTER
WRITE_PERMISSION_MISSING
TASK_EXCEEDS_CONTEXT_WINDOW
```

## Output

```text
AGENTIC ITERATION LOOP
MISSION:
ANALYZE:
PLAN:
EXECUTE:
EVALUATE:
ADJUST:
NEXT NODE / STOP:
NODE LEDGER:
```
