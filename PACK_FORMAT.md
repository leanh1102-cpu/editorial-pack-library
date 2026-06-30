# Pack Format

Mỗi pack phải có:

```text
packs/<project_id>/
  manifest.yml
  PACK.md
  rules/
  prompts/
  samples/
```

## `manifest.yml`

Nêu rõ id gói, phiên bản, phạm vi cho phép, phạm vi cấm, file cần đọc.

## `PACK.md`

Nêu vai trò của gói, ranh giới, thứ tự ưu tiên, luật dừng.

## `rules/`

Chỉ ghi luật biên tập đã chốt. Không ghi task, trạng thái, tranh luận chưa chốt.

## `prompts/`

Chỉ ghi prompt dùng lại. Prompt phải nêu dữ liệu đầu vào, đầu ra, điều kiện dừng.

## `samples/`

Chỉ giữ mẫu ngắn. Mẫu không thay canon.

## Core job packet

`core/job_packet/` giữ ba file dùng chung trước khi xử lý bản thảo:

- `EDITORIAL_JOB_PACKET.md`
- `ACCEPTANCE_CRITERIA.md`
- `RED_FLAGS.md`

Các file này không tạo task, không tạo report, không tự động hóa. Chúng chỉ khóa cách giao bài và cách xác định pass/fail.

## Version

- `1.0.0`: bản ổn định đầu tiên.
- `1.0.x`: sửa chữ, làm rõ câu, không đổi hành vi.
- `1.x.0`: thêm rule hoặc prompt mới, không phá file cũ.
- `2.0.0`: đổi cấu trúc hoặc thứ tự ưu tiên.
