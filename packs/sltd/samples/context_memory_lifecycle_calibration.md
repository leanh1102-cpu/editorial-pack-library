# SLTD Context Memory Lifecycle Calibration

These samples calibrate ByteRover-style context memory lifecycle discipline for SLTD.

They are not source truth and are not manuscript memory.

## 1. Stale handoff as current source

```text
BAD PATTERN:
The agent reads an old handoff and says C030 is ready.

WHY BAD:
Readiness and Human Chapter Pass require current source/status. Handoff is not live source.

EXPECTED OUTPUT:
STALE_HANDOFF_RISK
CONTEXT_MEMORY_NEEDS_SOURCE
DECISION: BLOCK
```

## 2. Checked but stale

```text
PATTERN:
A context entry was source-checked last session, but Notion may have changed.

EXPECTED OUTPUT:
MATURITY: CHECKED
RECENCY: POSSIBLY STALE
MUST RE-READ BEFORE: current readiness, lock, canon conflict, exact prose verdict
DECISION: KEEP AS ROUTE HINT, not source truth
```

## 3. Stable rule memory

```text
PATTERN:
Rule says Workdeck is legacy unless explicitly named current.

EXPECTED OUTPUT:
ENTRY TYPE: ROUTE / SOURCE POLICY
MATURITY: STABLE
SOURCE-TRUTH LIMIT: applies to routing, not manuscript content
DECISION: KEEP
```

## 4. Chat memory source-truth risk

```text
BAD PATTERN:
The agent says a scene contains a motif because it remembers a prior chat.

EXPECTED OUTPUT:
CHAT_MEMORY_SOURCE_TRUTH_RISK
SOURCE_RECHECK_REQUIRED
DECISION: BLOCK until source retrieval/source surface
```

## 5. Feedback delta reuse

```text
PATTERN:
The user previously said 'cảnh đúng nhưng mỏng.'

EXPECTED OUTPUT:
ENTRY TYPE: FEEDBACK
MATURITY: RAW unless converted by feedback delta check
RETRIEVAL USE: may guide rewrite only after target scope/source is clear
NEXT NODE: comparative_editorial_feedback_delta_check
```

## 6. Deprecated AI verdict

```text
BAD PATTERN:
An AI readiness score says a chapter passed, but later human read invalidated the pass.

EXPECTED OUTPUT:
MATURITY: DEPRECATED
STALE MEMORY RISK: HIGH
DECISION: DEPRECATE
PROHIBIT: using old AI score as readiness
```

## 7. GitHub live manuscript memory risk

```text
BAD PATTERN:
The agent proposes copying current Notion manuscript scenes into GitHub as memory files.

EXPECTED OUTPUT:
NO_GITHUB_LIVE_MANUSCRIPT_MEMORY
DECISION: BLOCK
SAFE REPAIR: store only rule memory or non-source handoff metadata with provenance
```

## 8. Context entry with provenance

```text
GOOD PATTERN:
The handoff says a branch was merged, cites PR number and merge commit, and is only used to choose next GitHub node.

EXPECTED OUTPUT:
PROVENANCE: PR / merge commit / timestamp
MATURITY: CHECKED or STABLE for repo state at that point
SOURCE-TRUTH LIMIT: GitHub state only, not manuscript status
DECISION: KEEP
```