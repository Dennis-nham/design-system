# Yêu cầu accessibility

## Tiêu chí mặc định

- Ưu tiên phần tử HTML native và semantics đúng; ARIA chỉ bổ sung khi native không đủ.
- Tất cả hành động dùng được bằng bàn phím; focus nhìn thấy rõ, thứ tự focus hợp lý và không có trap ngoài dialog/modal.
- Label, description, lỗi và trạng thái được liên kết programmatically.
- Không truyền đạt trạng thái chỉ bằng màu; hỗ trợ zoom, reflow, reduced motion và nội dung dài.
- Component tương tác có kiểm tra screen reader phù hợp và kiểm tra tương phản theo tiêu chuẩn đã chọn.

## Kiểm tra

Mỗi component ghi keyboard map, accessible name/state và phương án khi nội dung không tải. Tự động hóa chỉ là một lớp; review thủ công vẫn cần thiết. Chốt mục tiêu WCAG và phiên bản tiêu chuẩn trước khi tuyên bố tuân thủ.