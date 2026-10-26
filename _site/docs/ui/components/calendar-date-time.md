# Calendar, date picker và time picker

## Phạm vi

Phân biệt ngày dân sự, thời điểm tuyệt đối và giờ địa phương. API không được tự chuyển timezone ngầm. Giá trị lưu trữ, locale, calendar system, timezone và quy tắc tuần đầu tiên phải được xác định rõ.

## Date picker / calendar

- Có thể nhập ngày trực tiếp; picker là phương thức bổ sung chứ không phải lối duy nhất.
- Dùng lưới ngày có tên ngày/tháng truy cập được, điều hướng bằng bàn phím và công bố ngày đang chọn.
- Hỗ trợ min/max, ngày không khả dụng, locale và lựa chọn khoảng ngày nếu use case yêu cầu.
- Khi mở, focus có điểm đến hợp lý; đóng bằng Escape; focus quay về trigger.

## Time picker

Chốt 12/24 giờ theo locale, step phút, nhập bàn phím, giá trị không hợp lệ và xử lý ngày chuyển giờ daylight-saving. Không đoán timezone hệ thống thay cho caller.

## Điều kiện phát hành

Chọn thư viện date/time chuyên dụng đã được duy trì hoặc chứng minh đầy đủ tính đúng đắn trước khi tự triển khai logic lịch. Test locale, năm nhuận, DST, biên min/max và bàn phím.