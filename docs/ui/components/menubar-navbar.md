# Menubar và navbar

## Phân biệt

Navbar là vùng điều hướng liên kết trong trang/ứng dụng. Menubar là pattern điều khiển lệnh có tương tác bàn phím kiểu menu. Không dùng role `menubar` cho thanh link thông thường.

## Navbar

Hỗ trợ landmark navigation có nhãn, link active với trạng thái rõ, responsive collapse và thứ tự DOM phù hợp. Nút mở menu công bố expanded state; thay đổi kích thước màn hình không làm mất focus hoặc nội dung.

## Menubar

Chỉ dùng khi giao diện thực sự có mô hình menu lệnh. Đặc tả roving focus, phím mũi tên, Home/End, Enter/Space, Escape và hành vi submenu; hỗ trợ screen reader theo pattern được chọn.

Kiểm thử nhiều navigation landmark, focus, mobile, zoom và menu lồng nhau. Tránh mega-menu nếu chưa có use case xác thực.