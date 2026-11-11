# 5-min Horizon

Theo dõi tin tức tài chính - kinh tế - chính sách trong 5 phút. Web app (PWA) tĩnh, không cần máy chủ.

## Cấu trúc
- `index.html`: toàn bộ trang (giao diện, tin, chỉ số)
- `manifest.webmanifest`: tên app, màu, biểu tượng
- `sw.js`: service worker (đọc lại được khi mất mạng; luôn ưu tiên tải bản mới khi có mạng)
- `icon-*.png`, `apple-touch-icon.png`: biểu tượng app
- `logo.svg`, `logo-512.png`: logo (mặt trời mọc với 5 tia sáng trên đường chân trời), dùng được cho ảnh đại diện, bài đăng

## Đưa lên GitHub Pages
1. Tạo repository mới trên GitHub (ví dụ `5min-horizon`), để chế độ Public.
2. Tải toàn bộ file trong thư mục này lên nhánh `main` (nút Add file > Upload files, hoặc dùng git).
3. Vào Settings > Pages > Source: chọn "Deploy from a branch", nhánh `main`, thư mục `/ (root)`, bấm Save.
4. Sau 1–2 phút, trang có địa chỉ dạng `https://<tên-người-dùng>.github.io/5min-horizon/`.

## Cài lên điện thoại
- iPhone (Safari): mở địa chỉ trên, bấm nút Chia sẻ, chọn "Thêm vào Màn hình chính".
- Android (Chrome): menu ba chấm, chọn "Cài đặt ứng dụng" hoặc "Thêm vào màn hình chính".

## Cập nhật tin mỗi ngày
Thay file `index.html` bằng bản mới rồi commit. Người dùng mở app khi có mạng sẽ tự thấy bản mới. Chỉ cần đổi `CACHE` trong `sw.js` (ví dụ `5min-horizon-v2`) khi bạn sửa biểu tượng hoặc manifest.

## Gắn tên miền riêng (tùy chọn)
Settings > Pages > Custom domain, nhập tên miền, rồi trỏ DNS theo hướng dẫn của GitHub. Khi đó đường dẫn gốc là `/`, các file vẫn chạy đúng vì đều dùng đường dẫn tương đối.

## Lưu ý
Số liệu và tin trong `index.html` là bản chụp theo thời điểm ghi ở đầu trang, không tự động cập nhật. Không phải khuyến nghị đầu tư.
