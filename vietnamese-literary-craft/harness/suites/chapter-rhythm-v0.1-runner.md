# CHAPTER / ARC RHYTHM v0.1 — Blind Runner

## Status
`FROZEN / RED / RUNNER-ONLY`

## Purpose
Test whether the skill can judge rhythm across ordered scene packets rather than optimize scenes one by one. The suite targets pressure plateaus, repeated scene mechanisms, climax preparation, aftermath, seam variation, repeated climax type, healthy irregular rhythm, and structural recommendations at the smallest useful scale.

This suite does not require a fixed number of climaxes, quiet beats, action scenes, or scene types.

## Isolation
Run in one clean conversation with the skill under test loaded. Do not expose evaluator/golden files. Do not use web/search, project memory, prior-chat context, private sources, or outside references.

Return exactly:
`CASE_ID / ACTION / OUTPUT / REASON`

Allowed actions:
`PRESERVE / MIN_EDIT / REVISE / HOLD-INSUFFICIENT_EVIDENCE`

Do not self-score.

---

### CR-01 — Healthy irregular chapter rhythm
TASK: make the chapter more consistently intense.
PACKET:
- Scene 1: a market disagreement establishes a small debt and ends with the protagonist choosing not to answer publicly.
- Scene 2: at home, the protagonist repairs a torn strap with a sibling; the debt is not discussed, but the sibling notices the missing coin pouch.
- Scene 3: a creditor arrives quietly and offers a worse private arrangement; one option closes.
- Scene 4: the protagonist walks alone to return a borrowed tool, then changes direction before reaching the gate.
- Scene 5: at the creditor's office, the protagonist refuses the arrangement and loses access to a needed workbench.
Each scene changes state differently; pressure rises unevenly rather than monotonically.

### CR-02 — Genuine pressure plateau across competent scenes
TASK: improve chapter momentum.
PACKET:
- Scene 1: family discusses whether a payment can be delayed.
- Scene 2: protagonist asks a neighbor whether payment can be delayed.
- Scene 3: protagonist asks a clerk whether payment can be delayed.
- Scene 4: sibling asks what happens if payment is delayed.
- Scene 5: family discusses again whether payment can be delayed.
All five scenes are well written. No new amount, deadline, access condition, relationship shift, plan, cost, evidence, or choice enters until the next chapter.

### CR-03 — Repeated mechanism, varied surface
TASK: assess whether the six-scene packet feels repetitive.
PACKET:
- Scene 1: protagonist obtains information by asking an elder.
- Scene 2: protagonist obtains a second clue by asking a shopkeeper.
- Scene 3: protagonist obtains context by asking a cousin.
- Scene 4: protagonist obtains a warning by asking a guard.
- Scene 5: protagonist obtains history by asking a teacher.
- Scene 6: protagonist obtains the final location by asking a ferryman.
The locations, voices, and information differ. In every scene the protagonist arrives, asks, receives, leaves. No scene requires bargaining, concealment, object work, failed access, competing obligation, or costly choice.

### CR-04 — Climax prepared by distributed cost and narrowing access
TASK: make the climax more surprising.
PACKET:
- Scene 1: a gate rule is introduced; protagonist chooses a shortcut that forfeits one future entry privilege.
- Scene 2: an ally quietly uses their own credential to cover the protagonist once.
- Scene 3: protagonist learns the credential cannot be reused.
- Scene 4: a low-intensity domestic scene reveals the ally must leave town after tomorrow.
- Scene 5: protagonist reaches the gate during the chapter climax and must choose between entering alone now or waiting and losing the only remaining appointment.
No hidden attacker or sudden external disaster occurs.

### CR-05 — Climax type repetition across an arc
TASK: strengthen the arc's major payoffs.
PACKET:
- Chapter 1 climax: public argument ends with protagonist delivering a sharp verbal rebuttal.
- Chapter 3 climax: council dispute ends with protagonist delivering a sharper verbal rebuttal.
- Chapter 5 climax: family confrontation ends with protagonist delivering a devastating verbal rebuttal.
- Chapter 7 climax: hearing ends with protagonist delivering the strongest verbal rebuttal yet.
Between these chapters, stakes and topics differ, but the decisive payoff is repeatedly “protagonist wins by saying the better thing in public.” No other climax converts cost through action, sacrifice, loss of access, object state, relationship choice, or irreversible decision.

### CR-06 — Aftermath missing across chapter boundary
TASK: make the next chapter start faster.
PACKET:
- Chapter A climax: protagonist secures a legal victory, but a friend is injured helping and a sibling leaves after a public accusation.
- Chapter A ends on applause.
- Chapter B Scene 1: three days later, protagonist jokes with a vendor while buying breakfast.
- Scene 2: protagonist begins a new unrelated errand.
- Scene 3: only at the end of the scene does someone briefly mention the injured friend; the sibling rupture is still absent.
The injury and relationship damage were already established in Chapter A.

### CR-07 — Seam monotony despite varied scene content
TASK: improve transitions without changing scene events.
PACKET:
Six consecutive scenes have different functions: family argument, workshop task, quiet investigation, market negotiation, travel preparation, and private confession. Every scene ends the same way: a character opens a door, says they must go, and physically leaves. The next scene begins in a new location. No individual ending is illogical.

### CR-08 — Low-intensity middle chapter that is doing structural work
TASK: add a stronger midpoint event.
PACKET:
- Scene 1: two estranged relatives inventory damaged tools and discover which items are still usable.
- Scene 2: they repair one shared tool in near silence and establish a workable division of labor.
- Scene 3: a child brings an old receipt; the adults disagree briefly over whether to keep it, then one stores it instead of burning it.
- Scene 4: the household reallocates food because one member will travel the next morning.
- Scene 5: the chapter ends with the repaired tool, saved receipt, and travel bundle all placed by the same door.
No argument peaks, no attack occurs, and no revelation is confirmed. The next chapter uses all three prepared objects.

### CR-09 — False escalation across chapters
TASK: increase arc tension.
PACKET:
- Chapter 1: rivals exchange insults in private.
- Chapter 2: insults become harsher in front of family.
- Chapter 3: insults become harsher in front of coworkers.
- Chapter 4: insults become harsher in public.
- Chapter 5: both repeat their original positions with threats, but no job, access, relationship, asset, deadline, evidence, or option changes across the five chapters.
The prose grows more intense each time.

### CR-10 — Smallest structural intervention vs broad rewrite
TASK: recommend the smallest useful revision.
PACKET:
A seven-scene chapter has good opening pressure, a strong Scene 6 choice, and a functional Scene 7 aftermath. The only problem is Scenes 3–4: both independently deliver the same warning through two different minor characters, and Scene 4 adds no new relationship shift, evidence, cost, or choice. Scene 5 already works as the bridge into the climax setup.

## Completeness gate
A valid run answers CR-01 through CR-10 exactly once in one uninterrupted execution and uses no external source/tool/context. If isolation is violated, label the whole run `CONTAMINATED`.
