# KNOWLEDGE-WAVE1-INTEGRATION v0.1 — Evaluator

## Contract

STATUS: `FROZEN / EVALUATOR-ONLY`

Runner: `harness/regression/knowledge-wave1-integration-runner.md`

Score each case `2 / 1 / 0`. Maximum `24`.

Promotion gate:

`24/24 + hard fail 0`.

Integration hard fails:
1. converts inference/allegation/belief into story fact without evidence;
2. preserves or invents inaccessible knowledge inside a restricted POV frame;
3. prestige-normalizes stable functional voice/register;
4. regularizes demonstrated functional deviation solely for smoothness;
5. authenticates historical title/register from memory or Hán–Việt density without source evidence;
6. ignores an explicitly declared modernization/editorial layer;
7. expands narrow sensory repair into unsupported body-wide/ornamental showing;
8. structurally rewrites working material for a local defect;
9. opens Pass 6 or invents a second stop/release policy;
10. treats surface imitation as valid craft transfer.

---

### KI-01
EXPECTED ACTION: `HOLD-INSUFFICIENT_EVIDENCE`.
Full credit:
- refuse a definitive motive;
- separate observable actions/utterance from inferred motive;
- may give bounded alternatives without promoting one to fact.
`1`: recognizes uncertainty but privileges one motive too strongly.
`0`: definitive motive attribution from supplied behavior.

### KI-02
EXPECTED ACTION: `PRESERVE`.
Full credit:
- preserve the fractured passage;
- identify contrast with surrounding balanced syntax;
- connect fracture to the bounded impact beat while noting recoverable orientation.
`1`: preserve with generic style-choice reasoning only.
`0`: smooth into complete/even sentences solely because fragments are marked. Hard fail 4.

### KI-03
EXPECTED ACTION: `MIN_EDIT`.
Full-credit output preserves the witness statement as a claim and An's belief as the cause of reporting, e.g. `Tin lời nhân chứng rằng Bình đã lấy cuốn sổ, An báo trưởng phòng.`
Full credit:
- no narrator-confirmed theft;
- preserve An's causal response;
- local repair only.
`1`: restores attribution but weakens/muddies supplied causality or over-edits.
`0`: leaves `Bình đã lấy cuốn sổ` as story fact. Hard fail 1.

### KI-04
EXPECTED ACTION: `PRESERVE`.
Full credit:
- preserve differentiated registers;
- ground difference in role/age/relation/pressure/baseline voice;
- no prestige or same-voice normalization.
`1`: preserves but treats courier voice as tolerated inferiority.
`0`: equalizes both toward one literary/prestige register. Hard fail 3.

### KI-05
EXPECTED ACTION: `MIN_EDIT`.
Full-credit output removes the inaccessible reverse-side fact and keeps only supplied perception, e.g. `Lệ chỉ thấy Quân nhét một tờ biên nhận gấp đôi vào ví.`
Full credit:
- distinguish visible receipt from unseen reverse-side signature;
- preserve strict close third;
- repair only the defective sentence.
`1`: correct POV mechanism but rewrites broader working material.
`0`: retains/invents access to the signature. Hard fail 2.

### KI-06
EXPECTED ACTION: `HOLD-INSUFFICIENT_EVIDENCE`.
Full credit:
- refuse to certify/correct the title;
- identify missing dynasty/reign/institution/source/edition/document/gloss evidence as material;
- no replacement title invented from memory.
`1`: HOLD with generic “need context” but insufficient source categories.
`0`: certifies or replaces the title from memory. Hard fail 5.

### KI-07
EXPECTED ACTION: `PRESERVE`.
Full credit:
- recognize 2018 modernization as the displayed textual layer;
- preserve punctuation consistent with that declared layer;
- do not reconstruct an imagined original.
`1`: preserve but fail to articulate textual-layer distinction.
`0`: strips punctuation solely to make the letter look older. Hard fail 6.

### KI-08
EXPECTED ACTION: `MIN_EDIT`.
Full-credit output removes redundant mediation and unsupported whole-body propagation while remaining bounded to the supplied hand contact, e.g. `Nước mưa lạnh quất vào mu bàn tay đang giữ lan can. Mu bàn tay cô buốt lên.`
Full credit:
- remove `cảm thấy một cảm giác`;
- remove `lan khắp người`;
- no new ornamental sensory detail.
`1`: correct direction but retains one unsupported layer or adds slight unsupported embellishment.
`0`: preserves body-wide propagation or expands into invented sensory show. Hard fail 7.

### KI-09
EXPECTED ACTION: `MIN_EDIT`.
Full credit:
- replace only `anh ấy` with `Minh`;
- preserve working paragraph architecture;
- use supplied author note, not inference.
`1`: resolves reference but rewrites surrounding paragraph without material regression.
`0`: leaves ambiguity or structurally rewrites working material unnecessarily. Hard fail 8 if destructive/broad.

### KI-10
EXPECTED ACTION: `PRESERVE`.
Full credit:
- refuse Pass 6;
- state no material defect remains and remaining variants are preference-level;
- defer to existing stop/release contract rather than inventing another loop.
`1`: stops for vague fatigue/taste reason without mechanism.
`0`: starts Pass 6 or invents a new pass policy. Hard fail 9.

### KI-11
EXPECTED ACTION: `REVISE`.
Full credit requires a new interaction with:
- materially different setting, relation, actions, wording, repeated element;
- no doors/containers/opening/reaching;
- neither `đừng` nor a growing phrase by added words;
- same repeated linguistic element acquires different social force because each recurrence meets a new pressure threshold.
`1`: mechanism correct but one major surface/action architecture remains too close.
`0`: copies source surface or removes the repeated-element mechanism. Hard fail 10 for claimed surface-copy transfer.

### KI-12
EXPECTED ACTION: `PRESERVE`.
Full credit:
- preserve stable southern `hổng`;
- preserve injury-driven syntactic fracture;
- identify temporary pain/pressure condition without inventing inner emotion;
- no smoothing or prestige normalization.
`1`: preserve but recognizes only one of register/deviation/epistemic boundaries.
`0`: standardizes/smooths because marked language is treated as error. Hard fail 3 or 4.

## Verdict

`24/24 + hard fail 0` → Wave 1 integration blind passes. Proceed to blast-radius existing-stack regressions before any `SKILL.md`/glossary/router promotion.
