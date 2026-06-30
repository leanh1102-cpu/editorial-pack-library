# SLTD Editorial Mindmap

This file defines the static editorial map for SLTD AI work.

It is not a live status board. It does not replace Notion relation, rollup, lookup, Chapter Index, Scene Bank, or packet pages.

## Purpose

The mindmap helps an AI know which nodes exist, which nodes it has passed, which nodes remain open, and which node blocks the next conclusion.

## Source nodes

- User current instruction
- Notion Story SLTD Proser
- Notion Chapter Index
- Notion Scene Bank
- Notion Series Manuscript
- Notion Chapter Review
- Notion Story Outline
- Notion Plot Threads
- Notion Character index
- Notion Worldbuilding index
- Notion Location index
- Notion Timeline
- User-provided scene packet
- Legacy Google Doc or Workdeck

## Editorial role nodes

- Canon Guard
- Story Doctor
- Intensity Editor
- Vietnamese Line Editor
- Copyeditor
- Proofreader
- Publishing Readiness Reviewer
- Editorial Director

## Output nodes

- audit only
- rewrite
- patch suggestion
- story priority
- readiness verdict
- node checkpoint
- Notion update candidate

## Blocking nodes

These nodes block final conclusions:

- source not confirmed;
- current vs legacy source conflict;
- chapter lock status unclear;
- linked Scene Bank source missing;
- Human Chapter Pass missing when publication readiness is requested;
- Publication Lock not ready when packet lock is requested;
- a chapter inside a packet is not ready;
- canon conflict without current decision.

## Routing examples

### Current chapter audit

```text
BOOT -> SOURCE NODE -> CHAPTER INDEX -> SCENE BANK if needed -> CANON GUARD -> STORY DOCTOR -> INTENSITY EDITOR -> VIETNAMESE LINE EDITOR -> NODE CHECKPOINT
```

### Packet audit

```text
BOOT -> SOURCE NODE -> SERIES MANUSCRIPT -> CHAPTER INDEX LOCK CHECK -> STORY DOCTOR -> PUBLISHING READINESS REVIEWER -> EDITORIAL DIRECTOR -> NODE CHECKPOINT
```

### Scene rewrite

```text
BOOT -> SOURCE NODE -> SCENE BANK -> BEFORE_REWRITE HOOK -> CANON GUARD -> INTENSITY EDITOR -> VIETNAMESE LINE EDITOR -> AFTER_REWRITE HOOK -> NODE CHECKPOINT
```

## Rule

Use only the nodes needed for the user request.

Do not create new Notion pages, GitHub issues, workflows, reports, boards, or scripts from this map.
