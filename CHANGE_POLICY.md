# Change Policy

File này khóa cách sửa thư viện. Nó không tạo luồng làm việc, không tạo task, không mở workflow.

## 1. Loại thay đổi

Mọi chỉnh sửa phải thuộc một trong bốn loại:

### PATCH

Sửa lỗi chữ, làm rõ câu, chỉnh format. Không đổi hành vi AI.

### MINOR

Thêm rule, prompt, sample, manifest, pack note. Không phá file cũ. Không đổi thứ tự ưu tiên.

### MAJOR

Đổi cấu trúc pack, đổi thứ tự AI đọc, đổi rubric, hoặc đổi luật ưu tiên. Phải tăng version lớn.

### PROJECT_LOCAL

Chỉ áp vào một pack riêng, ví dụ `packs/sltd/`. Không đưa vào `core/`.

## 2. Luật core

- Không đưa canon, motif, giọng nhân vật, lore riêng vào `core/`.
- Lỗi chỉ thuộc một dự án phải sửa trong pack riêng.
- Lỗi thuộc văn xuôi tiếng Việt nói chung mới đưa vào `core/`.
- Chưa chắc thuộc loại nào thì để trong pack riêng trước.

## 3. Luật pack riêng

- Pack riêng có thể thêm rule riêng.
- Pack riêng không sửa pack khác.
- Pack riêng không sửa `core/` để chữa lỗi cục bộ.

## 4. Luật xóa file

Không xóa file trong cùng major version. Muốn bỏ file, đánh dấu `deprecated` trong manifest và ghi file thay thế. Chỉ xóa ở major version sau.

## 5. Luật AI khi sửa thư viện

AI phải:

1. Đọc `AI_ENTRY.md`.
2. Đọc `CHANGE_POLICY.md`.
3. Xác định loại thay đổi.
4. Chỉ sửa file nằm trong phạm vi người dùng nêu.
5. Không tạo workflow, issue, board, report, script, hay cấu trúc quản trị.

Nếu thay đổi không khớp bốn loại trên, dừng và hỏi người dùng.
