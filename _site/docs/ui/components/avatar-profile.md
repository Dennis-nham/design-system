# Avatar và profile

## Avatar

Avatar hiển thị ảnh hoặc fallback chữ cái/biểu tượng. API dự kiến gồm `src`, `alt`, `name`, `size`, `shape` và trạng thái hiện diện tùy chọn. Ảnh người dùng có alt theo ngữ cảnh; ảnh trang trí dùng alt rỗng. Không hiển thị presence chỉ bằng màu.

Ảnh lỗi/chưa tải phải giữ kích thước ổn định và chuyển sang fallback. Không tự cắt nội dung quan trọng; hỗ trợ high-density image và tên dài.

## Profile summary

Là molecule kết hợp avatar và thông tin tên/phụ đề; không hàm ý dữ liệu cá nhân hay quyền truy cập. Nếu tương tác điều hướng, dùng link có tên dễ hiểu; nếu mở menu, dùng button và công bố trạng thái.

Kiểm thử fallback, alt, loading/error, tên dài, kích thước nhỏ và tương phản.