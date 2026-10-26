# ebook-learning

Vault Obsidian ghi chú khi đọc ebook chuyên ngành (từ 2026).

## Cấu trúc
| Folder | Dùng cho |
|---|---|
| `00-INBOX/` | Note mới tạo mặc định rơi vào đây; xử lý rồi chuyển đi |
| `10-BOOKS/<Tên sách>/` | 1 folder = 1 cuốn: note tổng quan (trùng tên folder), `KTW-01 …` mỗi chương 1 note, `source/` chứa PDF/epub |
| `20-NOTES/` | Ý/khái niệm dùng lại nhiều nơi (chỉ tách khi dùng được ngay hoặc thấy ở ≥2 chỗ) |
| `30-MAPS/` | Trang tự lọc (`.base`): Đang đọc, Cần ôn, Theo chủ đề, Theo năm, Việc cần áp dụng |
| `90-TEMPLATES/` | `Book`, `Chapter`, `Note` (Ctrl+P → Insert template) |
| `99-ATTACHMENTS/` | Ảnh dán vào note |

## Quy ước
- Tên chương: `<mã sách>-NN Tên chương` (graph chỉ hiện tên file, mã sách tránh trùng tên).
- Chủ đề, năm, trạng thái nằm ở **metadata** của note tổng quan, không chia folder.
- Mỗi chương 3 tầng: ghi nhanh → tóm tắt bằng lời mình → 1–3 ý tách sang `20-NOTES`.
- Ôn tập: đặt `review_date` = ngày đọc +3 ngày, +2 tuần, +2 tháng; xem `30-MAPS/Can-on`.
- Cần áp dụng vào việc thật: đặt `apply_status: todo` + ghi `apply:`.
- Link trang PDF: `[[Tên sách.pdf#page=12]]`.

## PDF/epub
Không đưa vào git (`.gitignore`). Máy khác tự chép file vào `source/` của sách tương ứng.

## Đồng bộ giữa các máy
Plugin **Obsidian Git**: auto pull khi mở vault, auto commit + push mỗi 5–10 phút.
