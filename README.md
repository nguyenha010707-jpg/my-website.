# My Website - Portfolio Cá Nhân (Lab 1 & Lab 2)

Dự án website cá nhân được xây dựng trong khuôn khổ môn học **Lập trình Web** tại trường **Đại học Gia Định**. Dự án áp dụng chuẩn **HTML5 Semantic**, hệ thống **biểu mẫu & HTML5 Validation**, tối ưu **SEO Onpage**, tiêu chuẩn tiếp cận **Accessibility (WCAG 2.2)** và định kiểu giao diện bằng **CSS3**.

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
├── index.html       # Trang chủ: Giới thiệu chung, hình ảnh dự án Lab 1
├── about.html       # Trang giới thiệu: Thông tin cá nhân, sở thích, mục tiêu, bảng môn học
├── contact.html     # Trang liên hệ: Biểu mẫu liên hệ với HTML5 Validation chuẩn
│
├── css/
│   └── style.css    # CSS định dạng giao diện, Box Model, Reset CSS, Card & Form Styling
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

### 2. Lab 2 - Bài tập 03: Biểu mẫu HTML5 & Validation thuần
- Form liên hệ hoàn chỉnh trong `contact.html` với cấu trúc chuẩn:
  - Thẻ `<form action="#" method="POST">`.
  - **Fieldset 1 – Thông tin cá nhân**:
    - Họ và tên (`text`, `required`, `minlength="2"`, `maxlength="100"`).
    - Email (`email`, `required`, placeholder gợi ý).
    - Số điện thoại (`tel`, `pattern="[0-9]{10,11}"`, tooltip báo lỗi với `title`).
    - *Tính năng nâng cao*: Ô chọn Ngày sinh (`type="date"`).
    - *Tính năng nâng cao*: Gợi ý trường đại học qua thẻ `<datalist>` với các lựa chọn tiêu biểu.
  - **Fieldset 2 – Nội dung liên hệ**:
    - Chọn chủ đề liên hệ với `<select>` và các `<option>`.
    - Lựa chọn kênh ưu tiên liên hệ (Email / Điện thoại / Zalo) dạng radio buttons nằm trong `<fieldset>` con.
    - Ô nhập tin nhắn (`<textarea>`, `rows="5"`, `required`, `minlength="10"`, `maxlength="500"`).
    - Checkbox xác nhận đồng ý điều khoản sử dụng (`required`).
  - Nút bấm điều khiển:
    - `<button type="submit">`: Gửi tin nhắn và kích hoạt HTML5 Validation.
    - `<button type="reset">`: Xoá và đưa biểu mẫu về trạng thái ban đầu.

### 3. Lab 2 - Bài tập 04: SEO, Accessibility & Open Graph Metadata
- **Thẻ `<title>`**: Đạt chuẩn độ dài từ 50–60 ký tự, chứa tên sinh viên và từ khoá chính:
  - Trang chủ: `Huỳnh Nguyễn Hà – Portfolio Cá Nhân | Đại Học Gia Định` (54 ký tự).
  - Trang giới thiệu: `Huỳnh Nguyễn Hà – Giới Thiệu Bản Thân | ĐH Gia Định` (51 ký tự).
  - Trang liên hệ: `Huỳnh Nguyễn Hà – Liên Hệ Trực Tiếp | Đại Học Gia Định` (54 ký tự).
- **Thẻ `<meta name="description">`**: Đạt chuẩn độ dài từ 150–160 ký tự, mở đầu bằng động từ hành động mô tả nội dung trang:
  - Trang chủ: 159 ký tự (bắt đầu bằng *"Khám phá..."*).
  - Trang giới thiệu: 160 ký tự (bắt đầu bằng *"Tìm hiểu..."*).
  - Trang liên hệ: 156 ký tự (bắt đầu bằng *"Liên hệ..."*).
- **Thẻ Open Graph (`og:title`, `og:description`, `og:type`, `og:url`)**: Hỗ trợ hiển thị card preview đẹp mắt khi chia sẻ liên kết trên Facebook, Zalo, LinkedIn.
- **Tiêu chuẩn Accessibility (WCAG 2.2)**:
  - Quy tắc bắt buộc `label[for]` khớp chính xác với `input[id]` cho tất cả các trường nhập liệu trong biểu mẫu.
  - Mỗi trang có duy nhất 1 thẻ `<h1>` chính, phân cấp heading mạch lạc (`<h1>` -> `<h2>`).
  - Toàn bộ hình ảnh `<img>` đều có thuộc tính `alt` mô tả nội dung trực quan, rõ nghĩa.
  - Các phần tử form, liên kết và button có thể điều hướng mượt mà bằng bàn phím (Tab key).

---

## 🛠 Hướng dẫn chạy dự án trên VS Code
1. Mở thư mục dự án `my-website` trong **Visual Studio Code**.
2. Cài đặt tiện ích mở rộng **Live Server** (tác giả *Ritwick Dey*).
3. Nhấp chuột phải vào file `index.html` và chọn **Open with Live Server** (hoặc phím tắt `Alt + L, Alt + O`).
4. Trình duyệt mặc định sẽ tự động mở trang web tại địa chỉ `http://127.0.0.1:5500`.