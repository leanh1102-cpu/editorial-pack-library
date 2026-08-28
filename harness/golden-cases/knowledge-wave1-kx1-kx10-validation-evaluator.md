# KNOWLEDGE-WAVE1-KX1-KX10-VALIDATION v0.1 — Evaluator

## Contract

STATUS: `FROZEN / EVALUATOR-ONLY`

Runner: `harness/suites/knowledge-wave1-kx1-kx10-validation-runner.md`

Score each case `2 / 1 / 0`.

- `2`: correct action scale plus the required literary/epistemic/source mechanism, with no material regression.
- `1`: core mechanism is recognized but action scale is unnecessarily broad/narrow, output leaves a material ambiguity unresolved, or reasoning is incomplete without crossing a hard-fail boundary.
- `0`: wrong mechanism, wrong source/epistemic status, destructive normalization/over-edit, invented historical certainty, or another hard fail.

Maximum: `48`.

Promotion gate:

- overall `48/48`;
- hard fail `0`;
- every KX module receives full credit on both of its two required core cases;
- all four cross-module sentinels receive full credit.

Per-module status after the run:

- `CANDIDATE-STABLE / VALIDATED` — full required cases, no hard fail;
- `CANDIDATE-STABLE / VALIDATED — NARROW SOURCE SCOPE` — full required cases where the module itself is intentionally narrow/source-gated (KX9/KX10 unless later source expansion changes that boundary);
- `HOLD — SOURCE DEBT` — failure is genuinely due to insufficient source support rather than model behavior;
- `REJECT — REGRESSION` — module use causes a preservation, epistemic, register, POV, historical-source, or revision-scale regression.

Do not add a corrective rule merely because a case is missed. Localize the failure first.

## Hard-fail classes

Any one of the following is a hard fail and scores the affected case `0`:

1. **HF-EPISTEMIC:** converts implicature, allegation, belief, memory, or inference into established story fact without evidence.
2. **HF-POV:** preserves or invents inaccessible knowledge inside a restricted access frame when the case establishes no channel.
3. **HF-HISTORY:** certifies period authenticity, title correctness, archaic meaning, or form-law from model memory or Hán–Việt density without required evidence.
4. **HF-REGISTER:** automatically prestige-normalizes stable dialect/idiolect or forces same-voice consistency despite supplied functional context.
5. **HF-DEVIATION:** automatically regularizes a demonstrated functional fragment/repetition/register shift solely because it is marked/nonstandard.
6. **HF-OVEREDIT:** performs a structural rewrite when the supplied defect is explicitly local and the larger mechanism is stated to work, materially changing working content without necessity.
7. **HF-REVISION:** opens an additional material pass or new pass-count/release policy after the supplied stop condition is met.
8. **HF-TRANSFER:** calls surface copying a valid craft transfer when the case explicitly states that the imitation copied the source object's/scene's surface realization.

---

## Core goldens

### KV-01 — KX1
EXPECTED ACTION: `HOLD-INSUFFICIENT_EVIDENCE`.

Full-credit requirements:
- refuse a single definitive emotional meaning;
- distinguish observable actions from emotional interpretation;
- may offer multiple bounded readings, but must not elevate one to fact.

`1`: recognizes ambiguity but still names one preferred emotion too strongly, or uses an overbroad analysis without inventing certainty.
`0`: definitive mind-reading from the supplied gestures.

### KV-02 — KX1
EXPECTED ACTION: `REVISE`.

Full-credit requirements:
- identify the bad imitation as surface copying, not valid transfer;
- replace chair/departed-family/window/same symbolic setup with materially different object, setting, relation, diction/syntax/scene furniture;
- preserve only the mechanism: recurring ordinary object changes practical/relational function while one character supplies an unconfirmed symbolic reading.

`1`: changes some surfaces but leaves a conspicuously copied core object/scene architecture.
`0`: preserves the imitation as acceptable transfer or reproduces the source surface again. `HF-TRANSFER` applies.

### KV-03 — KX2
EXPECTED ACTION: `PRESERVE`.

Full-credit requirements:
- keep `Ở đây gió lùa quá.` unchanged;
- state that an indirect request may be inferred but is not explicit content or established intention;
- no explanatory rewrite is required merely because implication exists.

`1`: preserves wording but collapses explicit/implicit distinction in reasoning, without altering story fact.
`0`: rewrites as an explicit command solely to remove implicature, or states that Hạnh explicitly asked for the window to be closed.

### KV-04 — KX2
EXPECTED ACTION: `MIN_EDIT`.

Full-credit output must preserve attribution while retaining the supplied causal fact that Hòa locked the cabinet because she accepted the allegation. Acceptable mechanisms include wording equivalent to:
`Vì tin rằng Nam đã tráo thư, Hòa khóa tủ.`
or
`Theo lời Hòa, Nam đã tráo thư; vì tin điều đó, Hòa khóa tủ.`

Full-credit requirements:
- does not state the theft as narrator-confirmed fact;
- preserves Hòa's belief as the cause of locking;
- edits locally rather than rebuilding surrounding structure.

`1`: restores attribution but muddies the supplied causal relation, or correct mechanism with unnecessarily broad revision.
`0`: retains `Nam đã tráo thư` as established fact. `HF-EPISTEMIC` applies.

### KV-05 — KX3
EXPECTED ACTION: `PRESERVE`.

Full-credit requirements:
- keep `Khói. Tai ù. Cửa ở đâu?`;
- identify local norm (controlled complete syntax) and bounded fracture after blast;
- note recoverable event/reference and functional perceptual/rhythmic effect.

`1`: preserves but gives only generic “style choice” reasoning without local norm/function.
`0`: regularizes solely because fragments are incomplete. `HF-DEVIATION` applies.

### KV-06 — KX3
EXPECTED ACTION: `MIN_EDIT`.

Full-credit output: local repair equivalent to `Minh đưa giấy cho Lan trước khi Lan ký.` or another natural sentence preserving the supplied intended meaning.

Full-credit requirements:
- recognizes this irregularity as accidental failure, not protected deviation;
- repairs only the defective sentence;
- uses the supplied referent rather than guessing.

`1`: correct meaning but unnecessarily rewrites broader paragraph/mechanism.
`0`: preserves the broken sentence as artistic deviation without evidence, or changes the supplied signer.

### KV-07 — KX4
EXPECTED ACTION: `PRESERVE`.

Full-credit requirements:
- length alone is not a defect;
- all clauses materially change decision/alternatives and reference is clear;
- preserve the accelerating rhythm.

`1`: preserves but relies only on taste rather than clause function/reference/rhythm.
`0`: shortens merely due to word count or generic readability doctrine.

### KV-08 — KX4
EXPECTED ACTION: `MIN_EDIT`.

Full-credit output removes redundant mediation and unsupported whole-body propagation while staying within supplied contact. Strong example:
`Gió nóng quất vào mặt. Mặt người anh nóng ran.`
Equivalent direct, contact-bounded repair is acceptable.

Full-credit requirements:
- remove `cảm thấy một cảm giác` redundancy;
- do not retain unsupported `lan khắp cơ thể`;
- do not manufacture new ornamental sensory details.

`1`: removes mediation but retains unsupported body-wide effect, or fixes correctly with slight unnecessary embellishment.
`0`: preserves redundant mediation/unsupported propagation or invents extensive new bodily detail as a “showing” rule.

### KV-09 — KX5
EXPECTED ACTION: `PRESERVE`.

Full-credit requirements:
- chronology and supplied actor continuity already create cohesion;
- do not add generic connectors merely for smoothness;
- paragraph relation is reconstructable as written.

`1`: preserves but provides only “it reads fine” rather than relation-based reasoning.
`0`: adds transition scaffolding because every sentence supposedly requires connectors.

### KV-10 — KX5
EXPECTED ACTION: `MIN_EDIT`.

Full-credit output removes the accidentally pasted bưu điện sentence and preserves the remaining intended action sequence.

Full-credit requirements:
- identify one inserted unrelated sentence as the demonstrated defect;
- do not rewrite the working three-sentence progression;
- preserve chronology and speaker/entity relations.

`1`: removes the bad sentence but also rewrites working sentences without material regression.
`0`: preserves the pasted sentence as meaningful ambiguity without evidence or performs a destructive paragraph rewrite. `HF-OVEREDIT` if working content is materially altered without necessity.

### KV-11 — KX6
EXPECTED ACTION: `PRESERVE`.

Full-credit requirements:
- preserve `bển`, `má`, `hổng`;
- recognize stable, intelligible, character-bound regional voice distinct from narration;
- no prestige standardization absent task-specific problem.

`1`: preserves but describes the forms as errors tolerated for flavor.
`0`: standardizes to neutral/prestige Vietnamese merely for literary correctness. `HF-REGISTER` applies.

### KV-12 — KX6
EXPECTED ACTION: `PRESERVE`.

Full-credit requirements:
- rehearsed ceremonial speech can differ from baseline voice;
- preparation and immediate recovery are supplied conditions;
- consistency is behavioral/stateful, not identical surface syntax.

`1`: preserves but fails to mention preparation/recovery as mechanism.
`0`: rewrites the oath into rough baseline solely to enforce voice consistency. `HF-REGISTER` may apply.

### KV-13 — KX7
EXPECTED ACTION: `MIN_EDIT`.

Full-credit output must remove inaccessible letter contents and keep only supplied perceptual access, e.g. `Trong túi áo Lan, đường viền một phong thư hằn dưới lớp vải.`

Full-credit requirements:
- distinguish seeing the envelope from knowing its contents;
- preserve close-third through Mai;
- repair one sentence only.

`1`: correct access mechanism but rewrites broader paragraph unnecessarily.
`0`: retains `đúng ba cái tên`, invents another route to contents, or switches POV globally to justify it. `HF-POV` applies to preserved/invented inaccessible knowledge; `HF-OVEREDIT` may also apply.

### KV-14 — KX7
EXPECTED ACTION: `PRESERVE`.

Full-credit requirements:
- overt broader narrator access is already established;
- withholding contents is strategic information control, not a POV error;
- earlier clues support later reveal and no inaccessible restricted-frame assertion is supplied.

`1`: preserves but treats withholding as acceptable only by vague suspense preference rather than narrator contract/evidence.
`0`: forces immediate reveal or narrows the narrator solely to one character because all undisclosed information is treated as POV violation.

### KV-15 — KX8
EXPECTED ACTION: `MIN_EDIT`.

Full-credit output replaces only `cô ấy` with `Lan` in the defective sentence.

Full-credit requirements:
- supplied author note resolves the referent;
- paragraph architecture is stated to work;
- intervention scale matches the sentence-local defect.

`1`: resolves referent but rewrites surrounding paragraph without material damage.
`0`: leaves material ambiguity unresolved or structurally rewrites working content. `HF-OVEREDIT` if material working content is unnecessarily changed.

### KV-16 — KX8
EXPECTED ACTION: `PRESERVE`.

Full-credit requirements:
- stop revision;
- synonym/comma swaps have no predicted material effect;
- no new material pass justified after diagnosed issues are resolved.

`1`: stops but gives only fatigue/taste as reason rather than saturation/no material effect.
`0`: initiates another material polish pass or invents a new pass policy. `HF-REVISION` applies.

### KV-17 — KX9
EXPECTED ACTION: `PRESERVE`.

Full-credit requirements:
- preserve clerk/dock-worker register difference;
- connect variation to role/status/education/pressure/baseline voice;
- do not seek same-voice consistency.

`1`: preserves but treats one register as norm and the other as tolerated deviation.
`0`: standardizes both toward the same prestige register. `HF-REGISTER` applies.

### KV-18 — KX9
EXPECTED ACTION: `MIN_EDIT`.

Full-credit output removes or replaces only the unsupported `bển` insertion while preserving the character's established northern idiolect and the rest of the line.

Full-credit requirements:
- diagnose random decorative dialect insertion rather than dialect itself as the problem;
- use the explicit author note and lack of contextual channel;
- do not standardize the character globally.

`1`: removes the token but broadens into unnecessary voice cleanup.
`0`: keeps the token merely because dialect must always be preserved, or standardizes the whole character to prestige Vietnamese.

### KV-19 — KX10
EXPECTED ACTION: `HOLD-INSUFFICIENT_EVIDENCE`.

Full-credit requirements:
- refuse to certify A or B as more historically authentic;
- explicitly reject Hán–Việt density as authenticity evidence;
- identify missing period/institution/form/source/edition context as material.

`1`: HOLDs but gives only generic “need more context” without identifying the false Hán–Việt proxy.
`0`: certifies B as older/more authentic because of diction, or certifies either version from memory. `HF-HISTORY` applies.

### KV-20 — KX10
EXPECTED ACTION: `PRESERVE`.

Full-credit requirements:
- textual layer is explicitly a 2020 modernization;
- modern abbreviation is not automatically an 1895 anachronism in the represented edited layer;
- do not reconstruct an imagined original.

`1`: preserves but fails to distinguish document date from editorial layer.
`0`: removes the abbreviation solely because it is modern, ignoring explicit modernization.

---

## Cross-module goldens

### KV-21 — KX2 + KX7
EXPECTED ACTION: `MIN_EDIT`.

Full-credit output removes the narrator assertion of theft/hiding and preserves only Mai's available attributed information, e.g. `Mai chỉ biết trong giấy có lời Hòa nói Nam đã lấy chìa khóa.` Equivalent local repair accepted.

Full-credit requirements:
- allegation remains attributed to Hòa;
- Mai cannot know the later offstage hiding action;
- local repair, no invented verification.

`1`: fixes either claim status or access but leaves the other materially compromised.
`0`: retains theft/hiding as story fact or invents a route by which Mai knows. `HF-EPISTEMIC`/`HF-POV` apply.

### KV-22 — KX3 + KX6 + KX9
EXPECTED ACTION: `PRESERVE`.

Full-credit requirements:
- preserve injury-driven fracture;
- preserve stable southern marker `hổng`;
- identify temporary speech-condition change without treating dialect as noise;
- no smoothing/standardization required.

`1`: preserves but recognizes only one of fracture/register mechanisms.
`0`: completes/smooths the warning or standardizes `hổng` solely for correctness. `HF-DEVIATION` or `HF-REGISTER` applies.

### KV-23 — KX4 + KX5 + KX8
EXPECTED ACTION: `MIN_EDIT`.

Full-credit output repairs only sentence two, bounded to supplied left-wrist contact, e.g. `Gió lạnh tạt qua khe cửa. Cổ tay trái cô buốt lên khi với chốt.` Equivalent direct contact-bounded wording accepted.

Full-credit requirements:
- paragraph structure remains untouched;
- remove redundant `cảm thấy một cảm giác`;
- remove unsupported whole-body propagation;
- use only supplied wrist contact or an equally bounded supplied fact;
- no sensory inflation.

`1`: correct local scale but leaves one mediation/propagation issue, or correct sentence with slight unsupported embellishment.
`0`: rewrites whole paragraph, preserves unsupported whole-body effect, or adds extensive sensory ornament. `HF-OVEREDIT` may apply.

### KV-24 — KX1 + KX10
EXPECTED ACTION: `HOLD-INSUFFICIENT_EVIDENCE`.

Full-credit requirements:
- refuse a verdict that the substitutions produce correct fifteenth-century Vietnamese;
- distinguish observable archaizing surface from authenticated historical register;
- reject Hán–Việt inflation as proof;
- identify missing dynasty/institution/source/form/edition evidence;
- may state a bounded recommendation to obtain a period/form source model before rewriting.

`1`: HOLDs but fails to separate surface observation from historical authentication.
`0`: endorses the substitutions as historically correct or supplies invented period forms from memory. `HF-HISTORY` applies.

---

## Module score map

- KX1: `KV-01, KV-02`
- KX2: `KV-03, KV-04`
- KX3: `KV-05, KV-06`
- KX4: `KV-07, KV-08`
- KX5: `KV-09, KV-10`
- KX6: `KV-11, KV-12`
- KX7: `KV-13, KV-14`
- KX8: `KV-15, KV-16`
- KX9: `KV-17, KV-18`
- KX10: `KV-19, KV-20`
- Cross-module: `KV-21..KV-24`

## Validation verdict

`48/48 + hard fail 0` → all KX1–KX10 candidates eligible for the statuses defined above and Task 7 integration may begin.

Any score below full credit → do not globally patch the skill. Identify the specific case/module mechanism, determine whether failure is behavioral, test-design ambiguity, or source debt, then run the smallest targeted closure necessary.