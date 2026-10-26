---
type: book
title: "Kiến trúc ứng dụng web"
author: Huy (Technical Leader)
tags: [book, architecture, hexagonal, ddd]
status: reading
started: 2026-10-26
finished:
rating:
---

# Kiến trúc ứng dụng web

> [!abstract] Một câu tóm tắt
> Tách code nghiệp vụ (core) khỏi code hạ tầng (infrastructure), tiến tới Hexagonal Architecture (Ports & Adapters). Ví dụ minh họa bằng PHP/Laravel, 60 trang.

## Vì sao đọc
- Hiểu nền tảng của kiến trúc hexagonal/clean đang dùng trong walo-erp (handler → service → domain → repository).

## Mục lục & tiến độ
- [ ] Mục tiêu & tầm quan trọng của việc tách core / infrastructure (vấn đề khi trộn lẫn, lợi ích, giải pháp tổng quan)
- [ ] Ví dụ minh họa: core code là gì, infrastructure code là gì, ranh giới thực tế
- [ ] Domain Model (Entity vs Value Object)
- [ ] Repository Pattern (định nghĩa, interface, triển khai ở tầng hạ tầng)
- [ ] Sử dụng Domain Model + Repository trong luồng nghiệp vụ
- [ ] Read Models và View Models
- [ ] Tách logic use case khỏi Controller (Command/DTO, Application Service)
- [ ] Ports and Adapters (Hexagon Architecture): Port, Adapter, vận dụng vào kiến trúc phân lớp

## Ý đáng nhớ
- (tr. ) 

## Trích dẫn hay
> 

## Thuật ngữ
| Thuật ngữ | Nghĩa ngắn gọn |
|---|---|
| Core code | Logic nghiệp vụ thuần, không biết DB/framework |
| Infrastructure code | Code nối core với DB, API ngoài, file, framework |
| Port | Cổng giao tiếp trừu tượng (interface) mà core định nghĩa |
| Adapter | Bản cài đặt cụ thể của port (SQL, email, log...) |

## Ví dụ / code đáng giữ
```

```

## Liên hệ với công việc (walo-erp)
- 

## Câu hỏi còn thắc mắc
- [ ] 

## Việc sẽ làm sau khi đọc
- [ ] 

## Ghi chú liên quan
- [[ ]]
