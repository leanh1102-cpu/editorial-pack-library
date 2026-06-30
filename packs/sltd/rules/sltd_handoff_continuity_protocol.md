# SLTD Handoff Continuity Protocol

This rule turns handoff into a continuity-preserving transfer, not a loose session summary.

It protects active work when context window degrades, the model becomes unreliable, or the task must move to a new AI session.

## Core rule

A handoff is a navigation and state-transfer document.

It is not source text, not canon, not current manuscript, not proof of readiness, and not permission to write.

The next AI must use the handoff to find the next node, then verify current source before making verdicts or patches.

## Use when

- the context window is near limit;
- answers become vague, laggy, contradictory, or over-compressed;
- a long task must continue in another chat;
- a packet/chapter/scene pass has open loops;
- user wants the next AI to inherit work safely;
- an output was rejected and the next AI must not repeat it.

## Authority order

Handoff sits below:

```text
user current instruction
current Notion source
user-provided current packet
source fidelity gate
evidence discipline
role boundary contracts
node checkpoint
```

Handoff may preserve task state. It must not override current source, canon, human pass, publication lock, or user write permission.

## Handoff must separate

```text
FACT = source/node/action actually read or performed
INFERENCE = reasoned conclusion from source, not final truth
RECOMMENDATION = proposed next action
CANDIDATE = possible update or patch not yet applied
UNVERIFIED = memory, digest, or claim that must be re-read
```

If the handoff cannot separate these, mark it unsafe.

## Carry / do not carry

Every handoff must include:

```text
CARRY FORWARD:
- verified source read
- active scope
- current route
- active role
- node ledger
- evidence-backed blocker
- approved calibration or patch candidate
- next node

DO NOT CARRY:
- current status from memory
- inferred canon
- unverified readiness
- prose patch without exact OLD
- digest treated as source
- rejected output
- old Workdeck as current source unless named current
```

## Required ledgers

### Source ledger

Track source state:

```text
CURRENT SOURCE READ:
EXACT SOURCE TEXT READ:
DERIVED DIGEST — NOT SOURCE TEXT:
LEGACY REFERENCE:
CHAT MEMORY USED ONLY FOR ORIENTATION:
NOT READ:
MUST RE-READ BEFORE VERDICT:
SOURCE SURFACE STATUS:
COMPRESSION RISK:
```

### Role ledger

Track role state:

```text
ACTIVE ROLE:
ROLE CARD READ:
ROLE BOUNDARY STATUS:
ROLES RUN:
ROLES NOT RUN:
ROLE PASSED:
ROLE FAILED OR BLOCKED:
HANDOFF TO:
```

### Node ledger

Track work state:

```text
DONE:
PASSED:
NOT PASSED:
BLOCKED BY:
OPEN LOOPS:
NEXT NODE:
```

### Decision ledger

Track truth type:

```text
FACT:
INFERENCE:
RECOMMENDATION:
CANDIDATE ONLY:
UNVERIFIED:
```

### Patch ledger

Track patch state:

```text
PATCH APPLIED:
PATCH CANDIDATE:
EXACT OLD VERIFIED:
NOT APPLIED:
PATCH BLOCKED BY:
```

### Error ledger

Track errors to avoid:

```text
REJECTED OUTPUT:
WHY REJECTED:
RULE HIT:
DO NOT REPEAT:
CALIBRATION CANDIDATE:
INVALIDATED CLAIM:
```

## Next AI boot block

Every continuity handoff must include:

```text
NEXT AI MUST:
1. Read manifest version named in this handoff.
2. Read this handoff as navigation, not source truth.
3. Verify current source before current-state verdict.
4. Continue only at NEXT NODE unless user changes scope.
5. Run source surface check before prose patch or readiness claim.
6. Respect role boundary and do-not-carry items.
7. Do not write to Notion/GitHub unless user explicitly asks.
```

## Unsafe handoff labels

Use these when needed:

```text
HANDOFF_SAFE
HANDOFF_PARTIAL
HANDOFF_UNSAFE_SOURCE_MISSING
HANDOFF_UNSAFE_ROLE_MISSING
HANDOFF_UNSAFE_NEXT_NODE_MISSING
HANDOFF_UNSAFE_VERDICT_FROM_MEMORY
```

## Output

```text
SLTD CONTINUITY HANDOFF
PACK VERSION:
DATE:
SESSION TYPE:
SCOPE:
TASK:
USER INTENT:

SOURCE LEDGER:
- CURRENT SOURCE READ:
- EXACT SOURCE TEXT READ:
- DERIVED DIGEST — NOT SOURCE TEXT:
- LEGACY REFERENCE:
- CHAT MEMORY USED ONLY FOR ORIENTATION:
- NOT READ:
- MUST RE-READ BEFORE VERDICT:
- SOURCE SURFACE STATUS:
- COMPRESSION RISK:

ROLE LEDGER:
- ACTIVE ROLE:
- ROLE CARD READ:
- ROLE BOUNDARY STATUS:
- ROLES RUN:
- ROLES NOT RUN:
- ROLE PASSED:
- ROLE FAILED OR BLOCKED:
- HANDOFF TO:

NODE LEDGER:
- DONE:
- PASSED:
- NOT PASSED:
- BLOCKED BY:
- OPEN LOOPS:
- NEXT NODE:

DECISION LEDGER:
- FACT:
- INFERENCE:
- RECOMMENDATION:
- CANDIDATE ONLY:
- UNVERIFIED:

PATCH LEDGER:
- PATCH APPLIED:
- PATCH CANDIDATE:
- EXACT OLD VERIFIED:
- NOT APPLIED:
- PATCH BLOCKED BY:

ERROR LEDGER:
- REJECTED OUTPUT:
- WHY REJECTED:
- RULE HIT:
- DO NOT REPEAT:
- CALIBRATION CANDIDATE:
- INVALIDATED CLAIM:

CARRY FORWARD:
- ...

DO NOT CARRY:
- ...

NEXT AI MUST:
1.
2.
3.

HANDOFF STATUS:
```

## Stop rule

Do not create a continuity handoff that pretends to know source it did not read.

If source was not read, mark it under `NOT READ` and `MUST RE-READ BEFORE VERDICT`.

If next node is unclear, mark `HANDOFF_UNSAFE_NEXT_NODE_MISSING` and ask for scope clarification.
