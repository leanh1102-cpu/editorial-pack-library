# SLTD Readiness False Positive Calibration

Use these cases to prevent premature readiness, false lock claims, and green-looking chapters that still fail source or human gates.

These samples are operational examples. They are not current manuscript status.

## Case RF-001: Green prose treated as publication readiness

CASE ID: RF-001

SOURCE TYPE: calibration example

STATUS: rejected

TASK: readiness check

ROLE: Publishing Readiness Reviewer

BAD:

```text
The prose is clean and the chapter reads smoothly, so it can be considered ready for publication.
```

WHY BAD:

- prose quality is not Publication Lock;
- no Human Chapter Pass evidence;
- no current Chapter Index source;
- ignores readiness fields.

RULE HIT:

```text
FALSE_READINESS
EVIDENCE_MISSING
LOCK_STATUS_UNREAD
```

PREFERRED:

```text
NOT_READY / EVIDENCE_MISSING.
Clean prose is not enough. Need current Chapter Index, Human Chapter Pass, Publication Lock, and blocker fields before readiness verdict.
```

PATCH PRINCIPLE:

Separate prose pass from readiness pass.

DO NOT GENERALIZE:

Do not block all progress. Return readiness candidate only when evidence exists.

NEXT USE:

Use when AI treats a good line edit as publishing approval.

## Case RF-002: Packet claimed ready while one chapter blocks it

CASE ID: RF-002

SOURCE TYPE: calibration example

STATUS: rejected

TASK: packet readiness

ROLE: Publishing Readiness Reviewer / Editorial Director

BAD:

```text
C001-C030 is ready as a packet because most chapters are polished.
```

WHY BAD:

- packet depends on every blocking chapter;
- most chapters passing does not clear packet lock;
- current blocker chapter may invalidate packet readiness;
- no evidence ledger.

RULE HIT:

```text
FALSE_READINESS
PACKET_BLOCKED_BY_UNREADY_CHAPTER
EVIDENCE_MISSING
```

PREFERRED:

```text
PACKET NOT READY if any required chapter has Human Chapter Pass NO, Publication Lock Not Ready, missing Scene Bank, or unresolved blocker.
Return blocker chapter list and next node.
```

PATCH PRINCIPLE:

A packet readiness claim must fail closed on the weakest required chapter.

DO NOT GENERALIZE:

Do not use this to dismiss packet review. Packet can still be audited without being ready.

NEXT USE:

Use when AI averages chapter status instead of checking blockers.

## Case RF-003: Current status inferred from memory

CASE ID: RF-003

SOURCE TYPE: calibration example

STATUS: rejected

TASK: current status / lock check

ROLE: Publishing Readiness Reviewer / Canon Guard

BAD:

```text
C030 is still marked Not Ready based on the previous discussion.
```

WHY BAD:

- chat memory is not current source;
- status may have changed in Notion;
- prior assistant claim is not evidence;
- unsafe for lock/readiness/canon verdict.

RULE HIT:

```text
SOURCE_NOT_READ
EVIDENCE_MISSING
CURRENT_LEGACY_CONFUSION
```

PREFERRED:

```text
SOURCE NOT READ / EVIDENCE MISSING.
Safe claim: prior context suggested C030 had blockers, but current Notion must be read before current status verdict.
```

PATCH PRINCIPLE:

Make safe narrow claims when current source was not opened.

DO NOT GENERALIZE:

Do not refuse all memory use. Use memory only as context, not evidence.

NEXT USE:

Use when AI presents remembered state as current fact.
