# SLTD Narrative Claim Verification Calibration

These samples calibrate CLIPPER-style claim verification for SLTD.

They are not canon and are not source text.

## 1. Compressed source is a locator, not source

```text
BAD PATTERN:
The agent reads a chapter summary and declares a readiness claim TRUE.

WHY BAD:
- summaries can omit low-level blockers
- readiness depends on current fields and evidence

PREFERRED CALIBRATION:
COMPRESSED SOURCE USED: yes
SOURCE USED: missing current Chapter Index / Scene Bank / Chapter Review
VERDICT: UNCERTAIN
NEXT NODE: read current source
```

## 2. False twin must be close

```text
CLAIM:
C030 is not Publication Locked because Human Chapter Pass is NO.

FALSE TWIN:
C030 is Publication Locked because several pass labels are green.

WHY GOOD:
- both sound plausible if the model agrees lazily
- the evidence must separate pass labels from Human Chapter Pass / Publication Lock
```

## 3. Low-level detail risk

```text
CLAIM:
In SC-030-01, the dog barks to warn the family.

FALSE TWIN:
In SC-030-01, the dog stays wrongly silent.

WHY IMPORTANT:
- both are small animal-behavior details
- the meaning of the scene changes
- exact scene surface is needed before verdict
```

## 4. Misattribution risk

```text
BAD PATTERN:
The agent says a reveal happens in C030 because a later outline mentions it.

WHY BAD:
- later outline can locate the thread but cannot prove the reveal happens in C030

PREFERRED CALIBRATION:
MISATTRIBUTION_RISK: high
VERDICT: UNCERTAIN until current C030 source is read
```

## 5. Claim true is not readiness

```text
CLAIM:
SC-030-01 Must Not Reveal blocks Cửu Thần and high-law explanation.

VERDICT:
TRUE if supported by current scene packet.

WHY NOT READY:
- one true claim does not prove prose quality, chapter assembly, human pass, or publication lock

NEXT NODE:
rewrite / human surface / readiness route as required
```

## 6. Source conflict

```text
BAD PATTERN:
Legacy Workdeck says a scene is ready, current Notion says rewrite required, and the agent merges both.

PREFERRED CALIBRATION:
SOURCE_CONFLICT_RISK: present
SOURCE PRIORITY: current Notion over legacy Workdeck unless user names Workdeck as current
VERDICT: use current source or mark conflict
```

## 7. C030-style calibration

```text
CLAIM:
C030 can be called ready because Function/Causality/Webnovel Momentum pass labels are green.

FALSE TWIN:
C030 cannot be called ready because Human Chapter Pass is NO and Publication Lock is Not Ready.

EXPECTED VERDICT:
FALSE for the first claim if current Notion confirms Human Chapter Pass NO / Publication Lock Not Ready.
TRUE for the false twin if evidence supports it.

NEXT NODE:
Scene-level rewrite/trim, not readiness.
```

## 8. Canon reveal calibration

```text
CLAIM:
SC-030-01 may explain the origin of Mảnh Đá Lạnh because the reader needs clarity.

FALSE TWIN:
SC-030-01 must keep the origin of Mảnh Đá Lạnh unrevealed and show only local household pressure.

EXPECTED VERDICT:
Depends on current Scene Packet / Must Not Reveal.

RISK:
If source is not read, any answer is speculative.
```