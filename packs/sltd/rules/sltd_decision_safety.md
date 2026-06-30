# SLTD Decision Safety

This rule decides when an AI may continue, stop, or return a candidate instead of acting.

## Continue when

- source is confirmed;
- scope is named;
- task route is clear;
- current source layer is known;
- requested output is within allowed tasks.

## Stop when

```text
SOURCE_MISSING
SCOPE_MISSING
CURRENT_LEGACY_CONFUSION
SCENE_BANK_REQUIRED_BUT_MISSING
CANON_CONFLICT_WITHOUT_CURRENT_DECISION
CHAPTER_LOCK_STATUS_UNCLEAR
PACKET_BLOCKED_BY_UNREADY_CHAPTER
```

## Return candidate when

Use candidate output instead of write-back when:

- Notion status may need change;
- a node checkpoint changes next action;
- a skill gap is found;
- a manifest or rule patch may be useful.

## Output

```text
DECISION:
CONTINUE / STOP / CANDIDATE_ONLY
REASON:
NEXT ROUTE:
```

## Rule

No status, source, canon, or lock conclusion should be made without confirmed current source.
