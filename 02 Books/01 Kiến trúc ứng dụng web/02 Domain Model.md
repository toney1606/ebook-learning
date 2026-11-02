---
type: chapter
book: "[[Kiến trúc ứng dụng web]]"
pages: 16-21
status: todo
priority: 1
chapter: 3
review_date: 
apply_status: none
apply: 
---

## Ý quan trọng
I. Khái niệm
	- Là một tập hợp các khái niệm, đối tượng, quy tắc nghiệp vụ được mô hình hóa dưới dạng code, phản ánh sát nhất thực thể và quy trình trong thế giới thực và quy trình thế giới thực của bài toán mà phần mềm giải quyết.
	- Thường liên quan đến Entity, Value Object, Domain Service,... tuân theo tư tưởng Domain-Driven Design

II. Tác dụng
	- Thể hiện rõ các khái niệm domain
	- Đảm bảo tính nhất quán và đầy đủ của dữ liệu domain
	- Đóng gói logic liên quan vào đúng chỗ
	- Tách bạch hẳn domain logic khỏi các chi tiết kỹ thuật

III. Thiết kế một DE (Domain Entity)
1. Khái niệm
	- Entity là loại đối tượng có đặc điểm tồn tại lâu dài (có định danh duy nhất, VD: OrderID, để phân biệt các instance) và tương ứng với 1 thực thể thật (đơn hàng thật, người dùng thật, sản phẩm thật,....)
2. Cách tiếp cận
	- Cung cấp đầy đủ các dữ liệu bắt buộc tại thời điểm tạo đối tượng
3. Entity vs Value Object
	- Entity:
		- Có danh tính riêng để phân biệt
		- Thường thay đổi trạng thái theo thời gian
	- Value Object:
		- Không có danh tính riêng
		- Đại diện cho 1 giá trị và thường bất biến
	- 

















## Tóm lại
