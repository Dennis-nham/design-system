# Button

## Mục đích và API

Dùng cho hành động rõ ràng. Mặc định là button HTML; điều hướng dùng link. Các thuộc tính dự kiến: `variant` (primary, secondary, outline, ghost, danger), `size`, `disabled`, `loading`, `type` và nội dung/icon.

## Hành vi

- Chỉ một primary action nổi bật trong cùng nhóm khi phân cấp thị giác cần thiết.
- Loading không được làm nút đổi kích thước; thông báo trạng thái cho công nghệ hỗ trợ và ngăn submit lặp.
- Icon-only cần accessible name và tooltip nếu ý nghĩa chưa phổ biến.
- Disabled phải thể hiện rõ; với hành động cần giải thích lý do, cân nhắc giữ tương tác và mô tả yêu cầu thay vì chỉ disable.
- Focus bằng bàn phím hiển thị; Enter/Space kích hoạt theo hành vi native.

## Kiểm thử

Kiểm tra variant, loading, disabled, type submit/reset, icon-only, label dài và contrast ở mọi theme.