# KX2 — Implicature, Reference, and Inference

**Status:** `SOURCE-BACKED CANDIDATE / WAVE 1 / UNVALIDATED`

## CONCEPT
Literary language operates across several epistemic layers at once: what a sentence explicitly says, what an utterance plausibly does in context, what a character or narrator claims, what a reader infers, and what the story has actually established.

This module keeps those layers separate so editing does not convert implication into fact or repair ambiguity by inventing information.

## DEFINITION
- **Sentence meaning:** the linguistically encoded content recoverable from the sentence itself.
- **Situated utterance meaning:** what the utterance plausibly communicates or does in a particular context.
- **Explicit content:** what is directly stated.
- **Implicature/inferred social action:** meaning or communicative force inferred from context rather than explicitly encoded.
- **Reference:** the relation by which an expression such as a name, pronoun, or noun phrase identifies an entity in context.
- **Claim:** a proposition attributed to a character, narrator, witness, document, memory, or other source whose truth status may still be unresolved.
- **Story fact:** information established by the narrative evidence available under the relevant contract.

## TERMS
- sentence meaning
- utterance meaning
- explicit content
- implicature
- speech act / communicative force
- reference
- antecedent
- ambiguity
- claim
- belief
- inference
- fact
- attribution
- source status

## SCOPE
Use this module when a task involves:
- indirect requests, warnings, accusations, promises, or other speech acts;
- pronoun/reference ambiguity;
- witness statements, reports, memories, documents, or allegations;
- reader inference versus narrator-confirmed information;
- revisions that risk changing epistemic status.

This is not a comprehensive theory of Vietnamese semantics/pragmatics. It does not infer hidden intention from model intuition.

## MECHANISM
### 1. Separate encoded content from contextual force
Ask first: what was literally/explicitly said? Then ask separately: what social action is plausible in context?

Example:
`Ở đây gió lùa quá.`

Explicit content: a statement about the room condition.
Plausible contextual force: an indirect request to close a window.
The second does not become explicit content merely because it is plausible.

### 2. Track source attribution
For every proposition that matters, ask:
- who supplied it?
- is it observed, remembered, alleged, inferred, or narratively established?
- has another source verified it?

### 3. Resolve reference only from supplied evidence
If an ambiguous pronoun has a materially important referent:
- intended referent supplied → `MIN_EDIT` the local expression;
- intended referent not supplied and cannot be recovered → `HOLD-INSUFFICIENT_EVIDENCE` rather than guessing.

### 4. Preserve epistemic status through revision
A cleaner sentence is a regression if it turns a character's allegation into narrator fact.

## TEXTUAL SIGNALS
- indirect declaratives in contexts where action may be expected;
- pronouns with more than one plausible antecedent;
- verbs of saying, believing, remembering, seeing, hearing, suspecting;
- free indirect or close-third passages where source boundaries can blur;
- documents/letters/reports whose contents are quoted or summarized;
- modal or evidential language such as `có lẽ`, `hình như`, `nghe nói`, `theo lời`;
- shifts from attributed claim to unqualified declarative syntax.

## EFFECTS
Maintaining these distinctions can preserve:
- ambiguity without confusion;
- indirect dialogue;
- mystery/fair play;
- unreliable or limited narration;
- character bias;
- legal/social consequence attached to who knows or claims what;
- reader participation in inference.

## CONDITIONS
A pragmatic or referential interpretation is defensible when:
- contextual cues support it;
- alternative readings are considered where material;
- explicit content and inferred force remain separately labeled;
- reference resolution does not invent an antecedent;
- story-fact status is supported by the narrative evidence available to the relevant narrator/character frame.

## COUNTEREXAMPLES
- A statement near an open window may function as a request, but that does not mean an explicit request was spoken.
- A witness can sincerely report something false; sincerity and accuracy are distinct.
- A narrator or focal character can believe a proposition without the story establishing it as fact.
- A smoother revision can be worse if it removes attribution.
- Pronoun ambiguity is not automatically a defect; it becomes a repair target when the ambiguity is unintended and materially consequential.

## COMMON ERRORS
- converting implicature into explicit wording merely to make dialogue clearer;
- reporting a character allegation as fact;
- treating memory as verified history;
- choosing a pronoun referent from intuition when the packet does not supply enough evidence;
- explaining indirect speech that readers can already infer;
- erasing uncertainty because one reading seems more likely;
- using probability language without preserving source attribution.

## HISTORICAL VARIATION
`SOURCE-GATED`.

Pragmatic conventions and reference systems may vary historically and socially. Do not infer period-specific speech force, honorific value, or lexical reference without relevant evidence.

## FORM VARIATION
Indirectness, attribution, and reference operate across forms, but dramatic dialogue, epistolary narration, oral-style storytelling, classical prose, poetry, and documentary fiction may encode them differently. Form-specific rules remain source-gated until the relevant module exists.

## CLOSE READING METHOD
For a materially important proposition, build a compact epistemic map:

`WORDS ON PAGE → SOURCE → EXPLICIT CONTENT → PLAUSIBLE INFERENCE/FORCE → VERIFICATION STATUS → NARRATIVE CONSEQUENCE`

For reference:

`REFERRING EXPRESSION → POSSIBLE ANTECEDENTS → CONTEXTUAL EVIDENCE → MATERIAL CONSEQUENCE → REPAIR/HOLD`

## CRAFT TRANSFER
To create indirect dialogue, do not merely remove imperative grammar. Build a context in which:
- the literal statement is natural;
- relation/status/pressure makes an indirect action plausible;
- the listener has enough context to infer but not necessarily enough to be certain;
- the narration does not explain the inference redundantly.

To create epistemic tension, separate:
`what happened / what character believes / what character says / what reader currently believes`.

## DRILLS
1. Label ten propositions `EXPLICIT / IMPLICATURE / CLAIM / INFERENCE / FACT`.
2. Rewrite an allegation twice: once preserving attribution, once incorrectly collapsing it; explain the regression.
3. Given three ambiguous pronouns, repair only those whose ambiguity changes a material consequence.
4. Write an indirect request whose literal content remains natural even if the listener ignores the implication.
5. Build a four-layer map: event / belief / statement / reader belief.

## AI OPERATIONAL RULES
- Never promote a plausible implicature into explicit fact.
- Never convert witness/character/document claims into narrator fact without verification.
- If a reference ambiguity is material and the intended referent is supplied, use the smallest local repair.
- If a material referent is not recoverable from supplied evidence, use `HOLD-INSUFFICIENT_EVIDENCE` rather than guessing.
- Preserve uncertainty when the narrative deliberately supports more than one reading.
- Do not explain an implicature inside the prose merely because the model can infer it.
- When revising, check whether a wording change altered source attribution or certainty.

## SELF-CHECK
- What is explicitly stated?
- What am I inferring from context?
- Who is the source of each proposition?
- Did I turn a claim into fact?
- Is the referent actually supplied or am I guessing?
- Did the revision increase certainty without new evidence?
- Is ambiguity intentional, accidental, or simply unresolved?

## SOURCES
External source backbone:
- Phạm Thị Hòa (2009), *Ngữ dụng học với việc dạy đọc hiểu một văn bản bằng tiếng nước ngoài*. Used for context-sensitive utterance meaning and communicative force beyond sentence-level syntax/semantics; does not authorize certainty about unstated intention.

Validated internal dependencies:
- `curriculum/FOUNDATION.md` F1/F5.
- `curriculum/INTERMEDIATE.md` I1/I4/I8 for access, dialogue as social action, and fact/belief/claim/inference layering.
- Wave 1 Source Claim Ledger.

Project-specific action labels, HOLD behavior, and epistemic regression tests are internal validated operational policy, not claims attributed to the external source.
