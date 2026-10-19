# GProject - Thực Hành Cài Đặt Node.js, npm & Biên Dịch SASS (SCSS sang CSS)

Dự án hướng dẫn chi tiết và thực hành toàn diện quy trình kiểm tra, cài đặt **Node.js**, **npm**, **SASS CLI** và biên dịch tệp **SCSS sang CSS** theo chuẩn chuyên nghiệp.

---

## 📌 1. Kết quả kiểm tra môi trường trên hệ thống

| Công cụ | Lệnh kiểm tra | Phiên bản đã cài đặt | Trạng thái |
| :--- | :--- | :--- | :--- |
| **Node.js** | `node -v` | **v20.18.0** | ✅ Đã cài đặt & cấu hình PATH |
| **npm** | `npm -v` | **10.8.2** | ✅ Hoạt động sẵn sàng |
| **SASS CLI** | `sass --version` | **1.99.0** (Dart Sass) | ✅ Cài đặt toàn cục qua `npm install -g sass` |

---

## 📂 2. Cấu trúc tệp SCSS và CSS trong dự án

```text
GProject/
├── package.json              (Cấu hình npm scripts quản lý build/watch SASS)
├── styles.scss               (Tệp SCSS đơn thực hành biên dịch trực tiếp)
├── styles.css                (Tệp CSS sau khi biên dịch từ styles.scss)
├── scss/                     (Thư mục chứa các tệp module SCSS)
│   ├── _variables.scss       (Biến SASS: màu sắc, font, shadow)
│   ├── _mixins.scss          (Mixins: flexbox, transition, border-radius)
│   ├── _header.scss          (Module định dạng Header)
│   ├── _navbar.scss          (Module định dạng Navbar)
│   ├── _cards.scss           (Module định dạng Card Layout)
│   ├── _footer.scss          (Module định dạng Footer)
│   └── styles.scss           (Tệp SCSS chính import các module)
├── css/
│   ├── styles.css            (Tệp CSS được biên dịch tự động từ thư mục scss/)
│   └── style.css             (CSS gốc của website)
└── images/                   (Tài nguyên hình ảnh)
```

---

## 🚀 3. Hướng dẫn các lệnh SASS CLI đã thực hành

### 🔹 Biên dịch một tệp đơn:
```bash
sass styles.scss styles.css
```
*Tự động chuyển đổi `styles.scss` thành `styles.css`.*

### 🔹 Kích hoạt chế độ theo dõi tự động (Watch mode):
```bash
sass styles.scss styles.css --watch
```
*Tự động biên dịch lại ngay khi lưu thay đổi trong tệp SCSS.*

### 🔹 Biên dịch nhiều tệp SCSS cùng lúc (Thư mục đầu vào -> đầu ra):
```bash
sass scss/:css/ --watch
```
*Theo dõi toàn bộ thư mục `scss/` và xuất kết quả sang `css/styles.css`.*

### 🔹 Sử dụng thông qua npm scripts:
```bash
# Biên dịch một lần:
npm run build-css

# Chế độ theo dõi liên tục:
npm run watch-css
```

---

## 🛠️ 4. Xử lý lỗi quyền thực thi trên Windows PowerShell
Khi gặp lỗi script ExecutionPolicy trên Windows:
```powershell
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned -Force
```
Lệnh này cho phép chạy các tập lệnh CLI như `sass` hoặc `npm` một cách an toàn mà không bị giới hạn quyền truy cập.
