# GProject - Tái Cấu Trúc Responsive Grid Bằng SASS

Dự án bài tập: Tái cấu trúc mã nguồn HTML & CSS của repository **[codegym-vn/responsive-grid](https://github.com/codegym-vn/responsive-grid)** sang kiến trúc **SASS/SCSS** chuẩn mực, linh hoạt và dễ bảo trì.

---

## 🌟 1. Điểm Cải Tiến Khi Chuyển Sang SASS

1. **Loại bỏ hoàn toàn CSS nội tuyến (`inline styles`)**:
   - Trước: Toàn bộ màu nền, chiều cao, viền và độ rộng được nhúng trực tiếp trong thuộc tính `style="..."`.
   - Sau: Được trừu tượng hóa thành các class ngữ nghĩa rõ ràng: `.header-bar`, `.sidebar-menu`, `.content-panel`, `.footer-bar`, `.guide-grid`.
2. **Sử dụng Biến SASS (`$variables`)**:
   - Quản lý tập trung số lượng cột (`$grid-columns: 12`), bảng màu sắc chuẩn (`$header-color: #9933cc`, `$sidebar-color: #33b5e5`, `$footer-color: #0099cc`), và chiều cao từng hàng.
3. **Sử dụng Mixins & Vòng lặp `@for`**:
   - Tự động sinh 12 class lưới `.col-1` đến `.col-12` bằng vòng lặp `@for $i from 1 through 12` kết hợp mixin `@include grid-column($i, 12)`.
   - Tái sử dụng mixin `@mixin clearfix` để làm sạch luồng float của các cột.
4. **Cấu trúc module SASS chuyên nghiệp**:
   - Chia tách rõ ràng giữa biến (`_variables.scss`), mixin (`_mixins.scss`) và hệ thống lưới (`_grid-system.scss`).

---

## 📂 2. Cấu Trúc Thư Mục Dự Án

```text
GProject/
├── scss/
│   └── grid/
│       ├── _variables.scss       # Biến quản lý màu sắc, chiều cao, số cột lưới
│       ├── _mixins.scss          # Mixin clearfix và grid-column tính toán độ rộng cột
│       └── _grid-system.scss     # Hệ thống 12 cột và các component layout
├── responsive-grid.scss          # File SCSS trung tâm import toàn bộ partials
├── responsive-grid.css           # File CSS được biên dịch tự động từ SASS
├── responsive_grid.htm           # Mã HTML cấu trúc chuẩn đã được dọn sạch inline CSS
├── responsive-grid.html          # Bản sao HTML định dạng chuẩn
├── package.json                  # Quản lý script biên dịch SASS
└── README.md                     # Tài liệu hướng dẫn & giải thích dự án
```

---

## 📝 3. Chi Tiết Mã Nguồn SCSS

### 🔸 `scss/grid/_variables.scss`
```scss
$grid-columns: 12;
$grid-border-color: grey;
$grid-bg: #f1f1f1;
$guide-border-color: #000000;

$header-color: #9933cc;
$sidebar-color: #33b5e5;
$footer-color: #0099cc;
$white: #ffffff;

$header-height: 90px;
$main-height: 230px;
$footer-height: 50px;
$guide-height: 370px;
```

### 🔸 `scss/grid/_mixins.scss`
```scss
@mixin clearfix {
  &::after {
    content: "";
    display: table;
    clear: both;
  }
}

@mixin grid-column($col-num, $total-cols: $grid-columns) {
  width: calc(100% / #{$total-cols} * #{$col-num});
  float: left;
}
```

### 🔸 Sinh 12 cột tự động (`scss/grid/_grid-system.scss`):
```scss
@for $i from 1 through $grid-columns {
  .col-#{$i} {
    @include grid-column($i, $grid-columns);
  }
}
```

---

## 🚀 4. Lệnh Biên Dịch & Chạy Dự Án

```bash
# Biên dịch responsive-grid.scss ra CSS:
sass responsive-grid.scss responsive-grid.css

# Chế độ theo dõi tự động:
sass responsive-grid.scss responsive-grid.css --watch

# Dùng qua npm script:
npm run build-grid
```
