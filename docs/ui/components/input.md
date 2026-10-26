# Input và text fields

## Cấu trúc

Text field gồm label hiển thị, control, mô tả tùy chọn và thông báo lỗi gắn với control. Placeholder không thay thế label. Hỗ trợ `id`, `name`, `type`, `value/defaultValue`, `disabled`, `readOnly`, `required`, `aria-describedby` và error state theo quy ước framework đã chọn.

## Hành vi

- Không xóa nội dung người dùng khi validation thất bại.
- Lỗi chỉ xuất hiện theo thời điểm hợp lý; văn bản nêu cách sửa, không chỉ đổi viền đỏ.
- Hỗ trợ autocomplete, input mode và autofill native khi phù hợp.
- Textarea và input số/ngày cần API chuyên biệt nếu native semantics khác nhau.
- Kích thước target, focus ring và trạng thái disabled/read-only nhất quán.

## Kiểm thử

Label click/focus, required, help/error association, keyboard, autofill, giá trị dài, RTL và trình đọc màn hình.