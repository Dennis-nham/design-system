# NPMIS Design System

NPMIS là dự án hướng tới một design system và UI kit dùng chung, có thể phân phối qua npm, tích hợp vào ứng dụng web và phát triển cùng cộng đồng. Bộ tài liệu này mô tả mục tiêu, ranh giới kỹ thuật, hành vi giao diện và cách đóng góp; tài liệu không thay thế mã nguồn triển khai hay tư vấn pháp lý.

## Bắt đầu

- Website tài liệu: [Dennis-nham.github.io/design-system](https://dennis-nham.github.io/design-system/).
- Định hướng: [Tầm nhìn](VISION.md), [Sứ mệnh](MISSION.md), [Mục tiêu](GOALS.md).
- Phạm vi sản phẩm: [Phạm vi nền tảng](docs/product/platform-scope.md), [Nguyên tắc sản phẩm](docs/vision/product-principles.md).
- Kỹ thuật: [Tổng quan kiến trúc](docs/architecture/system-overview.md), [Chiến lược packages](docs/architecture/package-strategy.md), [Ứng dụng](docs/architecture/apps.md), [Phát hành npm](docs/architecture/publishing.md).
- UI: [Atomic Design](docs/ui/atomic-design.md), [Danh mục thành phần](docs/ui/components/README.md), [Tokens](docs/tokens/README.md), [Accessibility](docs/ui/accessibility.md).
- Cộng đồng và quản trị: [Đóng góp](CONTRIBUTING.md), [RFC](docs/governance/rfc.md), [Báo lỗi](docs/community/bug-report.md), [Yêu cầu tính năng](docs/community/feature-request.md).
- Tác giả và quyền: [Tác giả](AUTHOR.md), [Bản quyền](COPYRIGHT.md), [Giấy phép](LICENSE.md).

## Trạng thái

Đây là nền móng tài liệu ban đầu, chưa phải cam kết API ổn định hay chứng nhận tương thích. Các mục chưa được xác nhận được ghi rõ là quyết định cần đưa ra. Xem [lộ trình](docs/roadmap/v1.md) và [backlog](docs/roadmap/backlog.md) để theo dõi bước tiếp theo.

## Cấu trúc

```text
docs/
	architecture/  system-overview, packages, apps, publishing
	community/     quy trình báo lỗi, đề xuất và thảo luận
	governance/    RFC, quyết định, maintainers, releases
	ideas/         mẫu ghi nhận vấn đề và đề xuất
	product/       phạm vi sản phẩm và nhóm người dùng
	roadmap/       mốc v1 và backlog
	tokens/        màu sắc, typography, kích thước, motion
	ui/            nguyên tắc, accessibility và đặc tả component
```

## Đóng góp

Đọc [CONTRIBUTING.md](CONTRIBUTING.md), sau đó mở issue hoặc RFC trước thay đổi ảnh hưởng API, tokens hay chính sách tương thích. Mọi nội dung đều cần kiểm tra bằng ví dụ sử dụng và tiêu chí chấp nhận.

## Deploy GitHub Pages

Workflow `.github/workflows/deploy.yml` build site từ Markdown và deploy tự động khi có push lên `main`; có thể chạy thủ công từ tab Actions. Trong GitHub repository settings, đặt **Pages → Build and deployment → Source** thành **GitHub Actions**. Site dùng base path `/design-system`.