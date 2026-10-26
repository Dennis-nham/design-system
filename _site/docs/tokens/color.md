# Color tokens

## Nguyên tắc

- Dùng vai trò semantic: `text.primary`, `text.muted`, `surface.canvas`, `surface.raised`, `border.default`, `action.primary`, `status.error`.
- Tách trạng thái interactive (hover, active, focus, disabled) khỏi màu thương hiệu.
- Light/dark theme ánh xạ semantic token sang giá trị cụ thể; không để component tự định nghĩa palette riêng.
- Trạng thái không chỉ dựa vào màu; kiểm tra contrast theo tiêu chuẩn accessibility đã chọn.

## Bộ màu tham chiếu ban đầu

Các giá trị dưới đây gợi tinh thần màu hệ thống iOS 16, chỉ là điểm xuất phát độc lập cho theme NPMIS, không phải bảng màu chính thức của Apple. Hãy kiểm tra contrast và điều chỉnh theo brand trước khi ổn định token.

| Token semantic | Giá trị tham chiếu | Dùng cho |
| --- | --- | --- |
| `color.action.primary` | `#007AFF` | Hành động và liên kết chính |
| `color.status.success` | `#248A3D` | Trạng thái thành công |
| `color.status.warning` | `#9A6700` | Cảnh báo cần chú ý |
| `color.status.error` | `#D70015` | Lỗi và hành động nguy hiểm |
| `color.surface.grouped` | `#F2F2F7` | Nền khu vực nhóm nội dung |
| `color.surface.primary` | `#FFFFFF` | Bề mặt nội dung |
| `color.text.primary` | `#1C1C1E` | Văn bản chính |
| `color.text.secondary` | `#636366` | Văn bản phụ |

Dark theme phải ánh xạ lại semantic tokens theo nền tối; không đảo màu cơ học. Cần kiểm chứng mọi cặp foreground/background, including trạng thái disabled và focus.

## Mở rộng

Hỗ trợ theme qua CSS custom properties và cơ chế override theo phạm vi. Tránh đặt tên token gắn với màu sắc thị giác khi màu có thể đổi theo brand. Chưa chốt palette thương hiệu; mọi màu minh họa cần được đánh dấu là provisional.