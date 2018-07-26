## Đề số 006

Các hệ thống của Gobiz rất thường xuyên sử dụng các notification bằng email hay SMS. Trong các thông tin này sẽ có các đường link truy cập để khách hàng/người dùng có thể nhanh chóng truy cập đến thông tin cần thiết.

Tuy nhiên, đường link sẽ khá dài trong khi nội dung SMS, Gobiz không muốn dài - vừa đảm bảo tính ngắn gọn vừa tiết kiệm chi phí vì SMS sẽ bị tính số ký tự.

Vì vậy, Gobiz quyết định sẽ mở một URL Shorten service để tự làm ngắn các đường link dài, vừa khắc phục được vấn đề về chi phí, vừa chủ động trong việc cung cấp link này.

Dịch vụ này cần phải có thể:
- Có khả năng từ url -> short url qua API hoặc qua UI
- Có thể tự đặt shorturl cho một url nào đó, chỉ cần unique (qua API hoặc UI)
- Có thể thống kê số lượt truy cập trên từng url, tốt hơn là thống kê được theo cả trình duyệt, hệ điều hành,...
- Từ một url, nếu đã có short version tương ứng thì trả về short url đó luôn chứ không tạo thêm một short url khác, trừ phi custom url
- Không được dùng các lib shorten có sẵn