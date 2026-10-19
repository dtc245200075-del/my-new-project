# GProject - Creative Web Design (Website Template Nâng Cao)

Dự án bài tập: **Giao Diện Đẹp Mắt - Website Template Nâng Cao** sử dụng HTML5, CSS Flexbox & CSS Grid, hình nền hiệu ứng blur và thanh điều hướng cố định (fixed navbar).

---

## 🌟 Tính năng & Cấu trúc giao diện

1. **Header với nền ảnh và hiệu ứng Blur (`.header`)**:
   - Sử dụng hình nền `banner.jpg` chất lượng cao với pseudo-element `::before` áp dụng `filter: blur(8px)`.
   - Lớp phủ tối `::after` với `rgba(0, 0, 0, 0.5)` giúp tiêu đề `Creative Web Design` và nút kêu gọi hành động (`.btn`) nổi bật, rõ ràng.
2. **Navigation Menu cố định (`.navbar`)**:
   - Menu cố định trên cùng (`position: fixed; top: 0; z-index: 1000`) khi cuộn trang.
   - Các liên kết menu: *Trang chủ*, *Dịch vụ*, *Blog*, *Liên hệ* có hiệu ứng chuyển màu mượt mà khi hover (`#f39c12`).
3. **Content Section - Card Layout (`.card-container`, `.card`)**:
   - Bố cục lưới **CSS Grid** (`grid-template-columns: repeat(3, 1fr)`).
   - 3 Card dịch vụ hiện đại kèm hình ảnh minh họa chân thực:
     - **Thiết kế Website** (`images/service1.jpg`)
     - **SEO & Marketing** (`images/service2.jpg`)
     - **Hỗ trợ 24/7** (`images/service3.jpg`)
   - Hiệu ứng tương tác hover phóng to nhẹ (`transform: scale(1.05)`).
   - Sử dụng dấu chấm (`•`) chuẩn theo yêu cầu để phân cấp nội dung chuyên nghiệp.
4. **Footer chuyên nghiệp 2 cột (`.footer`)**:
   - Sử dụng **Flexbox** với `justify-content: space-between`.
   - Cột trái: Thông tin bản quyền (`• © 2025 Creative Web. All rights reserved.`).
   - Cột phải: Kênh truyền thông (`• Theo dõi chúng tôi: • Facebook | Twitter | LinkedIn`).

---

## 📁 Cấu trúc thư mục

```text
website-template-advanced/
├── index.html
├── css/
│   ├── style.css
├── images/
│   ├── banner.jpg
│   ├── service1.jpg
│   ├── service2.jpg
│   ├── service3.jpg
```
*(Đồng thời toàn bộ mã nguồn cũng được đặt tại thư mục gốc để thuận tiện truy cập trực tiếp).*

---

## 📸 Kết quả hiển thị

Giao diện hiển thị trực quan và đã được kiểm tra trên trình duyệt:
- `advanced-template-result.png`
