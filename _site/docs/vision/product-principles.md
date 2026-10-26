# Nguyên tắc sản phẩm

1. **Có nhu cầu trước khi có component:** ghi nhận người dùng và vấn đề trước khi mở rộng thư viện.
2. **Nền tảng trung lập:** không nhúng tên sản phẩm, nội dung nghiệp vụ hay thương hiệu của một khách hàng vào core.
3. **Dùng được trước, tùy biến sau:** trạng thái mặc định phải hữu ích; customization không phá accessibility.
4. **API ổn định có chủ đích:** mọi public export được xem là hợp đồng; deprecation có lộ trình.
5. **Hiển thị rõ trạng thái:** loading, empty, error, disabled và success phải được xem xét phù hợp với từng pattern.
6. **Tối ưu cho người dùng thật:** kiểm thử với bàn phím, màn hình nhỏ, nội dung dài và ngôn ngữ khác.
7. **Đo adoption có trách nhiệm:** chỉ thu thập số liệu cần thiết, minh bạch và không gửi dữ liệu sử dụng mặc định nếu chưa có consent.