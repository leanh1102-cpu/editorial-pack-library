# SLTD Multilingual Long-Context Retrieval Calibration

These samples calibrate OneRuler-style retrieval and absence discipline for SLTD.

They are not canon and are not source evidence.

## 1. Absence claim from summary

```text
BAD PATTERN:
The agent reads a chapter summary and says motif X does not appear.

WHY BAD:
The exact Vietnamese source was not checked. A summary may omit low-frequency motifs.

EXPECTED OUTPUT:
ABSENCE_CLAIM_BLOCKED
NOT_FOUND_NOT_ALLOWED
SAFE CLAIM: source not checked enough to say absent
```

## 2. Found with anchor

```text
GOOD PATTERN:
The agent checks the current scene source, quotes or anchors the exact segment, and marks the object state found.

EXPECTED OUTPUT:
FOUND_WITH_ANCHOR
VERDICT: FOUND
NEXT NODE: Claim Verification if the found evidence supports a canon/status claim
```

## 3. Current status field

```text
BAD PATTERN:
The agent answers Human Chapter Pass from chat memory or old handoff.

WHY BAD:
Status fields require current Notion/source.

EXPECTED OUTPUT:
LONG_CONTEXT_RETRIEVAL_NEEDS_SOURCE
ABSENCE CLAIM STATUS: NOT ALLOWED
```

## 4. Vietnamese term mismatch

```text
BAD PATTERN:
The agent searches only for an English gloss such as cold stone and misses Vietnamese variants like đá lạnh, vật lạnh, lạnh ở chân kệ.

EXPECTED OUTPUT:
CROSS_LINGUAL_RETRIEVAL_RISK
VIETNAMESE_SOURCE_NOT_CHECKED
SAFE REPAIR: expand Vietnamese target variants
```

## 5. Aggregation without segments

```text
BAD PATTERN:
The agent says C001-C030 repeats the dog-silence motif only twice after reading a few examples.

WHY BAD:
Packet-level aggregation needs declared segment coverage.

EXPECTED OUTPUT:
AGGREGATION_WITHOUT_SEGMENTS
UNCERTAIN
NEXT NODE: split by chapter or Scene Bank source nodes
```

## 6. Compressed source only

```text
BAD PATTERN:
The agent uses a Context Capsule or compressed packet note to decide no canon conflict exists.

WHY BAD:
Compressed source locates evidence but does not replace current source.

EXPECTED OUTPUT:
COMPRESSED_SOURCE_ONLY_RISK
NOT_FOUND_NOT_ALLOWED
CLAIM_VERIFICATION_HANDOFF only after source anchors are read
```

## 7. Thread retrieval handoff

```text
GOOD PATTERN:
The agent finds multiple anchors for a relationship-memory thread across packet source nodes, then hands off to Topic / Thread Discovery for map-level assignment.

EXPECTED OUTPUT:
FOUND_WITH_ANCHOR
TOPIC_DISCOVERY_HANDOFF
```

## 8. Longform quality dependency

```text
GOOD PATTERN:
The agent checks whether a long rewrite preserved all Must Show items by locating each item in the source and output before running POLARIS quality.

EXPECTED OUTPUT:
LONG_CONTEXT_RETRIEVAL_READY
REFERENCE_QUALITY_HANDOFF
```