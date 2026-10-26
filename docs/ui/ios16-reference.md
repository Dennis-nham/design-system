# Tham chiếu UI iOS 16

Tài liệu này chuyển hóa một số nguyên tắc giao diện quen thuộc của iOS 16 thành hướng dẫn độc lập cho Dennis. Đây là tham chiếu về hierarchy, surfaces và interaction; không sao chép screen, icon độc quyền, asset, tên thương hiệu hay chi tiết nhận diện của Apple.

## Ngôn ngữ thị giác

- Nền grouped neutral tạo phân lớp; nội dung đặt trên surface sáng, đường phân cách mảnh và có tương phản đủ.
- Dùng màu accent xanh cho action/link chính; success, warning và error có semantic roles riêng.
- Ưu tiên typography system-native, hierarchy gọn, body dễ đọc và label nhất quán.
- Control có kích thước ổn định, hit target thoải mái, trạng thái pressed/focus/disabled rõ ràng.
- Thanh điều hướng có thể dùng chất liệu bán trong suốt khi nội dung cuộn phía sau không làm giảm khả năng đọc; luôn có fallback opaque.
- Bo góc có cấp độ: control và row nhỏ gọn, surface lớn hơn vừa phải; tránh lạm dụng card lồng card.

## Quy đổi sang design tokens

| Nhóm | Hướng dẫn Dennis |
| --- | --- |
| Color | Dùng semantic tokens; có light/dark mappings và kiểm tra contrast |
| Typography | System font stack, scale ổn định, hỗ trợ tiếng Việt và zoom |
| Surface | Grouped background, primary surface, separator và material riêng |
| Shape | Radius theo cấp component, không tạo hình pill cho mọi control |
| Motion | Chuyển cảnh ngắn, có reduced-motion alternative |
| Icon | Dùng icon set có license rõ; icon-only control phải có accessible name |

## Áp dụng vào patterns

- **Buttons và controls:** phân cấp bằng style và vị trí; không phụ thuộc màu đơn lẻ; giữ trạng thái focus nhìn thấy.
- **Forms:** label luôn hiện, hỗ trợ autofill, helper/error text có liên kết ngữ nghĩa; không dùng placeholder làm label.
- **Navigation:** cấu trúc rõ, active item có trạng thái văn bản/semantics; trên web giữ link native và điều hướng bàn phím.
- **Calendar/date/time:** cung cấp nhập liệu trực tiếp, locale/timezone rõ và điều khiển bằng bàn phím; không giả định lịch iOS là chuẩn của mọi vùng.
- **Tooltip/toast:** nội dung ngắn, có thể tiếp cận, không che controls; lỗi quan trọng không tự biến mất quá nhanh.
- **Avatar/profile/media:** giữ crop và kích thước ổn định, fallback có ngữ nghĩa, không dùng ảnh trang trí thay thông tin cần thiết.

## Khác biệt giữa iOS và web

Không mang nguyên xi gesture-only behavior, tab bar mobile hoặc navigation stack của ứng dụng native sang web. Web cần URL có thể chia sẻ, semantics HTML, hover/focus, keyboard, responsive layout và browser history. Haptic feedback, system sheet và native picker chỉ dùng khi nền tảng hỗ trợ và luôn có phương án thay thế.

## Tiêu chí review

- [ ] Hierarchy vẫn rõ khi bỏ màu accent.
- [ ] Theme sáng/tối và contrast được kiểm tra.
- [ ] Dùng được bằng bàn phím, touch và screen reader.
- [ ] Layout hoạt động trên viewport hẹp, zoom và nội dung tiếng Việt dài.
- [ ] Không dùng asset hoặc font có quyền phân phối chưa rõ.
- [ ] Mọi hiệu ứng blur/transparency có fallback dễ đọc.