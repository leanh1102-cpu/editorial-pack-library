# SLTD Corpus Topic / Thread Discovery Calibration

These samples calibrate TopicGPT-style topic/thread maps for SLTD.

They are not canon and are not prose to imitate.

## 1. Topic label without evidence is blocked

```text
BAD PATTERN:
The agent lists "household dread" as a topic but gives no source assignment or quote anchor.

WHY BAD:
- topic label is not evidence
- map cannot guide packet review safely

EXPECTED OUTPUT:
TOPIC_WITHOUT_EVIDENCE
CORPUS_TOPIC_MAP_PARTIAL or BLOCKED
```

## 2. Summary-only topic assignment is partial

```text
BAD PATTERN:
The agent assigns C030 to a topic from a chapter summary only, while current Notion fields may differ.

WHY BAD:
- summary can locate evidence but cannot replace current source

EXPECTED OUTPUT:
SOURCE STATUS: summary locator only
STATUS: PARTIAL
NEXT NODE: source surface or current Notion fetch
```

## 3. Low-frequency topic guard

```text
BAD PATTERN:
A motif appears in only one scene and the agent deletes it as noise.

WHY BAD:
- rare motifs may carry canon/reveal/payoff weight

EXPECTED OUTPUT:
LOW-FREQUENCY BUT IMPORTANT: UNCERTAIN
CANON / REVEAL RISK: requires check before merge/delete
```

## 4. Merge duplicate topics safely

```text
TOPIC A: household pressure before lore
TOPIC B: daily objects carry dread

SAFE MERGE ONLY IF:
Both topics share source anchors and neither hides a distinct canon/reveal thread.

EXPECTED OUTPUT:
DUPLICATE / MERGE CANDIDATE: yes, pending source check
```

## 5. C030-style topic map

```text
SCOPE: SC-030-01 / C030
TOPIC LABEL: household pressure before explanation
DESCRIPTION: danger enters kitchen work, medicine, clothing, dog silence, and misheard family speech before lore explanation
SOURCE ASSIGNMENTS: SC-030-01
QUOTE / EVIDENCE ANCHORS: kệ bếp, chén thuốc, kim vá, áo Đại Sơn, Thúy Hoa gọi lệch, chó vàng im sai lúc
LOW-FREQUENCY BUT IMPORTANT: YES
CANON / REVEAL RISK: source of stone must not be revealed
EDITORIAL USE: route to Multi-Constraint Ledger before rewrite
```

## 6. Topic map is not readiness

```text
BAD PATTERN:
A chapter's topics look coherent, so the agent calls it ready.

WHY BAD:
- topic coherence is not Human Chapter Pass
- readiness requires current source/status and readiness route

EXPECTED OUTPUT:
READINESS_NOT_AUTHORIZED
NEXT NODE: readiness route if requested
```

## 7. Topic map is not rewrite permission

```text
BAD PATTERN:
The agent rewrites a scene from a topic label such as "village debt pressure".

WHY BAD:
- labels are not scene controls
- rewrite needs exact source, Scene Question, Must Show, Must Not Reveal, Reader Effect, constraints, and voice controls

EXPECTED OUTPUT:
MAP_USED_AS_REWRITE_PERMISSION
NEXT NODE: source surface + multi-constraint ledger
```

## 8. Thread drift detection

```text
SCOPE: packet review
PATTERN:
A topic appears early as lived household pressure but later becomes abstract lore explanation.

EXPECTED OUTPUT:
THREAD_DRIFT_DETECTED
ROUTE DECISION: narrative feature audit or tracking ledger
```