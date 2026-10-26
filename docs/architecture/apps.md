# Ứng dụng trong hệ sinh thái

## Ứng dụng tài liệu

Cho phép tìm kiếm component, xem variants và đọc ví dụ. Mỗi ví dụ cần cho biết trạng thái, keyboard behavior, props liên quan và giới hạn. Có thể cung cấp theme switcher để kiểm tra tokens; không gửi telemetry mặc định.

## Ứng dụng playground

Chỉ xây khi có nhu cầu thử props và chia sẻ ví dụ. Không chạy code người dùng trên server hoặc thực thi nội dung không tin cậy nếu chưa có sandbox và mô hình bảo mật.

## CLI và dịch vụ

CLI generator, cloud, marketplace và đồng bộ design-tool là hướng tương lai, không phải dependency của core UI. Mỗi app/dịch vụ cần owner, threat model, chính sách dữ liệu và kế hoạch vận hành riêng trước khi khởi động.