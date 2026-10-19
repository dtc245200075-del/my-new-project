# GProject - Phân Tích & Triển Khai Website Template Cơ Bản (HTML & CSS)

## 🎯 Mục tiêu bài tập
1. Phân tích cấu trúc của một website thực tế theo các phần chính: Header, Navigation Menu, Content Section, Footer.
2. Xây dựng lại bố cục tương tự bằng HTML5 & CSS với cấu trúc file/thư mục chuẩn, tinh gọn, khoa học.

---

## 🔍 BÁO CÁO PHÂN TÍCH CẤU TRÚC WEBSITE THỰC TẾ

### 1. Header (Đầu trang)
- **Vị trí & Vai trò:** Nằm ở vị trí trên cùng của website, đóng vai trò nhận diện thương hiệu và gây ấn tượng đầu tiên cho người truy cập.
- **Bố cục:** Chứa tiêu đề chính của trang web (`<h1>Creative Web Design</h1>`), dòng thông điệp giới thiệu (*Thiết kế website chuyên nghiệp - Hiện đại - Ấn tượng*) và nút kêu gọi hành động CTA (*Khám phá ngay*). Nền sử dụng hình ảnh sắc nét kèm hiệu ứng làm mờ (blur) để nổi bật nội dung chữ.

### 2. Navigation Menu (Thanh điều hướng)
- **Vị trí & Vai trò:** Đặt ngay sau Header (hoặc ghim cố định ở đầu trang), giúp người dùng dễ dàng chuyển đổi qua lại giữa các phần trong website.
- **Bố cục:** Gồm 4 mục điều hướng cốt lõi:
  - `Trang chủ`: Quay về trang chính.
  - `Dịch vụ`: Điều hướng nhanh đến phần giới thiệu dịch vụ.
  - `Blog`: Trang chia sẻ kiến thức và tin tức.
  - `Liên hệ`: Kênh kết nối và thông tin hỗ trợ.
- **Trải nghiệm UX:** Có hiệu ứng đổi màu mượt mà khi di chuột (hover).

### 3. Content Section (Phần nội dung chính)
- **Vị trí & Vai trò:** Phần trung tâm thể hiện giá trị và dịch vụ của doanh nghiệp.
- **Bố cục:** Thiết kế theo dạng thẻ (Card Layout) sử dụng CSS Grid chia thành 3 cột cân đối:
  - Thẻ 1: **Thiết kế Website** (Kèm ảnh minh họa & mô tả dịch vụ).
  - Thẻ 2: **SEO & Marketing** (Kèm ảnh dashboard chỉ số & mô tả).
  - Thẻ 3: **Hỗ trợ 24/7** (Kèm ảnh đội ngũ chăm sóc khách hàng & mô tả).
- Sử dụng dấu chấm (`•`) để phân cấp và nhấn mạnh từng ý nội dung rõ ràng, mạch lạc.

### 4. Footer (Chân trang)
- **Vị trí & Vai trò:** Nằm ở đáy trang web, chốt lại thông tin bản quyền và kết nối đa kênh.
- **Bố cục:** Bố trí 2 cột ngang đối xứng bằng Flexbox (`justify-content: space-between`):
  - Cột trái: Bản quyền sở hữu trí tuệ (`• © 2025 Creative Web. All rights reserved.`).
  - Cột phải: Kênh truyền thông xã hội (`• Theo dõi chúng tôi: • Facebook | Twitter | LinkedIn`).

---

## 📁 Tổ chức File và Thư mục Dự án

```text
GProject/
├── index.html                     (Mã HTML bố cục trang)
├── style.css                      (CSS định dạng giao diện)
├── css/
│   └── style.css                  (CSS thư mục chuẩn)
├── images/                        (Thư mục chứa tài nguyên ảnh)
│   ├── banner.jpg                 (Ảnh nền Header)
│   ├── service1.jpg               (Ảnh dịch vụ Thiết kế Web)
│   ├── service2.jpg               (Ảnh dịch vụ SEO & Marketing)
│   └── service3.jpg               (Ảnh dịch vụ Hỗ trợ 24/7)
├── original-website-analysis.png  (Ảnh chụp màn hình trang web gốc đã phân tích)
└── README.md                      (Báo cáo phân tích và tài liệu dự án)
```

---

## 📸 Ảnh chụp màn hình trang web phân tích
Ảnh chụp màn hình trang web thực tế được lưu tại: `original-website-analysis.png`
