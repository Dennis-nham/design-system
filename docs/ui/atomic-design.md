# Atomic Design trong Dennis

Atomic Design là cách phân loại độ phức tạp, không phải yêu cầu mọi component phải ghép cứng theo một sơ đồ.

- **Atoms:** Button, Icon, Input, Badge, Avatar, Checkbox, Radio, Switch.
- **Molecules:** SearchField, DatePicker, TimePicker, ProfileSummary, FormField.
- **Organisms:** Menubar, Navbar, Calendar, NotificationCenter, Sidebar.
- **Templates:** cấu trúc trang như Admin hoặc Dashboard, chỉ đưa vào core khi có tính tổng quát cao.
- **Pages/apps:** thuộc sản phẩm tiêu thụ; không đặt nghiệp vụ CRM/ERP cụ thể trong package UI.

Component cấp cao có thể dùng component cấp thấp qua public API. Tránh phụ thuộc ngược từ atom vào organism. Nhóm theo tác vụ và API trước, cấp Atomic Design là metadata hỗ trợ khám phá.