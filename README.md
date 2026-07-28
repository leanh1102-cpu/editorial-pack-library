# Editorial Pack Library

Repo này là thư viện gói biên tập. Nó không thay Notion, không giữ task, không giữ bản thảo sống, không sync dữ liệu.

## Mục đích

- Giữ rule biên tập ổn định.
- Giữ prompt dùng lại nhiều lần.
- Giữ sample tốt/xấu để AI bắt giọng.
- Tách phần dùng chung khỏi phần riêng từng dự án.
- Khóa cách giao bản thảo, tiêu chí pass/fail, và lỗi đỏ.

## Ranh giới cứng

AI không dùng repo này để:

- quản task;
- tạo bảng tiến độ;
- tạo workflow;
- mở issue;
- sửa cấu trúc Notion;
- lưu bản thảo đang làm;
- tự mở rộng canon.

Mỗi file phải thuộc một trong năm vai trò:

1. manifest
2. pack note
3. rule
4. prompt
5. sample

Các file trong `core/job_packet/` và `CHANGE_POLICY.md` là rule/pack note. Không thêm vai trò thứ sáu nếu người dùng chưa chốt.

## Cấu trúc

```text
core/               # luật, prompt, sample dùng chung
core/job_packet/    # giao bài, tiêu chí đạt, lỗi đỏ
packs/<project_id>/ # gói riêng từng dự án
```

Core không chứa canon riêng của dự án. Pack riêng không sửa core để chữa lỗi cục bộ.

## Khi AI dùng thư viện

AI phải bắt đầu từ `AI_ENTRY.md`. Nếu không đọc được pack, AI không được báo đã áp dụng pack.

## Khi sửa thư viện

Đọc `GOVERNANCE.md`, sau đó đọc `CHANGE_POLICY.md`. Mọi thay đổi phải thuộc PATCH, MINOR, MAJOR, hoặc PROJECT_LOCAL.

## Governance

Repository áp dụng `SYSTEM-ENGINEERING-CHARTER-V1` từ ngày 28/07/2026 theo `PARALLEL_CHANGE`.

- Charter: `docs/governance/SYSTEM_ENGINEERING_CHARTER_V1.md`
- Adoption receipt: `docs/governance/CHARTER_ADOPTION_RECEIPT.yaml`

`AI_ENTRY.md` và `CHANGE_POLICY.md` là local profile nghiêm ngặt hơn; Hiến chương không biến repository thành hệ thống task, workflow hoặc bản thảo sống.
