# SLTD General + Chapter Feedback Matrix Check

Use this prompt when the user asks for multi-chapter, packet, arc, hồi, or whole-story feedback that should include both general feedback and chapter-specific feedback.

This prompt does not authorize source writes, prose edits, canon changes, or readiness claims without the relevant gates.

## Read first

```text
manifest.yml
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_general_chapter_feedback_matrix_output_protocol.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md
rules/sltd_tracking_logic_ledger_traceability_gate.md
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md
rules/sltd_supernatural_event_residue_dread_amplitude_gate.md
rules/sltd_protagonist_advancement_growth_route_gate.md
rules/sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md
```

## Output

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

## Rules

- Do not review from memory when current source is required.
- General feedback must frame chapter feedback.
- Chapter feedback must state status and next action.
- Surface-risk claims need exact prose or must be marked partial/source required.
- Readiness claims require readiness gates and current source evidence.
- Tracking risk must be included for object, residue, thread, knowledge, status, or downstream logic issues.
- If the user asks for JSON, return JSON-compatible keys from the protocol.
- End with NEXT_NODE.

## Blocked output

```text
SOURCE NOT READ / EVIDENCE MISSING
SCOPE:
MISSING SOURCE:
SAFE NARROWER CLAIM:
NEXT_NODE:
```