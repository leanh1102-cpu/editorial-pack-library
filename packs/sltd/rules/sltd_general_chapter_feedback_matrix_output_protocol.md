# SLTD General + Chapter Feedback Matrix Output Protocol

This protocol turns multi-chapter review into a traceable feedback matrix.

It is an output protocol, not a replacement for source preflight, tracking, structural spine, Vietnamese surface, supernatural residue, protagonist inquiry, or readiness gates.

## Core rule

General feedback must come before chapter feedback.

Chapter feedback must inherit the general diagnosis, not contradict it or drift into isolated comments.

```text
GENERAL_FEEDBACK = packet/story-level critique: spine, tracking, protagonist route, supernatural residue, Vietnamese surface, pass integrity, readiness risk
CHAPTER_FEEDBACK = chapter-specific feedback tied to chapter number, current status, core function, blockers, and next action
FEEDBACK_MATRIX = a structured review object that keeps packet-level issues and per-chapter issues visible together
SOURCE_STATUS = whether current Notion/source surface was read, partial, missing, or blocked
REVIEW_VERDICT = one of ready / partial / blocked / source missing / tracking blocked / surface blocked
```

Do not use the matrix to hide missing source.

Do not produce generic advice when SLTD source status is unclear.

Do not treat this output as publication readiness unless readiness gates have been run.

## Use when

- the user asks to review many chapters, packet, arc, hồi, C001-C033, C001-C060, or whole-story feedback;
- the user wants general feedback plus chapter-by-chapter critique;
- a packet needs a compact report for Notion, handoff, or next-session planning;
- several gates have produced findings and the result needs to be normalized into one output shape;
- the review should show both global blockers and local chapter actions.

## Authority

This protocol does not authorize source writes, canon changes, outline changes, prose edits, or readiness claims.

If current source is required but not read, output SOURCE NOT READ / EVIDENCE MISSING.

If tracking logic is required but missing, output TRACKING_SURFACE_MISSING or LOGIC_TRACE_BLOCKED.

If exact prose surface is required but missing, output SOURCE_SURFACE_REQUIRED.

## JSON-compatible schema

```text
GENERAL + CHAPTER FEEDBACK MATRIX
SCOPE:
SOURCE_USED:
SOURCE_STATUS:
REVIEW_MODE:
GENERAL_FEEDBACK:
  STRUCTURAL_SPINE:
  TRACKING_LOGIC:
  PROTAGONIST_ROUTE:
  SUPERNATURAL_RESIDUE:
  VIETNAMESE_SURFACE:
  PASS_INTEGRITY:
  READINESS_RISK:
  TOP_BLOCKERS:
CHAPTER_FEEDBACK:
  - CHAPTER_NUMBER:
    CHAPTER_TITLE:
    CURRENT_STATUS:
    CORE_FUNCTION:
    MAIN_FEEDBACK:
    TRACKING_RISK:
    SURFACE_RISK:
    READINESS_VERDICT:
    NEXT_ACTION:
EVIDENCE_CHECK:
NODE_LEDGER:
NEXT_NODE:
```

## JSON key option

When the user explicitly requests JSON, use exactly these top-level keys:

```json
{
  "SCOPE": "",
  "SOURCE_USED": "",
  "SOURCE_STATUS": "",
  "REVIEW_MODE": "",
  "GENERAL_FEEDBACK": {
    "STRUCTURAL_SPINE": "",
    "TRACKING_LOGIC": "",
    "PROTAGONIST_ROUTE": "",
    "SUPERNATURAL_RESIDUE": "",
    "VIETNAMESE_SURFACE": "",
    "PASS_INTEGRITY": "",
    "READINESS_RISK": "",
    "TOP_BLOCKERS": []
  },
  "CHAPTER_FEEDBACK": [
    {
      "CHAPTER_NUMBER": "",
      "CHAPTER_TITLE": "",
      "CURRENT_STATUS": "",
      "CORE_FUNCTION": "",
      "MAIN_FEEDBACK": "",
      "TRACKING_RISK": "",
      "SURFACE_RISK": "",
      "READINESS_VERDICT": "",
      "NEXT_ACTION": ""
    }
  ],
  "EVIDENCE_CHECK": "",
  "NODE_LEDGER": [],
  "NEXT_NODE": ""
}
```

## Matrix rules

- Start with source status.
- Separate global blockers from chapter-specific actions.
- Do not provide chapter-level certainty when only summary/index was read.
- Do not mark readiness without pass integrity and current source evidence.
- If a chapter has no exact prose read, label surface verdict as partial or source required.
- If a chapter touches object/residue/thread continuity, include tracking risk.
- If feedback is only strategic, say so.

## Failure labels

```text
MATRIX_SOURCE_MISSING
MATRIX_SOURCE_PARTIAL
GENERAL_FEEDBACK_TOO_GENERIC
CHAPTER_FEEDBACK_UNGROUNDED
CHAPTER_FEEDBACK_IGNORES_GENERAL_BLOCKER
READINESS_CLAIM_WITHOUT_GATE
TRACKING_RISK_OMITTED
SURFACE_RISK_OMITTED
STATUS_CONFLICT_OMITTED
JSON_SHAPE_DRIFT
```

## Output labels

```text
FEEDBACK_MATRIX_OK
FEEDBACK_MATRIX_PARTIAL
SOURCE_NOT_READ
MATRIX_BLOCKED
```