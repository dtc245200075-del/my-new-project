# GProject - Trang Giới Thiệu Sản Phẩm Apple iPhone (Bootstrap 5)

Dự án thực hành xây dựng **Trang Giới Thiệu Sản Phẩm chuẩn phong cách Apple iPhone** bằng **Bootstrap 5.3.3** và **Font Awesome 6.5.2**, ứng dụng các thuộc tính Display Property, Margin & Padding, Flexbox (`justify-content`, `align-items`) và Grid System.

## 📌 Các thành phần và kỹ thuật nổi bật:
1. **Apple Minimalist Navbar**:
   - Sử dụng `.navbar-expand-lg.navbar-dark.bg-black` với logo `<i class="fab fa-apple"></i>`.
   - Căn giữa các mục menu bằng Flexbox (`justify-content-center`) và phân bổ khoảng cách `gap-lg-4`.
2. **Sub-Navbar Sticky**:
   - Tên sản phẩm **iPhone 16 Pro** và nút CTA **Mua ngay** (`btn-primary rounded-pill`) ghim cố định trên đầu trang.
3. **Hero Section (Bố cục Flexbox & Typography)**:
   - Căn giữa hoàn hảo bằng `d-flex flex-column justify-content-center align-items-center`.
   - Tiêu đề sản phẩm lớn `display-3 fw-bolder`.
   - Cụm nút hành động căn chỉnh bằng Flexbox và các lớp `gap-3`, `margin`, `padding`.
   - Hình ảnh sản phẩm chất lượng cao tối ưu co giãn bằng `img-fluid`.
4. **Highlights Section (Bootstrap Grid System)**:
   - Hệ thống lưới 4 cột (`row g-4`, `col-12 col-sm-6 col-lg-3`) giới thiệu các tính năng đột phá:
     - 🚀 **Chip A18 Pro**: `<i class="fas fa-microchip"></i>`
     - 📷 **Nút Điều Khiển Camera**: `<i class="fas fa-camera"></i>`
     - 💎 **Titanium Cấp 5**: `<i class="fas fa-gem"></i>`
     - 🔋 **Pin Bền Bỉ**: `<i class="fas fa-battery-full"></i>`
5. **Comparison Grid (So sánh sản phẩm)**:
   - Lưới 2 cột so sánh giữa iPhone 16 Pro và iPhone 16.
6. **Footer chuẩn Apple**:
   - Chú thích pháp lý, giá bán và bản quyền `Apple Inc.`.

## 📁 Danh sách tệp tin:
- `index.html`: Toàn bộ mã nguồn trang giới thiệu sản phẩm iPhone.
- `iphone.jpg`: Hình ảnh sản phẩm flagship Titanium.
- `iphone-product-desktop.png`: Ảnh chụp giao diện Desktop chuẩn Apple.
- `iphone-product-mobile.png`: Ảnh chụp giao diện Mobile responsive.
