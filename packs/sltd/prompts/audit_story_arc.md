# SLTD Story Arc Audit

Dùng prompt này khi người dùng yêu cầu rà mạch truyện, lực kéo chương, promise/payoff, hoặc so cụm chương với benchmark cơ học đọc truyện mạng.

## Phạm vi

Chỉ audit trong phạm vi người dùng giao:

- một chương;
- một cụm chương;
- một hồi;
- một tuyến promise/payoff.

Không rewrite văn xuôi nếu người dùng chỉ yêu cầu audit mạch.

## File cần đọc

1. `AI_ENTRY.md`
2. `packs/sltd/manifest.yml`
3. `packs/sltd/PACK.md`
4. `packs/sltd/rules/sltd_canon_guard.md`
5. `packs/sltd/rules/sltd_story_momentum.md`
6. Nguồn chương hoặc workdeck người dùng cung cấp

Nếu thiếu nguồn chương, dừng và ghi `[CẦN DỮ LIỆU: chương/cụm chương cần audit]`.

## Kiểm 7 trục

### 1. Chapter hook

Chương kéo người đọc bằng gì: nguy cơ, bí mật, nợ, vật lạ, lời né, dấu hiệu, hay hậu quả?

### 2. Changed state

Sau chương, thứ gì đổi? Ghi ngắn:

```text
BIẾT THÊM:
MẤT / NỢ:
NGUY CƠ MỚI:
VẬT / DẤU / NGƯỜI LIÊN QUAN:
```

### 3. Cost ledger

Đại Phong hoặc phe liên quan đạt gì, trả gì, để lộ gì?

### 4. Promise/payoff

```text
GIEO:
TRẢ:
TREO:
NGUY CƠ QUÊN:
```

Không tự đoán payoff nếu nguồn chưa có.

### 5. Competence ladder

Đại Phong giỏi hơn nhờ quan sát, thử sai, chịu đau, nhớ chi tiết nhỏ, hiểu giá, hay chỉ nhờ may?

### 6. Mystery pressure

Hồn sương, Trọc khí, Quy Tức, Mảnh Đá Lạnh, Mê Thúy Lâm hoặc yếu tố kỳ dị khác có giữ câu hỏi và giá phải trả không?

### 7. Benchmark guard

Nếu người dùng yêu cầu đối chiếu Quỷ bí chi chủ hoặc Cổ chân nhân, chỉ dùng làm benchmark cơ học:

```text
QBTC: câu hỏi, chứng cứ, trì hoãn, giá lore.
CCN: tính toán, tài nguyên, cái giá, logic sinh tồn.
```

Không mượn văn phong, hệ thống, nhân vật, motif, tổ chức, hoặc plot.

## Đầu ra chuẩn

```text
STATUS: PASS / WEAK PASS / NOT PASS
SCOPE: ...
PACK: sltd@1.2.0

MẠCH CHÍNH:
- ...

ĐIỂM KÉO ĐỌC:
- ...

SỔ GIÁ PHẢI TRẢ:
ĐẠT ĐƯỢC:
MẤT / NỢ / ĐAU:
AI BIẾT HOẶC NGHI NGỜ:

PROMISE / PAYOFF:
GIEO:
TRẢ:
TREO:
NGUY CƠ QUÊN:

RỦI RO MẠCH:
1.
2.
3.

KHUYẾN NGHỊ:
- Giữ:
- Siết:
- Cần nguồn thêm:
```

## Luật dừng

Dừng khi:

- thiếu nguồn chương;
- người dùng yêu cầu so benchmark nhưng không nêu phạm vi;
- audit đòi hỏi canon chưa có trong nguồn;
- phát hiện mâu thuẫn nguồn mà không có bản chốt.

Không ghi vào Notion hoặc GitHub nếu người dùng chưa yêu cầu rõ.
