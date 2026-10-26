# Tooltip và toast

## Tooltip

Tooltip bổ sung thông tin ngắn, không chứa nội dung thiết yếu hoặc controls tương tác. Kích hoạt bằng hover và focus; có thể đóng theo thiết kế bằng Escape; không che trigger và cần đủ thời gian để đọc. Icon-only control phải có accessible name độc lập.

## Toast

Toast thông báo kết quả không chặn luồng. Phân loại thông tin, thành công, cảnh báo và lỗi; nội dung ngắn, hành động tùy chọn. Dùng live region phù hợp, không thông báo dồn dập và cho phép người dùng đóng.

Thông báo quan trọng cần tồn tại đủ lâu hoặc không tự biến mất; lỗi cần có nơi bền vững trong trang. Không chỉ dùng màu/icon để truyền đạt mức độ.

Kiểm thử screen reader, nhiều toast, thứ tự mới nhất, pause/timeout khi focus và viewport nhỏ.