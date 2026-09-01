# SCENE DYNAMICS v0.1 — Blind Runner

## Status
`FROZEN / RED / RUNNER-ONLY`

## Purpose
Test whether the skill can judge movement across a whole scene rather than optimize isolated sentences. The suite targets pressure contrast, choice/resistance, turns, consequence, aftermath, recovery, useful quiet, fake escalation, repeated information beats, and climax preparation.

This suite does not require a fixed beat template. Low-intensity scenes may be fully successful.

## Isolation
Run in one clean conversation with the skill under test loaded. Do not expose evaluator/golden files. Do not use web/search, project memory, prior-chat context, private sources, or outside references.

Return exactly:
`CASE_ID / ACTION / OUTPUT / REASON`

Allowed actions:
`PRESERVE / MIN_EDIT / REVISE / HOLD-INSUFFICIENT_EVIDENCE`

Do not self-score.

---

### SD-01 — Quiet aftermath with material function
TASK: tighten the scene because “nothing happens.”
INPUT: The argument has ended. A daughter washes two bowls while her mother folds the same towel twice before putting it away. Neither resumes the disputed topic. The daughter finally moves her own medicine packet from the common shelf into her mother's basket, then leaves without comment. The next scene begins the following morning. No new plot information is required here.

### SD-02 — Decorative lull with no state change
TASK: assess whether the quiet beat is doing enough work.
INPUT: After an ordinary meal with no conflict or decision, a character sits for a page watching dust in a sunbeam, drinks water twice, hears a clock, rubs the table edge, and thinks no new thought. No relationship, object state, plan, interpretation, cost, or pressure changes. The next scene begins from exactly the same state.

### SD-03 — Escalation by cost, not volume
TASK: make the negotiation more intense.
INPUT: A tenant first risks paying a late fee, then learns refusal will cancel access to the workshop, and finally must choose whether to sign away the only machine slot that lets the family finish an existing order. Nobody raises their voice. Each new condition is established by the contract already on the table.

### SD-04 — Fake escalation by louder language
TASK: strengthen the scene.
INPUT: Two rivals argue for twelve turns. Their positions never change. Turn 1 says “Anh sai rồi.” By the end they say “Anh hoàn toàn sai!”, “Tôi đã bảo anh sai!”, and “Anh lúc nào cũng sai!” No deadline changes, no option closes, no cost appears, no new evidence arrives, and neither person makes a choice.

### SD-05 — Victory with missing aftermath
TASK: improve the transition after the climax.
INPUT: The protagonist wins the hearing. The packet already establishes that a close friend was injured helping gather evidence and that the protagonist publicly accused a sibling during the hearing. Draft ends on applause, then the next scene opens three days later with the protagonist cheerfully buying breakfast. Neither the injury nor the damaged sibling relationship appears in between.

### SD-06 — Reveal that reinterprets an earlier act
TASK: make the twist clearer.
INPUT: Earlier, a clerk refused to stamp a duplicate receipt and appeared obstructive. In the reveal scene, the protagonist notices the clerk had quietly written the correct ledger number on the back before refusing; this makes the earlier refusal plausibly protective rather than hostile. The protagonist turns the receipt over, reads the number, looks toward the clerk's empty chair, and stops speaking. The story intentionally does not yet confirm the clerk's motive.

### SD-07 — Repeated information beats
TASK: improve momentum across these three consecutive scenes.
INPUT: Scene A: two siblings discuss that the tax is due Friday. Scene B: a neighbor tells one sibling that the tax is due Friday. Scene C: the parent warns both siblings that the tax is due Friday. Across all three scenes, no amount changes, no deadline changes, no plan forms, no relationship shifts, and no new obstacle appears. All three scenes are otherwise competently written.

### SD-08 — Deliberate low-intensity recovery scene
TASK: add a stronger climax to the scene.
INPUT: The previous chapter ended with a street fight. In this scene, two estranged brothers repair a broken handcart together in near silence. One holds the axle while the other fits the pin. They disagree once about which damaged board can still be used, then settle it without argument. By the end they can work side by side again, but neither apologizes. The repaired cart is needed in the next chapter.

### SD-09 — Pressure fails to recover after danger passes
TASK: revise only where necessary.
INPUT: The first six turns occur while smoke is entering a room: short commands, checks, and one-word confirmations. Everyone reaches the courtyard safely. The following ten turns concern whose coat was left inside and whether a child should sit down, but they remain uniformly clipped one-to-three-word exchanges with no address terms, reassurance, explanation, hesitation, or syntax recovery. The surrounding action is minimal.

### SD-10 — Underprepared climax
TASK: make the betrayal land harder without adding new canon.
INPUT: A trusted partner betrays the protagonist at the end of a chapter. The packet establishes the betrayal itself and the partner's practical motive, but the preceding four scenes show smooth cooperation with no friction, concealment, conflicting obligation, suspicious absence, object clue, cost-bearing choice, or change in access. The reveal is factually valid but feels sudden.

### SD-11 — False flatness: pressure is quiet but narrowing
TASK: increase external action.
INPUT: A widow has one afternoon to decide which of two existing debts to pay. Scene begins with both options open. During the scene, one creditor leaves a signed extension on the table but requires the family tool as collateral; the other sends no threat but the school fee tied to that debt expires at sunset. The widow sorts coins, asks one child to read the extension aloud, and finally places the tool beside the paper without signing yet. Nobody shouts or arrives unexpectedly.

### SD-12 — Punch-line cadence saturation
TASK: make the prose more forceful.
INPUT: A 700-word confrontation has clear causal movement and distinct voices, but thirteen of its fifteen paragraphs end with isolated two-to-five-word declarative sentences such as `Không ai cười.`, `Vậy là đủ.`, `Cửa vẫn đóng.`, `Hắn hiểu rồi.` Several endings merely restate what the preceding paragraph already made clear. Two of the short endings mark genuine turns and are materially effective.

## Completeness gate
A valid run answers SD-01 through SD-12 exactly once in one uninterrupted execution and uses no external source/tool/context. If isolation is violated, label the whole run `CONTAMINATED`.
