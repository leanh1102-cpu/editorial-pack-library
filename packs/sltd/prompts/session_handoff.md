# SLTD Session Handoff

Use this prompt when ending a long task, when context window is degrading, or when the next chat may need to continue.

## Purpose

Create a continuity handoff that survives context-window loss and prevents the next AI from carrying forward unverified memory, rejected output, or compressed source.

This handoff is navigation and task state. It is not source text, not canon, not readiness evidence, and not permission to change source files.

## Required reading

```text
prompts/boot_task.md
rules/sltd_handoff_continuity_protocol.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_evidence_discipline.md
rules/sltd_role_boundary_contracts.md
prompts/node_checkpoint.md
current task output
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
1. Read manifest version named in this handoff.
2. Read this handoff as navigation, not source truth.
3. Verify current source before current-state verdict.
4. Continue only at NEXT NODE unless user changes scope.
5. Run source surface check before prose patch or readiness claim.
6. Respect role boundary and do-not-carry items.
7. Change Notion or GitHub only if the user explicitly asks.

HANDOFF STATUS: HANDOFF_SAFE / HANDOFF_PARTIAL / HANDOFF_UNSAFE_SOURCE_MISSING / HANDOFF_UNSAFE_ROLE_MISSING / HANDOFF_UNSAFE_NEXT_NODE_MISSING / HANDOFF_UNSAFE_VERDICT_FROM_MEMORY
```

## Rules

- Keep handoff compact but complete enough to restart the next node safely.
- Name exact nodes, not vague summaries.
- Separate FACT, INFERENCE, RECOMMENDATION, CANDIDATE, and UNVERIFIED.
- Do not store live manuscript text unless the user asks.
- Do not treat digest as source text.
- Do not mark a chapter locked unless current Notion supports it.
- If source was not read, mark it `NOT READ` and `MUST RE-READ BEFORE VERDICT`.
- If exact source surface was not available, mark compression risk and forbid prose patch.
- If an output was rejected, record it in ERROR LEDGER and DO NOT CARRY.
- If next node is unclear, mark `HANDOFF_UNSAFE_NEXT_NODE_MISSING`.
