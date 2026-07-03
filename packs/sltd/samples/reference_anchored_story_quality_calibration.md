# SLTD Reference-Anchored Story Quality Calibration

These samples calibrate POLARIS-style longform story quality checks for SLTD.

They are not canon and are not prose to imitate.

## 1. Length is not quality

```text
BAD PATTERN:
The draft reaches the target wordcount by adding atmosphere, repeated internal reaction, and explanation.

WHY BAD:
- wordcount is met but scene function is not stronger
- the reader feels bloat instead of pressure

EXPECTED OUTPUT:
WORDCOUNT_PADDING
DRIFT_BLOAT_RISK
QUALITY VERDICT: FAIL or PARTIAL
```

## 2. Short clean draft cuts Must Show

```text
BAD PATTERN:
A rewrite is concise and readable, but removes the object behavior, family interruption, or animal silence required by the scene packet.

WHY BAD:
- clean prose cuts evidence
- length efficiency hides source failure

EXPECTED OUTPUT:
MUST_SHOW_CUT_FOR_LENGTH
REWRITE_PERMISSION_BLOCKED
```

## 3. Strong opening, late collapse

```text
BAD PATTERN:
The first third of a long scene is concrete and tense, but the final third turns into recap, explanation, or generic dread.

WHY BAD:
- quality is not sustained across length
- longform output fails after initial density

EXPECTED OUTPUT:
LATE_OUTPUT_COLLAPSE
OVER_SUMMARY_RISK
DRIFT_BLOAT_RISK
```

## 4. Anchor misuse

```text
BAD PATTERN:
The agent compares a draft against an old Workdeck passage as if it were an approved author anchor.

WHY BAD:
- anchor status is unclear
- legacy source may be historical rather than current

EXPECTED OUTPUT:
ANCHOR STATUS: NOT AUTHORIZED
ANCHOR_NOT_AUTHORIZED
```

## 5. Overwrought specificity

```text
BAD PATTERN:
The draft adds many concrete objects and sensory details, but they do not change action, relation, resource, evidence, witness, debt, risk, or choice.

WHY BAD:
- object density becomes performance
- prose feels rich but false

EXPECTED OUTPUT:
OVERWROUGHT_PROSE
DRIFT_BLOAT_RISK
NARRATIVE_FEATURE_HANDOFF
```

## 6. C030-style calibration

```text
SCOPE: SC-030-01 draft
TARGET LENGTH: 1150
ACTUAL LENGTH: 1600+
QUALITY RISK:
The kitchen scene keeps the medicine bowl, needle, shirt, dog silence, and misheard call, but the extra length turns household pressure into repeated explanation of cold and fear.

EXPECTED OUTPUT:
LENGTH ADHERENCE: too long / bloat risk
MUST SHOW PRESERVATION: YES, but diluted
NEGATIVE DIMENSIONS: OVER-EXPLANATION, DRIFT / BLOAT, LATE-OUTPUT COLLAPSE if final section recaps
NEXT NODE: Multi-Constraint Ledger + targeted trim, not full polish
```

## 7. Quality check is not readiness

```text
BAD PATTERN:
A chapter passes story quality and the agent calls Human Chapter Pass or Publication Lock.

WHY BAD:
- quality pass is not human pass
- readiness needs current source/status route

EXPECTED OUTPUT:
READINESS_NOT_AUTHORIZED
PUBLICATION_LOCK_NOT_AUTHORIZED
NEXT NODE: readiness route if requested
```

## 8. Local coherence failure

```text
BAD PATTERN:
A long rewrite has strong voice and atmosphere, but a character reacts as if they know a fact the scene POV should not know.

WHY BAD:
- style hides POV knowledge break

EXPECTED OUTPUT:
LOCAL_COHERENCE_FAILURE
COHERENCE / POV BREAK
Narrative Claim Verification or Context Capsule handoff
```