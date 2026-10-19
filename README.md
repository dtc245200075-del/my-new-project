# GProject - Simple Web Development Template (HTML & CSS)

Dự án thực hành xây dựng cấu trúc và định dạng trang web **Simple Web Development Template** sử dụng thẻ `<section>` và **CSS Flexbox**.

## 📌 Các thành phần chính của trang web:
1. **Thanh điều hướng (`nav.navbar.background`)**:
   - Logo bo góc tròn (`.logo img`).
   - Danh sách menu liên kết: **Web Technology**, **C Programming**, **Courses**.
   - Khung tìm kiếm ở bên phải (`.rightNav`) với ô `#search` và nút `button.btn.btn-sm`.
2. **Phần 1: Web Technology (`section.firstsection`)**:
   - Nền màu xanh lá (`#1e7e34` / `green`), chiều cao `400px`.
   - Căn giữa nội dung bằng Flexbox (`.box-main`).
3. **Phần 2: C Programming (`section.secondsection`)**:
   - Nền màu xanh dương (`#0056b3` / `blue`), chiều cao `400px`.
   - Nội dung giới thiệu ngôn ngữ C.
4. **Phần 3: Java (`section.section`)**:
   - Bố cục Flexbox hai khối ngang: nội dung mô tả bên trái (`.paras`) và hình ảnh máy tính bên phải (`.thumbnail img`).
   - Hỗ trợ đổi chiều hiển thị linh hoạt với lớp `.section-Left` (`flex-direction: row-reverse`).
5. **Footer (`footer.background`)**:
   - Nền đen với dòng chữ bản quyền `Copyright © - All rights are reserved` căn giữa (`.text-footer`).

## 📁 Danh sách tệp tin:
- `index.html`: Toàn bộ cấu trúc HTML và liên kết CSS của trang web.
- `style.css`: Quy tắc định dạng CSS chi tiết theo đúng bài học.
- `logo.png`: Hình ảnh logo thanh điều hướng.
- `img.png`: Hình ảnh máy tính minh họa cho phần Java.
- `simple-template-result.png`: Ảnh chụp kết quả hiển thị trên trình duyệt.
