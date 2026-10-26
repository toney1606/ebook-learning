# ebook-learning

Vault Obsidian ghi chú khi đọc ebook chuyên ngành (từ 2026).

## Cấu trúc
Số đầu tên folder/file = thứ tự nên mở/đọc.

| Folder | Dùng cho |
|---|---|
| `01 Dashboards/` | Trang tự lọc: Sách cần đọc, Chương đọc tiếp, Cần ôn, Theo chủ đề, Theo năm, Cần áp dụng |
| `02 Books/` | Mỗi cuốn một folder `NN Tên sách` (NN = thứ tự ưu tiên đọc sách) |
| `03 Notes/` | Ý/khái niệm dùng lại nhiều nơi |
| `04 Inbox/` | Note mới tạo mặc định rơi vào đây, xử lý xong chuyển đi |
| `05 Templates/` | `Book`, `Chapter`, `Note` (Ctrl+P → Insert template) |
| `06 Attachments/` | Ảnh dán vào note |

Trong folder sách: note tổng quan `Tên sách.md`, các chương `NN Tên chương.md` (NN = thứ tự nên đọc, không phải số chương trong sách; số chương sách ghi ở thuộc tính `chapter`), `Files/` chứa PDF/epub.

## Quy ước
- Đổi thứ tự đọc = đổi số đầu tên (đổi tên trong Obsidian thì link tự cập nhật).
- Chủ đề, năm, trạng thái nằm ở metadata của note tổng quan, không chia folder.
- Mỗi chương chỉ ghi **Ý quan trọng** (kèm số trang) và **Tóm lại** (1–2 câu).
- Ưu tiên: `priority` 1 (cao) · 2 (vừa) · 3 (thấp).
- Ôn tập: điền `review_date`. Cần áp dụng: `apply_status: todo` + `apply`.
- Link trang PDF: `[[Tên sách.pdf#page=12]]`.

## PDF/epub
Không đưa vào git (`.gitignore`). Máy khác tự chép file vào `Files/` của sách tương ứng.

## Đồng bộ giữa các máy
Plugin **Obsidian Git**: auto pull khi mở vault, auto commit + push mỗi 5–10 phút.
