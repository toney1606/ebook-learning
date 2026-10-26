# ebook-learning

Vault Obsidian ghi chú khi đọc ebook chuyên ngành (từ 2026).

## Cấu trúc
| Folder              | Dùng cho                                                                                                   |
| ------------------- | ---------------------------------------------------------------------------------------------------------- |
| `Inbox/`            | Note mới tạo mặc định rơi vào đây, xử lý xong chuyển đi                                                    |
| `Books/<Tên sách>/` | Mỗi cuốn một folder: note tổng quan (trùng tên folder), mỗi chương một note `01 …`, `Files/` chứa PDF/epub |
| `Notes/`            | Ý/khái niệm dùng lại nhiều nơi                                                                             |
| `Dashboards/`       | Trang tự lọc: Sách cần đọc, Chương đọc tiếp, Cần ôn, Theo chủ đề, Theo năm, Cần áp dụng                                         |
| `Templates/`        | `Book`, `Chapter`, `Note` (Ctrl+P → Insert template)                                                       |
| `Attachments/`      | Ảnh dán vào note                                                                                           |

## Quy ước
- Chương: `NN Tên chương`. Chủ đề, năm, trạng thái nằm ở metadata của note tổng quan, không chia folder.
- Mỗi chương chỉ ghi **Ý quan trọng** (kèm số trang) và **Tóm lại** (1–2 câu).
- Ưu tiên: `priority` 1 (cao) · 2 (vừa) · 3 (thấp). Thứ tự đọc trong một cuốn: `order` 1, 2, 3…
- Ôn tập: điền `review_date`. Cần áp dụng: `apply_status: todo` + `apply`.
- Link trang PDF: `[[Tên sách.pdf#page=12]]`.

## PDF/epub
Không đưa vào git (`.gitignore`). Máy khác tự chép file vào `Files/` của sách tương ứng.

## Đồng bộ giữa các máy
Plugin **Obsidian Git**: auto pull khi mở vault, auto commit + push mỗi 5–10 phút.
