---
layout: default
title: Design tokens
---

# Design tokens

Tokens là hợp đồng đặt tên cho giá trị thiết kế. Ưu tiên tên theo vai trò (`color.text.primary`) thay vì tên theo sắc độ (`blue.700`) trong API sử dụng. Alias primitive có thể được giữ ở lớp nguồn.

Hướng dẫn thị giác tham chiếu iOS 16 và cách quy đổi sang web nằm trong [tài liệu UI iOS 16](../ui/ios16-reference.md).

| Đặc tả | Nội dung |
| --- | --- |
| [Color](color.md) | Semantic palette và theme |
| [Typography](typography.md) | Font roles, scale và line-height |
| [Spacing, radius, elevation](layout.md) | Nhịp layout và bề mặt |
| [Motion](motion.md) | Timing, easing và reduced motion |

Định dạng nguồn và cơ chế build cần được chọn bằng ADR. Mỗi token public cần mô tả ý nghĩa, theme, ví dụ và chính sách deprecation.