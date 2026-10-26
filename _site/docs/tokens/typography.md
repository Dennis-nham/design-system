# Typography tokens

Định nghĩa roles như `font.family.body`, `font.family.heading`, `font.size.body`, `font.size.label`, `font.size.heading.*`, `font.weight.*` và `line.height.*`. Các giá trị cuối cần được kiểm thử với tiếng Việt có dấu, nội dung dài và font fallback.

## Tham chiếu giao diện

Ưu tiên kiểu chữ system-native để giao diện hòa nhập môi trường mà không đóng gói font độc quyền: `-apple-system`, `BlinkMacSystemFont`, `"Segoe UI"`, sans-serif. Dùng scale phân cấp rõ ràng, tiêu đề đậm vừa phải, body thoáng và label ngắn; không dùng chữ siêu nhỏ để nhồi thông tin. Đây là lựa chọn tương thích đa nền tảng, không phải yêu cầu dùng font Apple.

Font bên thứ ba phải có license phù hợp, nguồn và phương án fallback. Không dùng kích thước phụ thuộc viewport cho mọi cấp chữ; ưu tiên scale có chủ đích và giới hạn reflow. Chốt font family sau khi kiểm tra tải, coverage glyph, hiệu năng và quyền phân phối.