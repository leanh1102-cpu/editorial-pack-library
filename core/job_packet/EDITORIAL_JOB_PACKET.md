# Editorial Job Packet

File này định nghĩa tối thiểu cần có trước khi AI chạm vào bản thảo.

AI chỉ xử lý bản thảo khi người dùng cung cấp đủ:

1. PROJECT
2. PACK
3. TASK
4. SCOPE
5. SOURCE LOCK
6. OUTPUT
7. ACCEPTANCE CRITERIA

## PROJECT

Tên dự án hoặc pack cần dùng.

Ví dụ: `Sương Lạc Tiên Đạo`.

## PACK

Đường dẫn pack.

Ví dụ: `editorial-pack-library/packs/sltd`.

Nếu không đọc được pack, AI phải báo `PACK NOT ACCESSIBLE`.

## TASK

Một việc cụ thể:

- audit_scene
- line_edit
- rewrite_scene
- flow_pass
- seam_pass

Không tự đổi task.

## SCOPE

Đoạn, scene, chương, hoặc vùng văn bản cần xử lý.

Thiếu scope thì dừng và hỏi lại.

## SOURCE LOCK

Nguồn khóa được phép dùng:

- Canon In
- Canon Out
- Scene Packet
- Handoff
- Quyết định đã chốt
- Không được dùng

Nếu rewrite mà thiếu Source Lock, dừng và ghi `[CẦN DỮ LIỆU: ...]`.

## OUTPUT

Người dùng phải nêu đầu ra mong muốn:

- chỉ audit
- chỉ bản sửa
- bản sửa kèm lỗi chính
- score kèm nhãn pass/fail

Không tự thêm report dài nếu không được yêu cầu.

## ACCEPTANCE CRITERIA

Dùng `core/job_packet/ACCEPTANCE_CRITERIA.md` và `core/job_packet/RED_FLAGS.md`.
