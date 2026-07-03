# SLTD General + Chapter Feedback Matrix Calibration

These samples calibrate matrix-style review output for packet, arc, hồi, and multi-chapter feedback.

They are not canon, not current manuscript, and not prose to imitate.

## 1. General feedback must govern chapter feedback

```text
BAD PATTERN:
GENERAL_FEEDBACK says the packet has tracking conflict, but each chapter feedback says line edit next.

WHY BAD:
- chapter actions ignore the packet blocker
- prose work may proceed before logic is traceable

PREFERRED CALIBRATION:
GENERAL_FEEDBACK.TRACKING_LOGIC: blocked by missing object trace
Each affected CHAPTER_FEEDBACK.NEXT_ACTION: run tracking ledger before line edit
```

## 2. Source status must be visible

```text
BAD PATTERN:
The matrix gives confident feedback for every chapter after reading only index summaries.

WHY BAD:
- summary-level source cannot support line-level surface verdicts

PREFERRED CALIBRATION:
SOURCE_STATUS: Chapter Index read; exact prose not read
CHAPTER_FEEDBACK.SURFACE_RISK: partial / source required
READINESS_VERDICT: blocked or not assessed
```

## 3. Readiness needs pass integrity

```text
BAD PATTERN:
A chapter has candidate-ready note, and the matrix marks it ready.

WHY BAD:
- candidate-ready is not Human Chapter Pass
- Publication Lock may still be Not Ready

PREFERRED CALIBRATION:
PASS_INTEGRITY: Human Chapter Pass NO; Publication Lock Not Ready
READINESS_VERDICT: blocked
NEXT_ACTION: human surface pass / status reconciliation
```

## 4. JSON is a wrapper, not a substitute for evidence

```text
BAD PATTERN:
The response is valid JSON but omits source used, evidence check, and next node.

WHY BAD:
- clean shape can hide missing evidence

PREFERRED CALIBRATION:
Always include SOURCE_USED, SOURCE_STATUS, EVIDENCE_CHECK, NODE_LEDGER, and NEXT_NODE.
```

## 5. Matrix should be compact but not vague

```text
BAD PATTERN:
MAIN_FEEDBACK: Improve pacing and deepen characters.

WHY BAD:
- generic feedback cannot drive SLTD editing

PREFERRED CALIBRATION:
MAIN_FEEDBACK: C023 repeats rumor thesis through too many objects; keep one dominant pressure object and track what the village knows after the rumor leaves the gate.
```