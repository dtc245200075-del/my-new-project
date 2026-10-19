# responsive-grid - Tái Cấu Trúc Mã CSS Sang SASS (CodeGym)

Bài tập: **Luyện tập kỹ năng sử dụng SASS**  
Nguồn gốc: **[codegym-vn/responsive-grid](https://github.com/codegym-vn/responsive-grid)**

---

## 📌 1. Mục tiêu bài tập
- Luyện tập kỹ năng sử dụng SASS.
- Tái cấu trúc lại mã CSS hỗn độn (inline styles và thẻ `<style>`) trong mã nguồn có sẵn của CodeGym sang kiến trúc SASS/SCSS chuyên nghiệp.
- Ứng dụng: Biến SASS ($variables), Mixins (@mixin), Vòng lặp (@for) sinh hệ thống lưới 12 cột tự động.

---

## 🌟 2. Các cải tiến chính khi chuyển sang SASS
1. **Loại bỏ 100% CSS nội tuyến (`inline styles`)**:
   - Chuyển toàn bộ các thuộc tính nhúng `style="..."` trong các thẻ `div` thành các class CSS có ngữ nghĩa: `.header-bar`, `.sidebar-menu`, `.content-panel`, `.footer-bar`, `.guide-grid`.
2. **Khai báo hệ thống Biến SASS (`$variables`)**:
   - Quản lý tập trung: `$grid-columns: 12`, `$header-color: #9933cc`, `$sidebar-color: #33b5e5`, `$footer-color: #0099cc`, `$header-height: 90px`, `$main-height: 230px`, `$footer-height: 50px`.
3. **Sử dụng Mixins & Vòng lặp `@for`**:
   - Tự động sinh 12 cột `.col-1` đến `.col-12` bằng vòng lặp `@for $i from 1 through 12` và mixin `@include grid-column($i, 12)`.
   - Mixin `@mixin clearfix` làm sạch luồng float.

---

## 📂 3. Cấu trúc tệp tin trong repository
```text
GProject/
├── responsive_grid.htm           # File HTML chuẩn theo tên gốc của CodeGym
├── responsive-grid.html          # File HTML responsive
├── index.html                    # File HTML chính hiển thị responsive grid
├── responsive-grid.scss          # File SCSS chính
├── responsive-grid.css           # File CSS được biên dịch tự động từ SCSS
├── scss/
│   └── grid/
│       ├── _variables.scss       # Khai báo các biến SASS
│       ├── _mixins.scss          # Khai báo các mixin clearfix và grid-column
│       └── _grid-system.scss     # Bố cục 12 cột và các khối layout
├── responsive-grid-result.png    # Ảnh chụp màn hình kết quả chạy trên trình duyệt
└── README.md                     # Tài liệu hướng dẫn & giải thích
```

---

## 🚀 4. Lệnh biên dịch SASS
```bash
# Biên dịch sang CSS:
sass responsive-grid.scss responsive-grid.css

# Chế độ theo dõi tự động khi có thay đổi:
sass responsive-grid.scss responsive-grid.css --watch
```
