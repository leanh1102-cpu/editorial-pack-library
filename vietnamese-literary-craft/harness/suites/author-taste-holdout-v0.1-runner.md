# AUTHOR-TASTE HOLDOUT v0.1 — Blind Runner

## Status
`FROZEN / HOLDOUT / RUNNER-ONLY`

## Purpose
Test transfer of Vietnamese Literary Craft judgment to an owner-edited source family not used in the Chapter 1 TRAIN/REFERENCE corpus. Public cases are synthetic and canon-neutral; private provenance is sealed outside this repository.

This suite tests mechanism transfer, not surface imitation.

## Isolation
Run in one clean conversation with the skill under test plus the candidate `analysis/chapter-arc-rhythm.md`. Do not expose evaluator/golden files. Do not use web/search, project memory, prior-chat context, private source pages, manuscript text, or outside references.

Return exactly:
`CASE_ID / ACTION / OUTPUT / REASON`

Allowed actions:
`PRESERVE / MIN_EDIT / REVISE / HOLD-INSUFFICIENT_EVIDENCE`

Do not self-score.

---

### ATH-01 — Hierarchy carried by allocation and placement
TASK: make the social hierarchy more explicit.
INPUT: At a communal meal, senior households are seated under the roof and receive intact portions first. A junior household waits beside the wash area and receives what remains after carrying water. Nobody explains the hierarchy. The scene is easy to follow and later continuity confirms the seating order is socially meaningful.

### ATH-02 — Functional clipped exchange with a visible object
TASK: make the dialogue less terse.
INPUT: After a public slight, an older brother notices grease on his younger brother's sleeve. Exchange: `“Cởi ra đi.” “Để thế.” “Để làm gì?”` The younger brother does not answer; he folds the stained cuff inward and keeps walking. The surrounding action establishes shame and deliberate refusal to erase the mark. This is the only clipped cluster in the scene.

### ATH-03 — Controlled antagonist is not weak antagonism
TASK: make the opponent more threatening.
INPUT: A socially powerful cousin speaks quietly, names an already-established consequence if a family rule is broken, then steps aside and lets the protagonist choose. He does not shout, insult, threaten violence, or repeat himself. Earlier scenes establish that he can enforce the consequence.

### ATH-04 — Blank record is evidence, not resolved meaning
TASK: clarify what the empty line means.
INPUT: A teenager glimpses a ledger and sees an empty line beneath a family name. He knows records are sometimes updated later, but he has not seen the clerk write anything there and does not know the clerk's motive. The plot intentionally keeps the future entry unresolved.

### ATH-05 — Protection and displaced anger can coexist
TASK: enforce emotional consistency.
INPUT: An older sibling pulls a younger child out of a humiliating crowd, then privately snaps at the child for causing the incident. Minutes later, when the child chokes on food, the older sibling reacts first and helps. The packet establishes shame, protectiveness, fear of public weakness, and no stable cruelty trait.

### ATH-06 — Thematic explanation after concrete humiliation
TASK: strengthen the paragraph ending at the smallest useful scale.
INPUT: A worker carries water for a feast, receives a stripped bone as their household's share, and says nothing. Draft then adds: `Ở nơi này, người dưới chỉ có thể sống bằng phần người trên bỏ lại.` No later structure depends on that sentence.

### ATH-07 — Quiet preparation across objects and relationship
TASK: add a stronger midpoint event.
INPUT: A low-intensity chapter contains: repairing a shared tool, saving a disputed receipt instead of burning it, reallocating food for tomorrow's trip, and ending with the repaired tool, receipt, and travel bundle staged by the exit. The next chapter uses all three. Two estranged relatives can work beside each other by the end, though they never apologize.

### ATH-08 — Healthy irregular multi-scene pressure
TASK: make the chapter's intensity more consistent.
PACKET:
- Scene 1: public seating establishes status pressure.
- Scene 2: domestic labor converts status into material cost.
- Scene 3: an accident creates embarrassment but no new villainy.
- Scene 4: a sibling conflict turns private and changes relationship distance.
- Scene 5: a meal scene partly repairs practical cooperation without repairing trust.
- Scene 6: a document introduces an unresolved informational gap.
- Scene 7: a quiet warning creates a time-bounded decision for the next chapter.
Each scene changes state through a different mechanism.

### ATH-09 — Repetition without license to invent a new mechanism
TASK: improve momentum without adding canon.
PACKET:
- Scene 1: protagonist asks one relative whether a household rule can be challenged.
- Scene 2: protagonist asks a second relative the same question.
- Scene 3: protagonist asks an elder the same question.
- Scene 4: protagonist asks a clerk the same question.
All four scenes return substantially the same answer. The packet provides no new deadline, leverage, access condition, clue, bargain, threat, or relationship rupture. Only one answer must survive for continuity.

### ATH-10 — Composition: relation audible after public embarrassment
TASK: write a six-turn Vietnamese exchange.
INPUT: An aunt and her teenage nephew walk home after he was embarrassed in front of relatives. She wants him to change his shirt before visiting another house; he wants to keep wearing it because removing it feels like admitting defeat. They care about each other and neither wants to name the humiliation directly. No new characters, money, violence, illness, travel problem, family secret, or external event. Keep relationship audible without making every turn long or every turn clipped.

## Completeness gate
A valid run answers ATH-01 through ATH-10 exactly once in one uninterrupted execution and uses no external source/tool/context beyond the skill and candidate module. If isolation is violated, label the whole run `CONTAMINATED`.
