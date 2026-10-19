# GProject - Thực hành Bootstrap 5 Tổng Hợp

Dự án thực hành sử dụng **Bootstrap 5.3.3** để tạo bố cục linh hoạt, ứng dụng Display Property, Margin & Padding, Flexbox, Carousel, Font Awesome và Form.

## 📌 Các bước thực hiện chi tiết:
1. **Bước 1 (Grid 3 cột & Flexbox căn giữa)**:
   - Sử dụng `.container.mt-5` và `.row`.
   - 3 cột `.col-md-4` kết hợp `.d-flex.justify-content-center.align-items-center` với các màu nền `bg-light`, `bg-secondary text-white`.
2. **Bước 2 (Margin & Padding)**:
   - Áp dụng `.my-5.py-3` tạo khoảng cách cho tiêu đề.
3. **Bước 3 (Display Property ẩn / hiện)**:
   - Sử dụng `.d-none.d-md-block.bg-warning.text-center.p-3` chỉ hiển thị trên màn hình lớn &ge; 768px.
4. **Bước 4 (Carousel 3 Slides)**:
   - Khối `#myCarousel` dạng slideshow tự động chuyển ảnh với nút prev/next.
5. **Bước 5 (Font Awesome)**:
   - Nhúng Font Awesome 6.5.2 và sử dụng `<i class="fas fa-home"></i>` và `<i class="fas fa-paper-plane"></i>`.
6. **Bước 6 (Form liên hệ)**:
   - Form gồm: Họ và tên (`#name`), Email (`#email`), Nội dung (`#message`) và nút Gửi (`btn btn-primary`).

## 📁 Danh sách tệp tin:
- `index.html`: Giao diện chính hoàn chỉnh.
- `exercise-exact.html`: Mã nguồn chuẩn 100% theo các đoạn code của đề bài.
- `image1.jpg`, `image2.jpg`, `image3.jpg`: 3 hình ảnh cho Carousel.
- `bootstrap-layout-sample.png`: Ảnh chụp kết quả trên trình duyệt.
