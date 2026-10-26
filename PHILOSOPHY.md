# Triết lý thiết kế

- **Rõ ràng trước tiện lợi:** API dễ đọc, hành vi có thể dự đoán.
- **Composable:** component nhỏ phối hợp được, không khóa người dùng vào một mẫu trang.
- **Accessible by default:** ngữ nghĩa HTML, bàn phím, focus và tương phản được tính từ đầu.
- **Tùy biến có giới hạn:** tokens là điểm điều chỉnh chính; tránh vô số biến thể không thể bảo trì.
- **Framework-aware, không framework-bound:** lõi giao ước và tokens không phụ thuộc giao diện của một ứng dụng cụ thể.
- **Tài liệu đi cùng mã:** ví dụ, trạng thái lỗi và giới hạn được ghi rõ.
- **Không giả định:** quyết định chưa được xác nhận phải có chủ sở hữu và trạng thái.