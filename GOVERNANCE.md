# Governance

Repository này đã chính thức áp dụng **SYSTEM-ENGINEERING-CHARTER-V1** từ ngày 28/07/2026.

- Bản Hiến chương: `docs/governance/SYSTEM_ENGINEERING_CHARTER_V1.md`
- Biên nhận áp dụng: `docs/governance/CHARTER_ADOPTION_RECEIPT.yaml`
- SHA-256 bản chuẩn: `106448bb46edbeb73cc6600e98b346cc71f21ee40a4424b2042e581b3a1e0e19`

## Local profile

`AI_ENTRY.md` và `CHANGE_POLICY.md` vẫn là quy tắc cục bộ nghiêm ngặt hơn. Hiến chương hệ sinh thái không cho phép repository này tự biến thành hệ thống task, workflow, issue, board, report, script hoặc nơi lưu bản thảo sống.

Mọi thay đổi mới phải giữ ranh giới `core/` và `packs/<project_id>/`, xác định đúng PATCH/MINOR/MAJOR/PROJECT_LOCAL, khai báo phạm vi, test và rollback khi có ảnh hưởng liên pack.
