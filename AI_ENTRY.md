# AI Entry

Khi người dùng yêu cầu dùng editorial pack, đọc theo thứ tự:

1. `AI_ENTRY.md`
2. `packs/<project_id>/manifest.yml`
3. `packs/<project_id>/PACK.md`
4. `core/job_packet/EDITORIAL_JOB_PACKET.md`
5. `core/job_packet/ACCEPTANCE_CRITERIA.md`
6. `core/job_packet/RED_FLAGS.md`
7. prompt hoặc rule đúng task
8. sample nếu người dùng yêu cầu bắt giọng

Không tự mở thêm file nếu task không cần.

## Trước khi chạm vào bản thảo

AI phải xác định đủ:

- PROJECT
- PACK
- TASK
- SCOPE
- SOURCE LOCK
- OUTPUT
- ACCEPTANCE CRITERIA

Thiếu TASK hoặc SCOPE thì dừng và hỏi lại.

Thiếu SOURCE LOCK cho rewrite thì dừng và ghi `[CẦN DỮ LIỆU: ...]`.

## Khi thiếu quyền truy cập

Nếu không đọc được pack:

- báo rõ không đọc được pack;
- dùng bản người dùng dán nếu có;
- không có bản dán thì chỉ tư vấn chung;
- không báo đã áp dụng pack.

## Thứ tự ưu tiên

1. Yêu cầu trực tiếp trong lượt hiện tại.
2. Quyết định đã chốt trong Notion hoặc nguồn người dùng đưa.
3. Scene Packet, Canon, Handoff người dùng cung cấp.
4. Pack riêng của dự án.
5. Core dùng chung.

Không dùng trí nhớ để bù canon.

## Khi sửa thư viện

Nếu người dùng yêu cầu sửa thư viện, đọc `GOVERNANCE.md` rồi đọc `CHANGE_POLICY.md`. Mọi thay đổi phải thuộc một trong bốn loại: PATCH, MINOR, MAJOR, PROJECT_LOCAL và đồng thời tuân thủ `SYSTEM-ENGINEERING-CHARTER-V1`.

Không tự tạo file, folder, issue, workflow, board, report, script, hoặc cấu trúc quản trị, trừ khi Owner yêu cầu rõ ràng như lần phát hành Hiến chương này.
