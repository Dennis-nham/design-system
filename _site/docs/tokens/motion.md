# Motion tokens

Motion giúp giải thích chuyển trạng thái, không trang trí cho mọi thao tác. Định nghĩa duration/easing theo nhóm (instant, short, standard) sau khi có prototype đo được.

- Tôn trọng `prefers-reduced-motion` và cung cấp trạng thái tương đương không chuyển động.
- Tránh animation làm chậm thao tác lặp lại hoặc gây nhấp nháy.
- Không animate layout lớn nếu có thể chuyển opacity/transform nhẹ và không làm mất ngữ nghĩa.
- Kiểm thử với nội dung động, toast và menu liên tiếp.

Giá trị token cụ thể là provisional cho tới khi được kiểm thử và thông qua.