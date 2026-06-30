# SLTD Evidence Discipline

Use this rule when an answer makes a claim about source, canon, lock status, readiness, chapter state, or packet state.

## Core rule

Do not make a current-state claim without current source evidence.

If the source was not opened or provided in the task, say so.

## Evidence block

Use this compact format for important claims:

```text
CLAIM:
SOURCE:
NODE:
CONFIDENCE:
UNREAD RISK:
```

## Claims that require evidence

Evidence is required for:

- current manuscript status;
- Chapter Index status;
- Human Chapter Pass;
- Publication Lock;
- Scene Bank readiness;
- packet lock;
- canon conflict;
- source conflict;
- whether a pass label is still valid;
- whether a chapter blocks a packet.

## Not enough evidence

These are not enough by themselves:

- chat memory;
- old Google Doc or Workdeck;
- old audit log;
- a prior assistant claim;
- a green label without current lock fields;
- a summary without page source.

## Stop rule

If evidence is missing for a current-state claim, return:

```text
EVIDENCE_MISSING:
NEEDED SOURCE:
SAFE CLAIM:
```

The safe claim should be narrower and avoid lock or readiness verdicts.
