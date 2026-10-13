# INS2053 - Soạn thảo và Quản trị Web (VNU-IS)

Dự án bài tập môn học **INS2053 - Web Authoring & Web Management**.

## Cấu trúc Repository

```text
├── homework/
│   └── submissions.md          # Danh sách link Google Drive nộp video OBS
├── project/
│   ├── css/
│   │   └── style.css           # 1 Stylesheet chung toàn site (Buổi 4, 5, 6)
│   ├── images/
│   │   ├── hero-banner.svg     # Banner giới thiệu CLB trên trang chủ
│   │   ├── coding-workshop.svg # Ảnh minh họa workshop lập trình
│   │   ├── meeting.svg         # Hình ảnh minh họa sinh hoạt CLB (trang About)
│   │   └── contact-map.svg     # Sơ đồ vị trí phòng sinh hoạt (trang Contact)
│   ├── index.html              # Trang chủ đầy đủ các phần, Event Cards & hình ảnh (Buổi 6)
│   ├── about.html              # Trang giới thiệu, bảng ban chủ nhiệm (Buổi 4, 6)
│   └── contact.html            # Trang liên hệ, kênh thông tin, sơ đồ & biểu mẫu (Buổi 6)
└── README.md                   # Hướng dẫn dự án
```

## Nội dung bài tập đã hoàn thành

### 1. Bài tập Buổi 04: Trang trí bằng External CSS
- Tạo stylesheet ngoài `project/css/style.css` và liên kết tới các trang bằng thẻ `<link>`.
- Định dạng nền tảng: `body` có màu nền, màu chữ tương phản, `font-family` và giãn dòng `line-height: 1.6`.
- Phân cấp rõ rệt 3 cấp đề mục: `h1`, `h2` (xanh royal), `h3` (cam đất).
- Định dạng hình ảnh `img` với `max-width: 100%`, bo góc `border-radius: 8px` và viền nhẹ.
- Định dạng danh sách có thứ tự `<ol>` và không thứ tự `<ul>`.

### 2. Bài tập Buổi 05: Bố cục trang với HTML ngữ nghĩa
- Dựng bố cục chuẩn HTML5 ngữ nghĩa:
  - `<header>`: Tiêu đề và tagline câu lạc bộ.
  - `<nav>`: Menu điều hướng ngang hiển thị bằng Flexbox (`Home`, `About`, `Contact`).
  - `<main>`: Vùng nội dung chính giới hạn `max-width: 860px`, căn giữa màn hình (`margin: auto`).
  - `<footer>`: Vùng chân trang với màu nền tối phân biệt, thông tin bản quyền và trường học.
- Reset khoảng cách viền lề `* { box-sizing: border-box; margin: 0; padding: 0; }`.

### 3. Bài tập Buổi 06: Xây mini-site 3 trang với điều hướng nhất quán
- **Bố cục nhất quán:** Cả 3 trang (`index.html`, `about.html`, `contact.html`) dùng chung cấu trúc `<header>`, `<nav>`, `<footer>`, `<main>` và liên kết đến cùng 1 file `css/style.css`.
- **Menu điều hướng:** Đường dẫn tương đối chuẩn xác (`index.html`, `about.html`, `contact.html`), di chuyển class `active` tương ứng trên từng trang để làm nổi bật vị trí người dùng đang xem.
- **Trang Contact hoàn thiện:** Có thông tin liên hệ, kênh hỗ trợ, địa chỉ/thời gian sinh hoạt, ảnh bản đồ phòng lab và form gửi tin nhắn (áp dụng từ bài học Buổi 6).
- **Trang chủ phong phú:** Gồm phần Chào mừng, Hoạt động (What We Do), 3 Lợi ích (Why Join Us?), 2 ảnh minh họa vector sắc nét và khối sự kiện sắp diễn ra (Event Cards với đường viền nhấn bên trái).
- **Trang About:** Bổ sung bảng thành viên ban điều hành (Data Table) theo chuẩn bài học.

## Hướng dẫn nộp bài
1. Mở file `homework/submissions.md`, điền Họ tên và MSSV.
2. Quay video 1–2 phút bằng OBS Studio giải thích code cho từng buổi, upload lên Google Drive (chế độ Public/Viewer), dán link vào file `homework/submissions.md`.
3. Chạy `git add .`, `git commit -m "HW6: Complete 3-page mini-site with navigation"` và `git push` lên GitHub.
