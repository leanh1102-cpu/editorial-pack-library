# SLTD Memory Boundaries

This file defines what kind of memory each system layer is allowed to provide.

## GitHub memory

GitHub editorial-pack-library is rule memory and skill memory.

It stores:

- agent identity;
- author working profile;
- pack rules;
- prompts;
- samples;
- task routing;
- stop conditions;
- version history.

GitHub does not store the live manuscript unless the user explicitly puts a manuscript file there.

## Notion memory

Notion Story SLTD Proser is the live project memory.

It stores:

- current Chapter Index;
- Scene Bank;
- Chapter Review;
- Series Manuscript packet reads;
- Story Outline;
- canon indexes;
- live status and lock notes.

For current prose status, Notion wins.

## Chat memory

Conversation memory is not source of truth.

It may help maintain continuity in the current session, but it cannot override GitHub rules or Notion live source.

## Legacy memory

Google Doc, old Workdeck, old packets, old gates, old logs, and imported notes are historical memory.

They can explain how an error happened before. They cannot define current manuscript state when Notion has newer pages.

## Conflict resolution

If layers conflict, use this order:

1. user instruction in current turn;
2. Notion live source;
3. GitHub rule pack;
4. user-provided scene packet;
5. legacy documents;
6. chat memory.

If conflict affects canon or current chapter status, stop and ask or cite the current Notion source.
