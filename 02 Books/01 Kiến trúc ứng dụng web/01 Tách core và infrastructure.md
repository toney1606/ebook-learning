---
type: chapter
book: "[[Kiến trúc ứng dụng web]]"
pages: 3-8
status: todo
priority: 2
chapter: 1
review_date:
apply_status: none
apply:
---
## Ý quan trọng
Mục tiêu của việc tách biệt code lõi và code hạ tầng là:
1. Không trộn lẫn giữa core code + infrastructure code, điều này sẽ giúp
	1.1. Tạo ra 1 ranh giới rõ ràng giữa tầng logic nghiệp vụ cốt lõi và phân triển khai kỹ  thuật bên ngoài
	1.2. Tách biệt giúp xây dựng một nền tảng kỹ thuật vững chắc đến phát triển hướng domain-driven (thiết kế hướng nghiệp vụ) + áp dụng Test First hay TĐ (Test-Driven Development: viết đoạn mã kiểm thử (test) trước khi viết mã tính năng thực tế.)
2. Hướng tới mã nguồn trong sáng, dễ đọc, và một kiến trúc linh hoạt sẵn sàng cho những thay đổi trong tương lai

Những vấn đề khi code lõi và code hạ tầng trộn lẫn:
1. Khó nắm bắt nghiệp vụ 
2. Phụ thuộc chặt vào công nghệ, khó thay đổi về sau
3. Khó kiểm thử tự động
4. Không bảo đảm tính nhất quán dữ liệu
5. Bảo trì khó khăn và dễ lỗi

Lợi ích của việc tách biệt core code và infrastructure code
1. Hỗ trợ phát triển hướng nghiệp vụ - hướng miền (DDD)
2. Dễ dàng phát triển theo hướng kiểm thử (TDD)

## Tóm lại
