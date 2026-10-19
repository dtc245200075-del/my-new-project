# GProject - Bài tập Thực hành Bootstrap Navbar

Dự án thực hành xây dựng thanh điều hướng (Navbar) chuyên nghiệp sử dụng thư viện **Bootstrap 5.3.0**.

## 📌 Các thành phần chính của Bootstrap Navbar:
1. **Navbar Brand (`.navbar-brand`)**: Tên thương hiệu / logo `MyWebsite`.
2. **Mobile Toggler (`.navbar-toggler`)**: Nút Hamburger 3 gạch kết hợp `data-bs-toggle="collapse"` thu gọn và mở rộng menu trên thiết bị di động.
3. **Danh sách Menu (`.navbar-nav`)**:
   - `Home` (`.nav-link.active`)
   - `About` (`.nav-link`)
   - `Services` (`.nav-item.dropdown`): Menu thả xuống gồm **Web Design** và **SEO**.
   - `Contact` (`.nav-link`)
4. **Bootstrap Bundle JS**: Kích hoạt tính năng xổ menu thả xuống (Dropdown) và đóng/mở menu trên di động.

## 📁 Danh sách tệp tin:
- `index.html`: Giao diện chính tích hợp Bootstrap Navbar chuyên nghiệp kèm nội dung minh họa.
- `navbar.html`: Mã nguồn mẫu bài làm tiêu chuẩn 100% theo các bước hướng dẫn đề bài.
- `navbar-demo.html`: Trang kiểm thử đồng thời giao diện Desktop, Dropdown và Mobile.
- `style.css`: Quy tắc định dạng CSS tùy biến giao diện.
- `bootstrap-navbar-test-result.png`: Ảnh chụp minh chứng kiểm tra Menu, Dropdown và Mobile Toggler.

## 🚀 Trải nghiệm & Kết quả:
- **Desktop:** Navbar trải dài theo hàng ngang, dropdown xổ xuống mượt mà.
- **Mobile:** Menu tự động thu gọn vào nút 3 gạch, khi click sẽ bung menu xuống gọn gàng.
