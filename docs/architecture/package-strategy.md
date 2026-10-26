# Chiến lược packages

## Cấu trúc gợi ý

- `@dennis-nham/tokens`: token nguồn, CSS variables và định dạng build (tên minh họa).
- `@dennis-nham/ui`: component web và styles (tên minh họa, cần kiểm tra namespace npm).
- `@dennis-nham/icons`: chỉ tách khi nguồn icon, license và nhu cầu tree-shaking đã rõ (tên minh họa).
- `@dennis-nham/docs`: ứng dụng tài liệu; không nhất thiết phát hành lên npm (tên minh họa).

Bắt đầu bằng ít package nhất có thể. Nếu một package UI và tokens đủ, không tách package để tạo cấu trúc hình thức.

## Hợp đồng package

- Chỉ public API trong entry point được công bố; giữ internal paths riêng.
- Khai báo rõ `exports`, `types`, module format, CSS entry và peer dependencies.
- Không yêu cầu người dùng cài dependency build-time không cần thiết.
- Kiểm thử package đã đóng gói bằng consumer fixture trước publish.
- License dự án là MIT; đặt tên scope npm sau khi xác nhận quyền sở hữu và tránh xung đột tên.

## Chính sách tương thích

SemVer chỉ áp dụng khi API công khai được định nghĩa. Deprecation cần thông báo, thay thế, thời hạn tối thiểu và hướng dẫn migration.