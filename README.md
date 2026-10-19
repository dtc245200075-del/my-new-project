# GProject - Tạo Landing Page với Bootstrap và Hình Ảnh

Dự án thực hành xây dựng **Landing Page responsive kết hợp hình ảnh** sử dụng **Bootstrap 5.3.0 Containers, Grid System, Buttons và Images**.

## 📌 Các thành phần chính của Landing Page:
1. **Banner / Hero Section**:
   - Sử dụng Bootstrap 5 (không dùng `.jumbotron` vì đã bị loại bỏ ở BS5) với các utility classes: `container`, `py-5`, `bg-*`, `text-center`.
   - Hình ảnh banner nổi bật tối ưu responsive với lớp `img-fluid`, `rounded`, `shadow`.
   - Nút kêu gọi hành động chính (CTA): `btn btn-primary btn-lg` (*Đăng Ký Ngay* / *Khám Phá Ngay*).
2. **Giới thiệu (About / Intro Section)**:
   - Một hàng `row` sử dụng Bootstrap Grid System:
     - Cột 1: Hình ảnh sản phẩm / đội ngũ áp dụng lớp `img-fluid rounded shadow-sm`.
     - Cột 2: Tiêu đề và đoạn văn bản mô tả chi tiết sản phẩm / dịch vụ.
3. **Danh sách tính năng (Features Section)**:
   - Một hàng `row` gồm 4 cột (`col-12 col-sm-6 col-md-3 text-center`):
     - ⚡ **Tốc độ vượt trội**: Tối ưu hiệu năng tải trang nhanh chóng.
     - 📱 **Đa nền tảng**: Tương thích mượt mà trên cả di động và máy tính.
     - 🔒 **Bảo mật tối tân**: Bảo vệ dữ liệu người dùng tuyệt đối.
     - 🛠️ **Hỗ trợ 24/7**: Đồng hành cùng khách hàng mọi lúc mọi nơi.
4. **Nút Kêu Gọi Hành Động (CTA Section)**:
   - Khu vực CTA tập trung lời kêu gọi đăng ký và các nút hành động kích thước lớn `btn-lg`.
5. **Footer**:
   - Thông tin bản quyền cuối trang (`bg-dark text-white text-center py-4`).

## 📁 Danh sách tệp tin trong dự án:
- `index.html`: Landing page hoàn chỉnh với thiết kế cao cấp, hình ảnh độ phân giải cao và tính responsive.
- `landing-images-exact.html`: Mã nguồn chuẩn từng dòng theo cấu trúc gợi ý trong bài học.
- `images/hero.jpg`: Hình ảnh banner hero công nghệ.
- `images/intro.jpg`: Hình ảnh giới thiệu sản phẩm / đội ngũ.
- `style.css`: Quy tắc định dạng CSS tùy biến giao diện.
- `landing-images-desktop.png`: Ảnh chụp giao diện Desktop.
- `landing-images-sample.png`: Ảnh chụp giao diện mẫu chuẩn đề bài.
- `landing-images-mobile.png`: Ảnh chụp giao diện Mobile responsive.
