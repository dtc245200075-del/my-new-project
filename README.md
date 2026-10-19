# GProject - Bố cục Web Responsive với Bootstrap Containers & Grid System

Dự án thực hành thiết kế bố cục trang web responsive sử dụng **Bootstrap 5.3.0 Containers & Grid System**.

## 📌 Các thành phần chính và yêu cầu kỹ thuật:
1. **Header**: Chứa tiêu đề trang web (`.bg-primary.text-white.text-center.py-4`).
2. **Navbar**: Thanh điều hướng Bootstrap Navbar tích hợp menu thả xuống (Dropdown) và nút Hamburger trên di động.
3. **Bootstrap Container**: Sử dụng thẻ `.container` giới hạn chiều rộng nội dung, tự động căn giữa theo từng breakpoint responsive.
4. **Hệ thống lưới Bootstrap Grid System (`row`, `col-xx`)**:
   - **Trên Desktop (≥992px):** Chia làm 2 cột chính nằm song song:
     - **Main Content**: Chiếm 8 cột (`col-lg-8` / `col-md-8`).
     - **Sidebar**: Chiếm 4 cột (`col-lg-4` / `col-md-4`).
   - **Trên Mobile (<992px):** Cả hai cột sử dụng `col-12`, giúp Sidebar tự động chuyển xuống bên dưới Main Content, hiển thị dạng 1 cột tối ưu cho màn hình nhỏ.
5. **Footer**: Chứa thông tin bản quyền cuối trang (`.bg-dark.text-white.text-center.py-4`).

## 📁 Danh sách tệp tin trong repository:
- `index.html`: Bố cục hoàn chỉnh với thiết kế thẩm mỹ cao, chuẩn Bootstrap 5.
- `grid-layout-exact.html`: Mã nguồn chuẩn từng dòng theo đúng khung đề bài hướng dẫn.
- `style.css`: Quy tắc tùy biến CSS giao diện.
- `containers-grid-sample.png`: Ảnh chụp giao diện khung bài làm chuẩn đề bài.
- `containers-grid-desktop.png`: Ảnh chụp giao diện Desktop (2 cột: 8 - 4).
- `containers-grid-mobile.png`: Ảnh chụp giao diện Mobile (1 cột: 12).
