# GProject - Layout Bootstrap (Online Shopping Mall)

Dự án thực hành sử dụng các thành phần của **Bootstrap 3.3.7** để xây dựng bố cục trang web thương mại điện tử **Online Shopping Mall**.

## 📌 Các bước và thành phần đã thực hiện:
1. **Khung bố cục chung (`layout.html`)**:
   - Sử dụng `.container` với các phần: `header.row`, `nav.navbar.navbar-inverse`, thân trang gồm `article.col-sm-9` và `aside.col-sm-3`, cùng `footer.panel.panel-default`.
2. **Thiết kế Header**:
   - Khối `.shopping-mall` với tiêu đề `h1` kiểu chữ Impact, phụ đề `h5`.
   - Hình ảnh quà tặng đẩy sang phải với lớp `.pull-right`.
3. **Thanh điều hướng Menu (`nav.navbar-inverse`)**:
   - Tích hợp biểu tượng **Bootstrap Glyphicons**:
     - 🏠 Trang chủ (`glyphicon-home`)
     - 📋 Giới thiệu (`glyphicon-list-alt`)
     - 📞 Liên hệ (`glyphicon-earphone`)
     - ✉️ Góp ý (`glyphicon-envelope`)
     - ❓ Hỏi đáp (`glyphicon-question-sign`)
     - 👤 Tài khoản (`glyphicon-user`) kèm Dropdown menu.
4. **Khu vực nội dung chính (`article.col-sm-9`)**:
   - Chia lưới mỗi hàng 3 sản phẩm, mỗi sản phẩm chiếm 4 cột (`col-sm-4.poly-prod`).
   - Cấu trúc thẻ sản phẩm: `.panel-heading` (Tên sản phẩm), `.panel-body` (Hình ảnh), `.panel-footer` (Đơn giá).
5. **Khu vực thanh bên (`aside.col-sm-3`)**:
   - Giỏ hàng (`.poly-cart`): Hình ảnh 5 cột, thông tin giỏ hàng 7 cột.
   - Ô tìm kiếm: Ô nhập từ khóa với `.form-control`.
   - Danh mục chủng loại hàng: Panel kết hợp `.list-group`.
6. **Footer**:
   - Hiển thị thông tin bản quyền: `CodeGym © 2017`.

## 📁 Danh sách tệp tin trong dự án:
- `layout.html`: Mã nguồn chính của bài thực hành theo yêu cầu đề bài.
- `index.html`: Bản sao đồng bộ của `layout.html` giúp xem trực tiếp trên GitHub Pages / Root.
- `poly.css`: Các lớp định dạng CSS tùy biến (`header`, `.shopping-mall`, `.poly-cart`, `.poly-prod`).
- `images/`:
  - `header-object.png`: Hình ảnh banner header.
  - `shoppingcart.gif`: Biểu tượng giỏ hàng.
  - `computer.png`: Hình ảnh sản phẩm.
- `layout-result.png`: Ảnh chụp minh chứng kết quả chạy trên trình duyệt.
