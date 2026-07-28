# SYSTEM-ENGINEERING-CHARTER-V1

**Phiên bản:** 1.0.0  
**Trạng thái:** RATIFIED — ACTIVE  
**Ngày hiệu lực:** 2026-07-28  
**Phê duyệt:** OWNER_APPROVED  
**SHA-256 bản Markdown chuẩn:** `106448bb46edbeb73cc6600e98b346cc71f21ee40a4424b2042e581b3a1e0e19`

## Phạm vi

Áp dụng cho toàn bộ dự án hiện có và về sau, bao gồm công cụ sáng tác/biên tập, thư viện rule/prompt/sample và các hệ thống PAI hỗ trợ Writing.

- Dự án hiện có áp dụng theo `PARALLEL_CHANGE`.
- Dự án mới phải khai báo tuân thủ trước commit nội dung hoặc mã đầu tiên.
- Quy tắc cục bộ nghiêm ngặt hơn tiếp tục có hiệu lực.

> Một thay đổi chỉ được phép tác động đến phạm vi đã khai báo. Mọi tác động ngoài phạm vi phải bị phát hiện trước merge hoặc trước phát hành.

## Quy tắc áp dụng cho thư viện biên tập

1. `core/` và `packs/<project_id>/` là bounded context riêng; pack dự án không sửa core để chữa lỗi cục bộ.
2. Mỗi thay đổi phải xác định rõ PATCH, MINOR, MAJOR hoặc PROJECT_LOCAL theo `CHANGE_POLICY.md`.
3. Một thay đổi chỉ chạm đúng file và pack đã khai báo; không mở rộng canon, workflow hoặc cấu trúc quản trị.
4. File bị thay thế phải deprecate trước khi xóa; không xóa trong cùng major version.
5. Không dùng trí nhớ để bù canon; thiếu source lock phải dừng.
6. Không tuyên bố đã áp dụng pack nếu chưa đọc được pack và manifest.
7. Mọi thay đổi có thể ảnh hưởng nhiều pack phải có Change Contract, regression trên pack liên quan và rollback.
8. Không đưa dữ liệu BVNT, dữ liệu cá nhân hoặc secret vào thư viện.
9. Không mở issue, workflow, board, report hoặc script trái với ranh giới đã khóa của repository.
10. Không tạo node/release mới để né blocker hoặc thay đổi chưa hoàn tất.

## Local profile nghiêm ngặt hơn

`AI_ENTRY.md` và `CHANGE_POLICY.md` tiếp tục là authority cục bộ về thứ tự đọc, phạm vi sử dụng và phân loại thay đổi. Khi có khác biệt với Hiến chương hệ sinh thái, áp dụng quy tắc nghiêm ngặt hơn. Hiến chương này không biến repository thành hệ thống quản lý task, workflow hoặc bản thảo sống.

## Thứ bậc

Hiến chương hệ sinh thái chi phối kỹ thuật, phạm vi thay đổi, versioning, deprecation, bằng chứng và rollback. Pack/manifest/canon của từng dự án tiếp tục chi phối nội dung sáng tác và biên tập.
