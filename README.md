# GProject - Tối Ưu Hóa CSS Bằng SASS Variables & Mixins

Dự án thực hành tối ưu hóa CSS bằng **SASS Variables** và **Mixins**, giúp giảm lặp code, kiểm soát giao diện tập trung và nâng cao tính tái sử dụng.

---

## 🎯 1. So Sánh Trước & Sau Khi Tối Ưu Hóa

### 🔹 File CSS ban đầu (trước tối ưu):
```css
h1 {
  font-size: 32px;
  color: #222;
}

h2 {
  font-size: 28px;
  color: #222;
}

.button {
  background: red;
  color: white;
  padding: 10px 20px;
  border-radius: 5px;
}

.card {
  background: white;
  padding: 15px;
  border-radius: 10px;
  box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.1);
}
```

### 🔹 Sau khi tối ưu bằng SASS:
- Các giá trị màu sắc, font chữ, khoảng cách và đổ bóng được chuyển thành **Biến SASS** trong `abstracts/_variables.scss`.
- Các khối CSS lặp lại (nút bấm, hộp card) được đóng gói thành **Mixins** trong `abstracts/_mixins.scss`.
- Phân chia module rõ ràng theo cấu trúc 7-1 pattern tinh gọn.

---

## 📂 2. Cấu Trúc Thư Mục Dự Án

```text
GProject/
├── abstracts/
│   ├── _variables.scss       # Khai báo biến: $primary-color, $text-color, $font-large, $font-medium, $padding-standard, $box-shadow-default
│   └── _mixins.scss          # Khai báo mixin: button-style($bg-color), box-style
├── base/
│   ├── _global.scss          # Định dạng chung cho body
│   └── _typography.scss      # Định dạng h1, h2 sử dụng biến SASS
├── layout/
│   └── _container.scss       # Định dạng khung .container
├── components/
│   ├── _buttons.scss         # Áp dụng @include button-style($primary-color)
│   └── _cards.scss           # Áp dụng @include box-style
├── main.scss                 # Tập hợp toàn bộ partials
├── main.css                  # File CSS sau khi biên dịch từ main.scss
├── demo.html                 # Trang demo kiểm thử trực quan
└── package.json              # Quản lý lệnh biên dịch SASS
```

---

## 📝 3. Chi Tiết Mã Nguồn SCSS

### 🔸 `abstracts/_variables.scss`
```scss
$primary-color: red;
$text-color: #222;
$font-large: 32px;
$font-medium: 28px;
$padding-standard: 10px 20px;
$box-shadow-default: 2px 2px 10px rgba(0, 0, 0, 0.1);
```

### 🔸 `abstracts/_mixins.scss`
```scss
@mixin button-style($bg-color) {
  background: $bg-color;
  color: white;
  padding: $padding-standard;
  border-radius: 5px;
}

@mixin box-style {
  background: white;
  padding: 15px;
  border-radius: 10px;
  box-shadow: $box-shadow-default;
}
```

### 🔸 `base/_typography.scss`
```scss
h1 {
  font-size: $font-large;
  color: $text-color;
}

h2 {
  font-size: $font-medium;
  color: $text-color;
}
```

### 🔸 `components/_buttons.scss`
```scss
.button {
  @include button-style($primary-color);
}
```

### 🔸 `components/_cards.scss`
```scss
.card {
  @include box-style;
}
```

### 🔸 `main.scss`
```scss
@import "abstracts/variables";
@import "abstracts/mixins";
@import "base/global";
@import "base/typography";
@import "layout/container";
@import "components/buttons";
@import "components/cards";
```

---

## 🚀 4. Lệnh Biên Dịch & Chạy Thử Nghiệm

```bash
# Biên dịch sang CSS:
sass main.scss main.css

# Chế độ tự động theo dõi khi có thay đổi:
sass main.scss main.css --watch

# Dùng npm scripts:
npm run build-main
```
