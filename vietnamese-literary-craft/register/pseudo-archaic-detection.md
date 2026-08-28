# KX10 — Pseudo-Archaic Detection

**Status:** `SOURCE-BACKED CANDIDATE / WAVE 1 / NARROW SOURCE SCOPE / DIAGNOSTIC ONLY / UNVALIDATED`

## CONCEPT
Pseudo-archaic detection identifies risk that language looks superficially old without sufficient historical/textual support. It is a conservative diagnostic module: it can flag unsupported archaizing, anachronism candidates, and textual-status problems, but it cannot authenticate period correctness from model memory or lexical appearance alone.

Core route:

`PERIOD CLAIM → TEXTUAL STATUS → SOURCE/EDITION → REGISTER SIGNALS → ANACHRONISM/ARCHAIZING RISK → EVIDENCE SUFFICIENT? → HOLD OR BOUNDED DIAGNOSIS`

## DEFINITION
- **Archaic/dated form:** a lexical, semantic, orthographic, syntactic, rhetorical, or discourse feature whose historical status is supported by dated textual or scholarly evidence.
- **Pseudo-archaic:** language designed or perceived as old-fashioned primarily through surface cues without adequate evidence that those cues fit the claimed period, institution, form, or textual layer.
- **Hán–Việt inflation:** increasing Sino-Vietnamese lexical density as a generic oldness signal without evidence that the resulting phrase/register is historically appropriate.
- **Anachronism candidate:** a feature whose apparent temporal mismatch requires verification before being called an error.
- **Textual status:** whether the object being judged is an original, transcription, translation, modernization, editorial adaptation, fictional facsimile, quoted document, or another mediated layer.
- **Edition policy:** explicit editorial choices about spelling, punctuation, lexical modernization, abbreviations, glossing, or normalization.
- **Authentication:** a positive claim that a form/register is historically correct for a specified period/context. This module does not perform authentication without sufficient evidence.

## TERMS
- archaic
- dated form
- pseudo-archaic
- Hán–Việt
- văn Hán
- Hán hóa
- anachronism
- provenance
- textual status
- edition
- modernization
- transcription
- translation
- gloss policy
- period register
- institution/title
- source gate

## SCOPE
Use this module when a task asks whether historical-looking Vietnamese prose is genuinely appropriate, artificially archaized, anachronistic, or textually mediated.

Use it to detect risk involving:
- unsupported Hán–Việt inflation;
- modern discourse markers inside an otherwise unmarked historical frame;
- unexplained mixture of historical-looking and contemporary register;
- official titles or institutional vocabulary without period/institution support;
- lexical forms claimed to be old without dated evidence;
- documents whose edited/translated/modernized status changes what should be judged.

Do not use it to:
- certify historical authenticity from intuition;
- equate Hán–Việt density with antiquity;
- confuse Hán–Việt vocabulary with văn Hán;
- modernize a text merely because contemporary readers find it strange;
- reconstruct a presumed original from an explicitly modernized edition without source evidence;
- invent a period title, honorific, orthography, or phrase from memory.

## MECHANISM
### 1. Identify the exact historical claim
Ask what is being claimed: period, reign, institution, region, document type, literary form, speaker social position, or editorial layer.

A vague request to make prose `cổ hơn` does not supply enough criteria for authentication.

### 2. Establish textual status
Determine whether the material is:
- original historical text;
- modern transcription;
- translation;
- modernization/adaptation;
- fictional historical narration;
- in-world document reproduced through a later editor;
- other mediated form.

Do not judge a modernized layer as though it were a diplomatic transcription of an original.

### 3. Require evidence appropriate to the claim
Potential evidence includes:
- dated primary texts;
- reliable dictionary/historical lexical scholarship;
- textual criticism/provenance;
- institution-specific historical studies;
- edition notes or translator/editor policy;
- form-specific scholarship.

### 4. Diagnose surface risk without authenticating
Flag risks such as:
- common modern Vietnamese mechanically replaced by dense Hán–Việt strings;
- register that becomes opaque while lacking a source model;
- modern bureaucratic/media/chat phrasing in an unmarked period voice;
- titles or honorifics used without known institutional context;
- inconsistent temporal layers within the same supposed document.

A risk flag means `needs evidence`, not `historically wrong`.

### 5. Apply the HOLD boundary
If a materially necessary period, institution, source, edition, provenance, or gloss/modernization policy is missing, use `HOLD-INSUFFICIENT_EVIDENCE` for the historical verdict.

You may still state the narrower supported diagnosis, e.g. `Version B is more Hán–Việt-dense, but that does not establish that it is more historically authentic.`

### 6. Respect explicit modernization
If a document is explicitly presented as modernized by an editor/translator—inside the fiction or in the actual edition—modern spelling, punctuation, or common abbreviations may belong to that editorial layer and are not automatically period errors.

## TEXTUAL SIGNALS
Potential risk signals:
- abrupt density of Sino-Vietnamese compounds unsupported by the surrounding register;
- literal calque-like strings produced by replacing common words with formal/Hán–Việt alternatives;
- modern abbreviations, institutional phrases, media language, or conversational markers inside an unmarked historical document;
- historically specific titles with no supplied dynasty/institution;
- mixture of contemporary punctuation/lexicon with an alleged unmediated original;
- archaic spellings whose edition status is unknown;
- narrator notes declaring modernization, translation, transcription, or editorial intervention;
- lexical forms whose current meaning differs from meanings attested in older sources.

Signals are prompts for source checking, not automatic error labels.

## EFFECTS
Careful source-gated diagnosis can preserve:
- historical plausibility without fake certainty;
- distinction between source text and editorial layer;
- reader trust in period detail;
- meaningful register difference;
- author freedom to stylize without falsely calling stylization documentary authenticity.

Poor diagnosis can create pseudo-history by replacing uncertainty with invented confidence.

## CONDITIONS
A positive historical/register verdict requires evidence matched to the claim. Depending on the task, materially necessary fields may include:
- period/date;
- court/institution/region;
- document/form type;
- source or comparable corpus;
- edition/transcription/translation status;
- house gloss/modernization policy.

When these are absent and matter to correctness, HOLD.

A narrower risk diagnosis is allowed when the evidence only supports the risk. Example: `mechanical Hán–Việt substitution is visible` is narrower than `this phrase is historically wrong`.

## COUNTEREXAMPLES
- `Người lính đi vào nhà hỏi chuyện` versus `Quân sĩ nhập thất vấn sự`: the second is more Hán–Việt-dense, but without period/form/source evidence neither can be certified as more authentic.
- A title `X` cannot be judged period-correct without dynasty/institution/region/source context.
- A fictional 1895 deposition containing a modern abbreviation need not be repaired if the narrative explicitly states that a 2020 editor modernized common abbreviations.
- A seventeenth-century lexical form attested in dated manuscripts may legitimately differ from modern usage; contemporary unfamiliarity does not make it wrong.
- An intentionally stylized fantasy register can be artistically functional without claiming documentary historical authenticity.

## COMMON ERRORS
- `more Hán–Việt = more ancient`;
- `less understandable = more authentic`;
- treating Hán–Việt and văn Hán as the same thing;
- inventing official titles from genre familiarity;
- correcting an explicitly modernized edition back toward an imagined original;
- calling every contemporary-looking feature an anachronism before checking textual status;
- applying modern standard Vietnamese as the correction norm for older texts;
- using one historical corpus to certify all periods;
- presenting model memory as provenance.

## HISTORICAL VARIATION
Historical variation is the subject of this module but remains source-gated at the claim level.

Evidence from one period or corpus does not automatically generalize to another. Lexical form can survive while meaning changes; orthographic/editorial representation can also differ from the historical original.

## FORM VARIATION
`SOURCE-GATED BY FORM`.

Chiếu, biểu, hịch, phú, biền văn, ký, truyền kỳ, poetry, legal documents, private letters, chronicles, translations, and modern historical fiction can use different registers and conventions. Do not infer form-law or historical diction from label alone.

## CLOSE READING METHOD
Build a source-status map before judging:

`CLAIMED PERIOD/FORM → WHOSE VOICE → TEXTUAL LAYER → SOURCE/EDITION → OBSERVABLE REGISTER FEATURES → WHAT IS VERIFIED → WHAT IS ONLY SUSPECTED → VERDICT/HOLD`

Keep three outputs distinct:
1. **observable surface:** what the passage actually does;
2. **risk diagnosis:** what may be pseudo-archaic/anachronistic;
3. **historical verdict:** only what evidence can establish.

## CRAFT TRANSFER
For historical stylization, transfer evidence-backed mechanisms rather than generic old-looking vocabulary.

Possible process:
1. choose a verified period/form source model;
2. identify recoverable patterns in address, syntax, lexical distribution, textual conventions, or document structure;
3. distinguish original features from editorial modernization;
4. create new prose without copying source wording;
5. label remaining uncertainty instead of filling it with Hán–Việt density.

## DRILLS
1. Compare two supposed old-style sentences and separate `surface density` from `historical evidence`.
2. Given a title with missing dynasty/institution, choose between repair and HOLD.
3. Classify ten features as `VERIFIED DATED / ANACHRONISM CANDIDATE / EDITORIAL LAYER / UNSUPPORTED ARCHAIZING`.
4. Diagnose a modernized historical document without reconstructing its presumed original.
5. Rewrite a pseudo-archaic sentence only after a supplied source model establishes the target register.

## AI OPERATIONAL RULES
- KX10 detects risk; it does not authenticate history from memory.
- Hán–Việt density is not evidence of period authenticity.
- Distinguish Hán–Việt, văn Hán, and Hán hóa; do not collapse them.
- Missing materially necessary period/institution/source/edition/gloss policy → `HOLD-INSUFFICIENT_EVIDENCE`.
- State the narrower supported diagnosis when a full verdict is blocked.
- Do not invent official titles, honorifics, period lexical meanings, or form-law.
- Check textual status before calling a feature anachronistic.
- Explicit modernization/translation/editing can legitimately introduce contemporary spelling, punctuation, or abbreviations into a representation of an older document.
- Do not modernize older language solely because it differs from contemporary standard Vietnamese.
- Evidence from one historical corpus remains bounded to its demonstrated scope.

## SELF-CHECK
- What exact period/form/institution is being judged?
- What is the textual layer: original, transcription, translation, modernization, or fiction?
- What source proves the historical status I am about to claim?
- Am I equating Hán–Việt density with authenticity?
- Is the supposed anachronism actually part of a declared editorial layer?
- Did I infer a title/honorific/meaning from memory?
- Is the evidence period-specific enough?
- Should the correct action be HOLD rather than correction?

## SOURCES
External source backbone:
- Vũ Đức Nghiệu (2010), *Khảo sát các từ cổ trong ba văn bản viết bằng chữ Quốc ngữ thế kỷ XVII*. Used for the principle that dated textual evidence with provenance can establish historical lexical/semantic difference, including forms whose historical meanings differ from current meanings. Its findings are bounded to the surveyed seventeenth-century corpus and do not authenticate arbitrary fictional prose.
- The same study's documented manuscript dates, repository/provenance information, modern transcription, and facsimile relationship support the need to distinguish original textual evidence from later representational/editorial layers.

Validated internal dependencies:
- `curriculum/ADVANCED.md` A7 historical-cultural mediation/textual status and A6 source-gated register/form boundaries.
- `register/modern-vietnamese.md` for the limit of modern-register judgments.
- Wave 1 Source Claim Ledger.

The exact HOLD action, required evidence fields, and conservative authentication boundary are internal validated operational policy. They are not presented as universal historical-linguistic laws derived solely from the external source.