# Cover và thumbnail

## Mục đích

Hiển thị bản xem trước media có tỷ lệ khung hình và hành vi tải ổn định. Cover là vùng media lớn; thumbnail là ảnh thu nhỏ dùng trong danh sách hoặc lựa chọn.

## Hợp đồng

Nhận URL/nguồn ảnh, alt, aspect ratio, fit, kích thước responsive và fallback. Tỷ lệ được đặt trước để tránh layout shift. `object-fit: cover` chỉ dùng khi crop chấp nhận được; cung cấp cách xem đầy đủ khi nội dung có ý nghĩa.

Hỗ trợ loading, lỗi tải, nội dung không có ảnh, lazy loading phù hợp và giới hạn kích thước nguồn. Không nhúng ảnh ngoài không tin cậy mặc định; caller chịu trách nhiệm quyền sử dụng và bảo mật URL.

Kiểm thử ảnh vỡ, alt, crop, hình dọc/ngang, kích thước nhỏ và layout shift.