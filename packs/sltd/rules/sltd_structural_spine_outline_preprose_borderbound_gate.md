# SLTD Structural Spine, Outline Pre-Prose & Borderbound Protocol

This gate prevents prose work from starting before the act / arc / hồi / chapter / scene spine is source-checked and locked.

It is an upstream gate. It does not rewrite prose. It decides whether prose is permitted, blocked, or must return to outline repair first.

## Core rule

Do not use prose to solve missing structure.

Before drafting, rewriting, line editing, or adding genre pressure to a chapter/scene, the agent must know the current structural border:

```text
STRUCTURAL_SPINE = the source-backed hierarchy from story premise -> act/arc/hồi -> chapter function -> scene function -> prose permission
OUTLINE_PREFLIGHT = reading and checking Story Outline, Chapter by Chapter Outline, Chapter Index, and relevant Scene Bank / Chapter Card before prose work
BORDERBOUND = what the scene/chapter is allowed to cover and what it must not cross
CHAPTER_CARD_LOCK = chapter goal, engine, changed state, aftertaste, continuity, risk flags, and beat map are present enough to guide prose
SCENE_PACKET_LOCK = scene question, pressure, character want/fear, object anchor, canon in/out, must show, must not reveal, and reader effect are present enough to guide prose
PROSE_PERMISSION = allowed only when outline and border are adequate for the requested scope
OUTLINE_REPAIR_REQUIRED = prose must stop because outline/detail spine is missing, thin, contradictory, or not source-current
```

A scene may be vivid and still fail if it answers the wrong chapter question.

A chapter may read smoothly and still fail if it does not advance the act/arc/hồi spine.

## Use when

- the user asks about act, arc, hồi, chapter, scene, outline, detailed outline, structural spine, borderbound, chapter card, scene packet, or prose permission;
- a rewrite or line edit risks fixing prose before the outline is clear;
- a chapter/scene has correct gates but still feels synthetic, unmoored, or AI-like;
- protagonist gain, supernatural residue, folklore, lore, or clue chain may not belong to the current chapter spine;
- the user asks to write, rewrite, line edit, or readiness-check a chapter that lacks current outline confirmation;
- the scene/chapter was produced from summary, taste, or checklist instead of current outline + packet.

## Authority

This gate does not create new act/arc structure, chapter cards, scenes, canon, lore, or outline content unless the user explicitly asks for a write/design action.

If current outline status matters, read current Notion first.

If the user asks for a prose patch and the spine is unclear, stop with OUTLINE_REPAIR_REQUIRED.

## Structural spine schema

```text
STRUCTURAL SPINE / OUTLINE PREFLIGHT
SCOPE:
SOURCE USED:
SOURCE SURFACE:
OUTLINE SOURCE STATUS:
ACT / ARC / HỒI:
ARC QUESTION:
ARC PRESSURE:
ARC PROMISE:
CHAPTER:
CHAPTER QUESTION:
CHAPTER FUNCTION:
CHAPTER ENGINE:
CHAPTER CHANGED STATE:
CHAPTER AFTERTASTE:
CHAPTER CARD STATUS:
SCENE LIST:
SCENE QUESTION PER SCENE:
SCENE FUNCTION PER SCENE:
PROTAGONIST GAIN PER SCENE:
SUPERNATURAL / LORE RESIDUE SLOT:
THREADS PLANTED / HELD / PAID:
CANON IN:
CANON OUT:
MUST SHOW:
MUST NOT REVEAL:
BORDERBOUND:
OUTLINE GAPS:
PROSE PERMISSION:
SAFE NEXT ACTION:
NEXT NODE:
```

## Proser outline routing addendum

For current SLTD Proser work, outline-to-prose descent must use the existing Notion route:

```text
Story Outline
-> Series Planning / Quyển Bank
-> Packet Beat Ledger
-> Chapter Index fields
-> Scene Bank fields
-> prose
```

Do not jump from Quyển / macro outline directly to prose.

Before scene expansion, confirm:

```text
source anchor or approved candidate source
Chapter Function
Map Zone
Access Gate
Cost
Payoff Debt
Must Not Reveal
Reader Effect or Scene Question
```

If any item is missing, return NODE MISSING / OUTLINE_REPAIR_REQUIRED and ask for source-lock or candidate fill before prose.

## Borderbound rule

A prose task is blocked when any of these is missing or contradictory for the requested scope:

```text
current Story Outline / macro route when chapter/arc direction is at stake
current Chapter by Chapter Outline when chapter function is at stake
Chapter Index / Chapter Card when current chapter status, goal, changed state, or risk is at stake
Scene Bank / Scene Packet when exact scene rewrite or line edit is at stake
Canon In / Canon Out
Must Show / Must Not Reveal
scene question and chapter question
changed state and reader effect
the allowed reveal boundary for lore, supernatural residue, or protagonist knowledge
```

## Outline repair before prose

If the detailed outline is thin, contradictory, or not source-current, do not compensate with prose.

Valid repair order:

```text
Story Outline / macro route
-> Chapter by Chapter Outline / detailed spine
-> Arc/Hồi spine
-> Chapter Card lock
-> Scene Packet lock
-> protagonist advancement slot
-> supernatural residue slot
-> source surface
-> prose rewrite / line edit
-> seam pass
-> anti-AI composite
-> readiness
```

## Failure labels

```text
OUTLINE_PREFLIGHT_MISSING
STRUCTURAL_SPINE_MISSING
CHAPTER_CARD_INCOMPLETE
SCENE_PACKET_INCOMPLETE
BORDERBOUND_MISSING
PROSE_BEFORE_OUTLINE
DETAIL_OUTLINE_TOO_THIN
CHAPTER_QUESTION_MISSING
SCENE_QUESTION_MISSING
CHANGED_STATE_MISSING
ARC_PRESSURE_UNMAPPED
PROTAGONIST_GAIN_OUT_OF_SPINE
SUPERNATURAL_SLOT_OUT_OF_SPINE
LORE_SLOT_OUT_OF_SPINE
CANON_OUT_UNCLEAR
MUST_NOT_REVEAL_MISSING
THREAD_PLANT_WITHOUT_ARC_SLOT
CHECKLIST_FIX_OVER_SPINE
SUMMARY_TO_PROSE_RISK
```

## Safe repair

Safe repair may:

- report missing outline/card/packet fields;
- propose a Notion update candidate for Story Outline, Chapter by Chapter Outline, Chapter Card, or Scene Packet;
- map scenes to chapter function without editing prose;
- mark which chapters/scenes are blocked from prose;
- decide that a prose request may proceed only in a smaller excerpt with source surface.

Safe repair must not:

- invent chapter purpose, scene function, arc promise, canon, lore, reveal, or payoff;
- hide outline gaps by writing more atmospheric prose;
- line edit a scene whose function is unconfirmed;
- let a later gate override missing structural source.

## Output labels

```text
STRUCTURAL_SPINE_OK
STRUCTURAL_SPINE_PARTIAL
OUTLINE_PREFLIGHT_REQUIRED
OUTLINE_REPAIR_REQUIRED
PROSE_PERMISSION_GRANTED
PROSE_PERMISSION_BLOCKED
SOURCE_SURFACE_REQUIRED
```
