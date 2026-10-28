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
3. Minh bạch và dễ hiểu hơn
4. Tăng khả năng tái sử dụng và linh hoạt mở rộng
5. Dễ bảo trì và nâng cấp framework
6. Chuẩn hóa kiến túc và thuận lợi cho teamwork

Giải pháp tổng quan để tách biệt core code và infrastructure code
1. Sử dụng Dependency Injection và Inversion of Control
2. Phân tầng kiến trúc rõ ràng
	Tầng domain chứa các Entity, Value Object, Domain Service
	Tầng application điều phối use case, phối hợp domain với hạ tầng
	Tầng infrastructure chứa các adapter cụ thể: repo, service send mail, control framework
	=> Domain không phụ thuộc ai, còn Application và Infrastructure phụ thuộc Domain: Layered Architecture - code core nằm ở trung tâm, hạ tầng ở rìa
3. Áp dụng các mẫu thiết kế hợp lý
	Repository Pattern: 
		Trừu tượng hóa truy xuất và lưu trữ dữ liệu domain
		Ngăn cách giữa domain và DB
	Domain Model
		Tập trung logic nghiệp vụ vào object Domain
	Dependency Injection
		Cấu hình các phụ thuộc
	Factory Pattern
		Tạo ra đối tượng thay vì gọi trực tiếp hàm của Thư viện bên ngoài
			VD: Dùng Clock Interface thay vì gọi new DateTime() trong core code
	
## Tóm lại
