# GProject - Chuyển Đổi CSS Truyền Thống Sang SASS Chuẩn

Dự án thực hành chuẩn hóa mã nguồn CSS sang kiến trúc **Modular SASS/SCSS** chuyên nghiệp theo cấu trúc thư mục 7-1 pattern tinh gọn: `abstracts`, `base`, `layout`, và `components`.

---

## 🎯 1. So Sánh Trước & Sau Khi Chuẩn Hóa SASS

### 🔹 File CSS ban đầu (`styles.css`):
```css
body {
  font-family: Arial, sans-serif;
  color: #333;
  background: #f4f4f4;
}

.container {
  width: 80%;
  margin: 0 auto;
}

.button {
  background: blue;
  color: white;
  padding: 10px 20px;
  border-radius: 5px;
}

.card {
  border: 1px solid #ddd;
  padding: 20px;
  box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.1);
}
```

### 🔹 Cấu trúc SASS chuẩn hóa:
Tách thành các module riêng biệt giúp dễ bảo trì, mở rộng và tái sử dụng mã.

---

## 📂 2. Cấu Trúc Thư Mục Chuẩn Hóa

```text
GProject/
├── abstracts/
│   ├── _variables.scss       # Biến màu sắc, nền, border, shadow
│   └── _mixins.scss          # Mixin tái sử dụng button-style và box-shadow
├── base/
│   └── _global.scss          # Định dạng chung cho thẻ body
├── layout/
│   └── _container.scss       # Định dạng layout khối container
├── components/
│   ├── _buttons.scss         # Component nút bấm áp dụng @include button-style
│   └── _cards.scss           # Component thẻ card áp dụng @include box-shadow
├── main.scss                 # File tập trung import toàn bộ partials
├── main.css                  # File CSS được biên dịch tự động từ main.scss
├── demo.html                 # Giao diện demo kiểm thử các component
└── package.json              # Quản lý lệnh biên dịch qua npm scripts
```

---

## 📝 3. Chi Tiết Mã Nguồn SCSS

### 🔸 `abstracts/_variables.scss`
```scss
$primary-color: blue;
$text-color: #333;
$background-color: #f4f4f4;
$border-color: #ddd;
$box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.1);
```

### 🔸 `abstracts/_mixins.scss`
```scss
@mixin button-style($bg-color) {
  background: $bg-color;
  color: white;
  padding: 10px 20px;
  border-radius: 5px;
}

@mixin box-shadow {
  box-shadow: $box-shadow;
}
```

### 🔸 `base/_global.scss`
```scss
body {
  font-family: Arial, sans-serif;
  color: $text-color;
  background: $background-color;
}
```

### 🔸 `layout/_container.scss`
```scss
.container {
  width: 80%;
  margin: 0 auto;
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
  border: 1px solid $border-color;
  padding: 20px;
  @include box-shadow;
}
```

### 🔸 `main.scss`
```scss
@import "abstracts/variables";
@import "abstracts/mixins";
@import "base/global";
@import "layout/container";
@import "components/buttons";
@import "components/cards";
```

---

## 🚀 4. Lệnh Biên Dịch SASS

```bash
# Biên dịch main.scss ra main.css:
sass main.scss main.css

# Chế độ tự động cập nhật khi sửa SCSS:
sass main.scss main.css --watch

# Sử dụng npm script:
npm run build-main
```
