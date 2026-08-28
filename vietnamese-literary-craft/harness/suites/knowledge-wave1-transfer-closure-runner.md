# KNOWLEDGE-WAVE1-TRANSFER-CLOSURE v0.1 — Blind Runner

## Isolation contract

STATUS: `FROZEN / TARGETED CLOSURE / RUNNER-ONLY`

PURPOSE: validate KX1 craft-transfer discipline after KV-02 showed correct mechanism transfer but insufficient surface differentiation.

Run in one clean conversation. Load only KX1 `analysis/close-reading.md`, the base skill operational files needed for the action taxonomy, and this runner. Do not consult evaluator/golden files, web/search, project memory, prior chat context, or outside sources.

Answer both cases in one uninterrupted response.

Return exactly one block per case:

`CASE_ID / ACTION / OUTPUT / REASON`

Allowed actions:

`PRESERVE / MIN_EDIT / REVISE / HOLD-INSUFFICIENT_EVIDENCE`

Do not score yourself.

---

### KT-01
TASK: repair the imitation so it transfers the mechanism while materially changing object, setting, relationship, practical functions, symbolic interpretation, diction, and scene furniture.
INPUT: MODEL MECHANISM: an ordinary recurring object changes practical and relational function across three scenes while one character gives it an unconfirmed symbolic interpretation. SOURCE SURFACE: an empty chair in a family home after a father leaves; nobody sits in it; a child drags it to a window; one character reads the chair as proof that the absent father is still present/returning. BAD IMITATION: a bench in another family home after a mother leaves; nobody sits on it; a child drags it to a doorway; one character says it means the mother will return. Create a materially different micro-example. Do not use furniture, a family-home setting, parent/child relationship, departure/return, doors/windows, or a symbolic meaning of continued presence/return.

### KT-02
TASK: repair the imitation by transferring the interactional mechanism without copying the model's scene, wording, relationship, action sequence, or repeated lexical item.
INPUT: MODEL MECHANISM: one repeated utterance changes social force across three turns as pressure escalates; repetition is functional because each occurrence responds to a new threshold. SOURCE SURFACE: a person says `Đừng`, then `Đừng mở`, then `Đừng mở cái cửa đó` as another hand moves from reaching for a latch to opening a door. BAD IMITATION: a sibling says `Thôi`, then `Thôi mở`, then `Thôi mở cái hộp đó` as another hand reaches for and opens a box. Create a different micro-example. Do not use siblings, doors/boxes/containers, opening/reaching actions, `đừng`, `thôi`, or a three-step expansion of the same phrase by merely adding words.

## Run completeness gate

A run is valid only if both cases are answered without evaluator/golden visibility or external context. If isolation is violated, label the run `CONTAMINATED`.
