# Đóng gói và phát hành npm/GitHub

## Trước khi công bố

- Chốt license, package scope, quyền publish và danh sách maintainer.
- Kiểm tra build output, `exports`, typings, CSS, files được đóng gói và peer dependencies.
- Chạy test trên artifact đóng gói trong consumer fixture; không chỉ test workspace source.
- Tạo changelog, tag tương ứng và ghi rõ breaking changes.
- Dùng GitHub Actions với quyền tối thiểu, bảo vệ branch và môi trường publish có approval phù hợp.

## Quy trình phát hành dự kiến

Pull request được kiểm tra tự động; maintainer review; merge vào nhánh chính; tạo release/tag; CI build và kiểm thử; publish bằng trusted publishing/provenance nếu registry và cấu hình hỗ trợ; xác minh package trên npm sau publish.

Không lưu npm token dài hạn trong repo. Bật 2FA và quản lý quyền publish theo tổ chức. Pin action theo SHA khi yêu cầu bảo mật của dự án đã được chốt.

## Phiên bản

Trước v1, có thể dùng prerelease (`0.x` hoặc tag `next`) để nhận phản hồi, nhưng phải công bố mức ổn định. Không tự động phát hành từ mọi commit nếu chưa có quy trình rollback và người chịu trách nhiệm.