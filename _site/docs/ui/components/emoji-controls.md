# Emoji và controls cơ bản

## Emoji

Emoji picker là tiện ích tùy chọn, không nên là dependency bắt buộc của input văn bản. Cần xác định bộ dữ liệu, license, Unicode version, skin tone, tìm kiếm, nhóm, bàn phím và cách biểu diễn emoji sequence. Không giả định hình glyph giống nhau giữa hệ điều hành.

## Checkbox, radio và switch

- Checkbox biểu diễn lựa chọn độc lập; hỗ trợ checked, unchecked và indeterminate khi hợp lý.
- Radio chọn đúng một giá trị trong nhóm; có legend/label và điều hướng nhóm nhất quán.
- Switch biểu diễn bật/tắt tức thời; tên accessible phải nêu setting, không dùng switch thay checkbox trong form nhiều lựa chọn.
- Ưu tiên native input hoặc đảm bảo semantics, focus và keyboard tương đương.

Kiểm thử trạng thái, nhãn dài, touch target, form submission, disabled và công nghệ hỗ trợ.