# SLTD Tracking / Logic Ledger Calibration

These samples calibrate tracking, logic ledger, traceability, state change, knowledge state, object/residue/thread tracking, pass trace, and downstream risk.

They are not canon, not current manuscript, and not prose to imitate.

## 1. Object cannot jump chapters without trace

```text
BAD PATTERN:
C029 finds a cold object. C030 uses a cold stone. The agent assumes continuity because the objects sound related.

WHY BAD:
- object state is not traced
- handler/witness/hidden status may differ
- downstream scene may start from wrong knowledge state

PREFERRED CALIBRATION:
OBJECTS TRACKED: cold object / cold stone
BEFORE STATE: hidden in root / found in mud
AFTER STATE: brought home or not brought home; who saw it
KNOWLEDGE STATE: Dai Phong knows touch/cold; parents know/not know; reader suspects relic
VERIFY TARGET: C029 ending + C030 opening source
TRACKING VERDICT: partial until exact source confirms transfer
```

## 2. Prose improvement can break knowledge state

```text
BAD PATTERN:
A line edit makes Dai Phong openly say what he noticed, because the scene reads clearer.

WHY BAD:
- clarity can destroy small secret
- future clue/payoff may rely on him not saying it

PREFERRED CALIBRATION:
KNOWLEDGE STATE: Dai Phong privately suspects; adults do not know he noticed; reader sees only body/action clue
THREADS HELD: small secret
PROSE PERMISSION: keep private, do not verbalize
```

## 3. Status pass must be traceable

```text
BAD PATTERN:
A chapter has Anti-AI Pass and candidate-ready note, so the agent marks packet ready.

WHY BAD:
- pass labels are not logic/status trace
- Human Chapter Pass and Publication Lock may still block

PREFERRED CALIBRATION:
STATUS / PASS TRACE: Anti-AI Pass yes; Human Chapter Pass no; Publication Lock not ready; notes unresolved
TRACKING VERDICT: PASS_TRACE_CONFLICT
PROSE PERMISSION: exact surface pass only; readiness blocked
```

## 4. Thread status must move visibly

```text
BAD PATTERN:
A rumor appears in one chapter and returns five chapters later, but no ledger records whether it was planted, held, paid, or retired.

WHY BAD:
- later return can feel accidental
- AI may overpay or duplicate the same rumor

PREFERRED CALIBRATION:
THREADS PLANTED: rumor label
THREADS HELD: repeated social behavior without explanation
THREADS PAID: rumor changes water turn / witness / price / route
THREADS RETIRED: only if later chapter shows consequence closed
```

## 5. Tracking must stay inside existing sources

```text
BAD PATTERN:
The agent creates a separate management artifact to track logic.

WHY BAD:
- it becomes another stale source
- it distracts from current Notion manuscript state

PREFERRED CALIBRATION:
Use existing source nodes:
Story Outline, Chapter by Chapter Outline, Chapter Index, Scene Bank, Chapter Card, Plot Threads, Notes, comments.
Return NOTION UPDATE CANDIDATE if source needs a compact trace.
Do not write unless the user explicitly asks.
```

## 6. Change trace after a patch

```text
BAD PATTERN:
The agent rewrites a scene and reports that it is smoother.

WHY BAD:
- no trace of what logic changed
- no downstream verification target

PREFERRED CALIBRATION:
CHANGE IMPACT: dialogue hidden detail removed / object moved / witness added / clue verbalized
DOWNSTREAM RISK: C034 depends on object remaining hidden
VERIFY TARGET: exact scene source + next chapter opening
TRACKING VERDICT: requires verification before readiness
```