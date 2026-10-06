# My Website - Portfolio Cá Nhân (Lab 1, Lab 2 & Lab 3)

Dự án website cá nhân được xây dựng trong khuôn khổ môn học **Lập trình Web** tại trường **Đại học Gia Định**. Dự án áp dụng chuẩn **HTML5 Semantic**, hệ thống **biểu mẫu & HTML5 Validation**, tối ưu **SEO Onpage**, tiêu chuẩn tiếp cận **Accessibility (WCAG 2.2)** và định kiểu giao diện hiện đại bằng **CSS3 (CSS Reset, Selectors, Box Model, Typography)**.

---

## 👤 Thông tin sinh viên
- **Họ và tên**: Huỳnh Nguyễn Hà
- **Ngành**: Công nghệ thông tin – Chuyên ngành Kỹ thuật phần mềm
- **Trường**: Đại học Gia Định (GDU)
- **Năm học**: 2026 – 2027
- **GitHub Repository**: [my-website](https://github.com/nguyenha010707-jpg/my-website..git)

---

## 📁 Cấu trúc thư mục dự án

```text
my-website/
│
├── index.html       # Trang chủ: Giới thiệu chung, hình ảnh dự án Lab 1, layout card
├── about.html       # Trang giới thiệu: Thông tin cá nhân, sở thích, mục tiêu, bảng môn học, class highlight
├── contact.html     # Trang liên hệ: Biểu mẫu liên hệ với HTML5 Validation chuẩn
│
├── css/
│   └── style.css    # CSS chuẩn hóa: CSS Reset (*, *::before, *::after), Box Model, Typography, Form & Table styling
│
├── images/
│   └── project.png  # Ảnh chụp giao diện minh hoạ dự án
│
└── README.md        # Tài liệu thuyết minh dự án
```

---

## 🚀 Các tính năng và nội dung đã hoàn thiện

### 1. Lab 1: Cấu trúc HTML cơ bản & CSS Box Model
- Khởi tạo cấu trúc các trang web `index.html`, `about.html`, `contact.html`.
- Áp dụng các thẻ HTML5 Semantic: `<header>`, `<nav>`, `<main>`, `<section>`, `<figure>`, `<figcaption>`, `<footer>`, `<address>`.
- Xây dựng bảng môn học (Table) có `<thead>`, `<tbody>`, `<tfoot>`, `<caption>`.
- Định kiểu giao diện bằng CSS (`css/style.css`): Box-sizing reset, font chữ Google Fonts `Inter`, bảng màu hài hoà, card layout với `box-shadow` và `border-radius`.

### 2. Lab 2: Biểu mẫu HTML5, Validation thuần & SEO Onpage
- **Form liên hệ hoàn chỉnh (`contact.html`)**:
  - Phân chia 2 fieldset: `Thông tin cá nhân` và `Nội dung liên hệ`.
  - Đầy đủ các trường: `fullname` (text, required, minlength=2), `email` (email, required), `phone` (tel, regex pattern 10-11 số), `subject` (select 3 tùy chọn), kênh ưu tiên (3 radio buttons), `message` (textarea required, minlength=10), checkbox điều khoản (required).
  - *Nâng cao*: Ô chọn Ngày sinh (`type="date"`) và danh sách gợi ý trường đại học (`<datalist>`).
  - Nút bấm điều khiển: `<button type="submit">` và `<button type="reset">`.
- **Tối ưu SEO & Metadata**:
  - Thẻ `<title>`: Chuẩn 50–60 ký tự, chứa tên sinh viên và từ khóa chính.
  - Thẻ `<meta name="description">`: Chuẩn 150–160 ký tự, mở đầu bằng động từ hành động.
  - Thẻ Open Graph metadata (`og:title`, `og:description`, `og:type`, `og:url`) cho Zalo/Facebook.
  - Tiêu chuẩn Accessibility (WCAG 2.2): Quy tắc bắt buộc `label[for]` trỏ đúng `input[id]`, mỗi trang duy nhất 1 thẻ `<h1>`, tất cả ảnh có thuộc tính `alt` mô tả nội dung.

### 3. Lab 3 - Bài tập 01: CSS Selectors, Reset & Box Model
- **CSS Reset chuẩn ở đầu file**:
  ```css
  *, *::before, *::after {
      box-sizing: border-box; /* width bao gồm cả padding + border */
      margin: 0;
      padding: 0;
  }
  ```
- **Typography & Base Styles**:
  - `body`: font-family `'Inter'`, Arial, sans-serif; màu nền `#f4f7fb`, màu chữ `#1e293b`, `line-height: 1.6`.
  - `p`: màu `#334155`, `line-height: 1.7`.
  - `a`: màu `#1d6fa4`, hiệu ứng hover `#0d9488` có gạch chân.
- **Header & Navigation tối màu**:
  - `header`: màu nền `#1a2e5a`, padding `16px 32px`, chữ màu trắng, tiêu đề h1 `1.5rem bold`.
  - Menu điều hướng con `header nav a`: màu `#93c5fd`, `margin-left: 20px`, hiệu ứng hover màu trắng.
- **Layout Main & Box Model Card**:
  - `main`: căn giữa với `max-width: 800px; margin: 0 auto; padding: 32px 16px;`.
  - `.card`: `background: white; padding: 24px; border-radius: 8px; box-shadow: 0 2px 8px rgba(0,0,0,0.1); margin-bottom: 24px;`.
- **Footer**:
  - `footer`: màu nền `#1e293b`, chữ `#94a3b8`, căn giữa, padding `24px 32px`, `margin-top: 48px`, link `footer a` màu `#93c5fd`.
- **Tính năng nâng cao**:
  - Áp dụng class `.highlight` (`background: #fef3c7; padding: 4px 8px; border-radius: 4px;`) vào đoạn văn nổi bật trong `about.html`.
  - Đảm bảo Google Font `'Inter'` được nhúng chính xác vào thẻ `<head>` của cả 3 trang trước file `css/style.css`.

### 4. Lab 3.2: Flexbox Layout (Navbar, Hero Section & Cards Grid)
- **Navbar Flexbox**:
  - `display: flex; justify-content: space-between; align-items: center;`.
  - Logo nằm bên trái, danh sách liên kết `nav-links` nằm bên phải.
- **Hero Section (`section.hero`)**:
  - `display: flex; flex-direction: column; align-items: center; justify-content: center; min-height: 300px;`.
  - Nút kêu gọi hành động `.btn-primary` có hiệu ứng hover đổi màu nền.
- **Cards Grid tự responsive (`.cards-grid`)**:
  - `display: flex; flex-wrap: wrap; gap: 24px;`.
  - Mỗi thẻ `.card` có `flex: 1; min-width: 250px;`, tự động xuống dòng khi màn hình < 800px mà không cần media query.
- **(Nâng cao) Footer Flexbox**:
  - `display: flex; justify-content: space-between;` phân tách 2 cột (thông tin liên hệ bên trái, bản quyền bên phải).

### 5. Lab 3.3: Bố cục CSS Grid Layout (trang `about.html`)
- **Bố cục phân vùng `.page-layout`**:
  - `display: grid;` với 2 cột (`220px 1fr`), 3 hàng (`auto 1fr auto`).
  - Định nghĩa vùng bằng `grid-template-areas`:
    ```text
    "header header"
    "sidebar main"
    "footer footer"
    ```
  - `min-height: 100vh;` đảm bảo phủ kín màn hình, footer tự động neo ở đáy.
- **Thanh bên `<aside class="sidebar">`**:
  - Nền màu `#f1f5f9`, chứa danh sách liên kết nhanh (Quick Links) cuộn đến các phần trong trang.
- **Lưới thẻ kỹ năng `.skills-grid`**:
  - `display: grid; grid-template-columns: repeat(auto-fill, minmax(200px, 1fr)); gap: 16px;`.
  - 5 thẻ kỹ năng (`.skill-card`): HTML5, CSS3 & SCSS, JavaScript, Git & GitHub, Web Design với hiệu ứng hover sinh động.

### 5. Lab 3 - Bài tập 5: Thiết kế Responsive Design (Mobile-First)
- **Mobile Default (< 768px)**:
  - Bố cục 1 cột (`1fr`), `sidebar` tự động ẩn (`display: none;`).
  - Font-size và padding giảm phù hợp với màn hình di động, menu `nav` xếp dọc (`flex-direction: column;`).
  - Lưới kỹ năng `.skills-grid` chuyển thành 1 cột xếp chồng.
  - Đảm bảo không bị lỗi tràn ngang (horizontal scroll).
- **Tablet (≥ 768px)**:
  - Bố cục 2 cột (`180px + 1fr`), `sidebar` hiển thị lại (`display: block;`).
  - Menu `nav` chuyển thành hàng ngang (`flex-direction: row;`).
  - Lưới kỹ năng `.skills-grid` chia thành 2 cột (`repeat(2, 1fr)`).
- **Desktop (≥ 1024px)**:
  - `sidebar` mở rộng thành 240px (`240px + 1fr`).
  - Lưới kỹ năng tự động điều chỉnh nhiều cột (`repeat(auto-fill, minmax(200px, 1fr))`).

### 6. Lab 3.4: Tái cấu trúc sang SCSS (Sass Architecture)
- **Cấu trúc thư mục `scss/` gồm 5 partials + `main.scss`**:
  - `_variables.scss`: Quản lý tập trung biến màu sắc, typography, khoảng cách `$spacing`, `$radius` và `$shadow`.
  - `_reset.scss`: CSS Reset và base typography.
  - `_components.scss`: Mixins tái sử dụng (`@mixin flex-center`, `@mixin card-style`), nút bấm placeholder (`%btn-base`), `.btn-primary` (`@extend`), cùng các thành phần card, form, table.
  - `_layout.scss`: Định nghĩa cấu trúc khung lớn (.navbar, .hero, .cards-grid, .page-layout, .sidebar, footer).
  - `_responsive.scss`: Tập trung toàn bộ media queries cho Tablet (768px), Desktop (1024px) và Landscape.
  - `main.scss`: Import toàn bộ partials theo chuẩn `@use`.
- **Biên dịch tự động**:
  - Biên dịch tự động từ `scss/main.scss` sang `css/style.css` bằng Sass compiler: `sass --watch scss/main.scss:css/style.css`.

---

## 🛠 Hướng dẫn chạy dự án trên VS Code
1. Mở thư mục dự án `my-website` trong **Visual Studio Code**.
2. Cài đặt tiện ích mở rộng **Live Server** (tác giả *Ritwick Dey*).
3. Nhấp chuột phải vào file `index.html` và chọn **Open with Live Server** (hoặc phím tắt `Alt + L, Alt + O`).
4. Trình duyệt mặc định sẽ tự động mở trang web tại địa chỉ `http://127.0.0.1:5500`.