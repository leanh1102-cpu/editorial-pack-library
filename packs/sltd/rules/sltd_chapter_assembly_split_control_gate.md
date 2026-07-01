# SLTD Chapter Assembly & Split Control Gate

This gate controls chapter assembly after scene-level editing.

It prevents a chapter from becoming an overfilled container that holds too many scene units, reader promises, turns, or payoffs.

## Core rule

Scene is the edit unit. Chapter is the reader unit. Packet is the continuity and momentum unit.

A scene can pass and the chapter can still fail.

Do not assume that edited scenes automatically assemble into a readable chapter.

## Use when

- scene-level edits are being assembled into a chapter;
- chapter length becomes large or unclear;
- a chapter approaches or exceeds the project warning range;
- a chapter contains multiple major turns, reader promises, or payoff points;
- the chapter feels like several chapters joined together;
- readiness fails because the chapter is too heavy, not because each scene is weak;
- the user asks whether to split, merge, shorten, or restructure chapters.

## Authority

This gate sits below:

```text
current user instruction
current Notion source or user-provided source packet
source fidelity gate
canon guard
evidence discipline
role boundary contracts
```

It must not delete source, change canon, alter locked outcome, or silently split a live manuscript.

It may recommend split structure, but writing to Notion requires explicit user permission.

## Length risk bands

Use word-count bands as warnings, not absolute law:

```text
< 2500 words = usually safe if the chapter has sufficient pressure
2500-4500 words = healthy webnovel chapter range
4500-6500 words = run chapter assembly check
6500-8000 words = high split risk
8000+ words = must justify keeping as one or propose split
```

If the count is characters, not words, label it clearly and do not apply word-count bands mechanically.

Length alone does not decide split.

Reader unit decides split.

## Reader unit test

Ask:

```text
PRIMARY READER QUESTION:
GOVERNING CHAPTER PRESSURE:
MAJOR TURNS:
PAYOFF POINTS:
OPEN LOOPS:
CLOSED LOOPS:
NATURAL BREAKPOINTS:
CHAPTER-END HOOKS:
```

A chapter is at split risk when it has more than one reader unit.

## Split triggers

Consider split when:

- there is more than one major turn;
- there is more than one scene climax;
- there are two or more reader promises pulling in different directions;
- a scene creates a natural chapter-end hook;
- the chapter changes reading goal after midpoint;
- an early payoff is buried under later scenes;
- the title no longer covers the chapter;
- the chapter requires internal recap to stay readable;
- mobile reading fatigue appears before the main payoff;
- readiness fails from weight rather than weak scenes.

## Keep-as-one conditions

A long chapter may stay whole when:

- one governing pressure pulls all scenes;
- one primary reader question remains active;
- every scene tightens the same chapter pressure;
- payoff size justifies the length;
- the chapter end creates a clear changed state;
- there is no natural breakpoint stronger than the final hook.

## Assembly audit

Use:

```text
CHAPTER ASSEMBLY & SPLIT CHECK
SCOPE:
SOURCE USED:
SOURCE SURFACE:
SCENES INCLUDED:
TOTAL LENGTH:
LENGTH TYPE: words / characters / unknown
CHAPTER FUNCTION:
GOVERNING CHAPTER PRESSURE:
PRIMARY READER QUESTION:
MAJOR TURNS:
PAYOFF POINTS:
OPEN LOOPS:
CLOSED LOOPS:
NATURAL BREAKPOINTS:
SPLIT RISK:
RECOMMENDED STRUCTURE:
IF KEEP AS ONE:
IF SPLIT:
ROLE HANDOFF:
NEXT NODE:
```

## Recommended structures

Use one of:

```text
KEEP_AS_ONE
SPLIT_RECOMMENDED
SPLIT_REQUIRED
MERGE_WITH_NEIGHBOR
SHORTEN_WITHOUT_SPLIT
REORDER_SCENES_BEFORE_DECISION
SOURCE_SURFACE_REQUIRED
```

## Split recommendation

When proposing split, specify:

```text
PART A:
- scenes:
- reader question:
- ending hook:

PART B:
- scenes:
- reader question:
- opening pickup:
- ending hook:
```

Do not rewrite or renumber live chapters unless explicitly asked.

## Handoff

If scene content is not exact, hand off to Source Surface Check.

If the chapter has no governing pressure, hand off to Story Doctor or First-Pass Editorial Workflow.

If the chapter is synthetic after assembly, hand off to Anti-AI Composite Check.

If split affects readiness, hand off to Publishing Readiness Reviewer.

## Output labels

```text
CHAPTER_ASSEMBLY_OK
SPLIT_RISK_WARN
SPLIT_RECOMMENDED
SPLIT_REQUIRED
ASSEMBLY_REORDER_NEEDED
SOURCE_SURFACE_REQUIRED
```
