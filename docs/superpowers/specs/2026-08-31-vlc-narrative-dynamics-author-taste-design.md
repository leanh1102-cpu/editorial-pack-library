# VLC Narrative Dynamics + Author-Taste Golden v0.1 — Design

## Status
`LOCKED DESIGN / IMPLEMENTATION AUTHORIZED / GOLDEN CANDIDATE ONLY`

## Goal
Nâng Vietnamese Literary Craft từ phán đoán chủ yếu ở câu/đoạn/exchange lên phán đoán nhiều tầng `sentence → exchange → scene → beat → chapter/arc → reader effect`, dùng human-approved Vietnamese prose controls và production deltas để hiệu chuẩn mà không biến gu tác giả thành quota hoặc công thức máy.

## Source boundary
- `editorial-pack-library` là source-of-record cho VLC rules, sanitized golden candidates, harness và runtime snapshots.
- Nguồn prose nội bộ của các dự án khác chỉ là evidence upstream. Không copy canon, tên riêng, đoạn văn dài, link private hoặc manuscript body vào repo public.
- Provenance chi tiết giữ ở private Notion/Drive staging; public repo chỉ giữ source class, mechanism, anonymized/synthetic case và scope.
- Không sửa `pai-control-plane`, repo Linux/PAI khác, `core/`, `packs/sltd/`, `CONSTITUTION.md` hoặc workflow/automation trong roadmap này.

## Repository separation / future PAI integration
`editorial-pack-library` và `pai-control-plane` là hai repository độc lập. VLC được phát triển và validate tại repo editorial. PAI sau này chỉ consume một runtime snapshot đã validate theo commit-pinned contract. Không vendor ngược PAI runtime/governance vào VLC và không dùng subtree/submodule như source-of-truth kép trong v0.1.

Future flow:
`VLC main → validated runtime snapshot → pinned commit/hash → PAI Git consumer/import layer → PAI-specific UAT/receipt`

PAI không được tự promote một VLC candidate chưa qua golden/holdout/regression gate.

## Locked roadmap

### Layer 1 — Vietnamese Prose / Author-Taste Golden
Mục tiêu: học decision boundary về văn Việt tự nhiên, không học bề mặt câu chữ.

Candidate sources:
- owner-approved positive controls từ một dự án prose nội bộ đã qua review;
- production before/after deltas nơi người viết phải sửa AI;
- reader-effect evidence khi có phàn nàn lặp và có thể quy về mechanism.

Các mechanism ưu tiên:
- câu trung bình/dài làm nền; câu ngắn chỉ khi có chức năng;
- ít lời ≠ proposition-only terse saturation;
- relational texture qua xưng hô, hư từ, vòng lời, tự sửa, giữ mặt;
- im lặng/hậu quả được dựng bằng vật, thân thể, hành động thay vì dán nhãn;
- việc nhà và vật cụ thể mang kinh tế, quan hệ, cost;
- kết scene bằng chuyển động/áp lực cụ thể thay vì châm ngôn;
- giữ độ gồ ghề sống, không polish mọi câu thành cùng một độ sắc.

Không tạo quota số từ/câu/turn.

### Layer 2 — Scene Dynamics Golden
Mục tiêu: phát hiện cảnh đúng từng câu nhưng phẳng ở cấp vận động.

Core model:
`STATE → PRESSURE → CHOICE/RESISTANCE → TURN → CONSEQUENCE → RECOVERY/NEW PRESSURE`

Không bắt mọi scene đủ sáu ô. Đây là diagnostic map, không template.

Phải phân biệt:
- quiet beat có chức năng vs scene thiếu lực;
- escalation bằng cost/choice vs chỉ tăng âm lượng;
- short-turn cluster có social action vs terse saturation;
- aftermath/recovery beat vs filler;
- reveal/payoff thay đổi cách hiểu/tình thế vs chỉ thêm information.

### Layer 3 — Chapter / Arc Rhythm Harness
Mục tiêu: kiểm variation xuyên nhiều scene/chapter.

Phát hiện:
- nhiều scene liên tiếp cùng mechanism vận động;
- pressure plateau;
- climax đến không có tích lực hoặc cost;
- thiếu aftermath;
- repeated negotiation/information beats;
- cao trào cùng loại lặp lại;
- seam không tạo câu hỏi/pressure mới;
- mọi scene đều tiết chế hoặc mọi scene đều gào.

Không áp quota kiểu “mỗi chương phải có N beat”.

### Layer 4 — Author-Taste Holdout
TRAIN/REFERENCE và HOLDOUT phải tách.

Holdout phải:
- chưa được skill đọc trong authoring cycle;
- lấy từ scene/chapter khác source span hoặc dự án khác;
- được freeze trước khi candidate module nhìn thấy evaluator;
- test mechanism transfer, không surface imitation.

Không dùng training source để tuyên bố generalization.

## Public corpus contract
Mỗi public candidate item có:
- `ID`
- `SOURCE_CLASS` (không private URL)
- `SCOPE`
- `OBSERVABLES`
- `MECHANISM`
- `FAILURE_BOUNDARY`
- `PRESERVE_BOUNDARY`
- `ANONYMIZED_CASE`
- `TRANSFER_RISK`
- `STATUS`

Không lưu raw manuscript excerpt dài hoặc project canon.

## Evaluation model
Mở rộng evaluation nhưng không biến điểm số thành prose rule.

Các trục mới:
- `VIETNAMESE_RELATIONAL_TEXTURE`
- `EXCHANGE_VARIATION`
- `SCENE_PRESSURE_DYNAMICS`
- `CHOICE_COST_CONSEQUENCE`
- `RECOVERY_AFTERMATH`
- `CHAPTER_RHYTHM_VARIATION`
- `AUTHOR_TASTE_TRANSFER`
- `SURFACE_IMITATION_RISK`

Hard-fail examples:
- copy surface/canon từ source training sang case mới;
- tự thêm plot fact để “làm cao trào”;
- kéo dài mọi câu/thoại để chống terse saturation;
- áp quota beat/câu/turn;
- xóa quiet beat có chức năng chỉ vì “thiếu action”;
- biến inference thành fact;
- rewrite rộng khi defect chỉ cục bộ;
- dùng holdout sau khi đã lộ evaluator/source.

## Runtime behavior target
Khi WRITE/REVISE fiction, skill phải có thể chạy hidden self-check ở ba scale:
1. utterance/sentence;
2. exchange/scene;
3. chapter-context nếu packet có nhiều scene.

Self-check không được leak thành checklist trong prose output.

## Promotion gates
1. Candidate corpus frozen.
2. RED harness frozen trước module patch.
3. Targeted prose/taste suite full pass, hard fail 0.
4. Scene dynamics suite full pass, hard fail 0.
5. Chapter/arc rhythm suite full pass, hard fail 0.
6. Holdout transfer pass, surface imitation hard fail 0.
7. Existing BASELINE-36 + sensory + cross-layer + dialogue-texture regressions clean/composite-closed.
8. `CONSTITUTION.md` unchanged; no `core/`, `packs/sltd/`, workflows, automations or PAI repo writes.
9. Only then update router/index, merge, and refresh runtime snapshot.

## PAI Git consumer contract (future)
PAI integration is a separate downstream change. It should consume:
- runtime snapshot branch/ref;
- exact source commit SHA;
- package status (`RUNTIME-VALIDATED` only when earned);
- compatibility/receipt metadata.

PAI-side changes remain governed by PAI's own C0–C4 classification, tests, rollback, evidence and receipts. VLC merge does not imply PAI deployment.
