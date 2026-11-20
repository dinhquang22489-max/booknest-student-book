# BookNest — Góc Đọc & Trao Đổi Sách Sinh Viên

**Tác giả:** Đinh Nhật Quang — **MSV:** 2071020158

BookNest là website tĩnh giới thiệu tủ sách dùng chung cho sinh viên: xem các nhóm sách gợi ý, lịch mở tủ sách và gửi biểu mẫu mô phỏng đăng ký mượn hoặc góp sách.

## Liên kết

- **Repository:** [github.com/dinhquang22489-max/booknest-student-book](https://github.com/dinhquang22489-max/booknest-student-book)
- **GitHub Pages:** [booknest-student-book](https://dinhquang22489-max.github.io/booknest-student-book/)

## Hồ sơ bàn giao

- [README.md](README.md) — hướng dẫn sử dụng và kiểm tra.
- [CHANGELOG.md](CHANGELOG.md) — lịch sử các phiên bản `v3` đến `v1`.
- [docs/evidence-index.md](docs/evidence-index.md) — phép thử và minh chứng.
- [AI_LOG.md](AI_LOG.md) — nhật ký sử dụng AI.
- [RELEASE_NOTES.md](RELEASE_NOTES.md) — ghi chú phát hành hiện tại.

## Cấu trúc dự án

```text
booknest-student-book/
├── README.md
├── CHANGELOG.md
├── AI_LOG.md
├── RELEASE_NOTES.md
├── docs/
│   └── evidence-index.md
├── index.html
├── ket-qua.html
├── css/
│   └── style.css
└── assets/
    └── images/
        ├── hero-bookshelf.jpg
        ├── sach-cong-nghe.jpg
        ├── sach-ky-nang.jpg
        └── sach-van-hoc.jpg
```

## Chạy trên máy local

1. Tải hoặc clone repository.
2. Mở `index.html` trực tiếp trong trình duyệt; hoặc mở thư mục dự án bằng VS Code và chạy `index.html` qua tiện ích Live Server.
3. Nếu gửi biểu mẫu bằng phương thức GET, trình duyệt sẽ điều hướng đến `ket-qua.html` và các trường có thể xuất hiện trong query string. Chỉ dùng dữ liệu giả khi thử.

## Kiểm tra trang và chức năng

Đã kiểm tra trên GitHub Pages công khai ngày 21/11/2026:

1. Ở 320px, trang không tràn ngang; menu hiển thị và bảng cuộn ngang bên trong `.table-wrap`.
2. Lưới thẻ sách có một cột ở 320px, hai cột ở 640px và ba cột ở 960px; ảnh trong từng hàng có chiều cao đồng đều.
3. Biểu mẫu chặn trường bắt buộc để trống và email sai định dạng (`:user-invalid`); dữ liệu kiểm thử hợp lệ được chuyển bằng GET đến `ket-qua.html`.
4. Dùng `Tab` và `Shift + Tab` cho thấy viền `:focus-visible` rõ trên phần tử đang nhận focus.
5. Tài liệu trang chủ, CSS và bốn ảnh JPG trả về HTTP `200` khi tải từ GitHub Pages.

Chi tiết số đo và giới hạn minh chứng ảnh chụp được ghi trong [docs/evidence-index.md](docs/evidence-index.md).

## Ảnh và nguồn

Thư mục `assets/images/` hiện có bốn ảnh JPG được dùng trong trang: ảnh kệ sách (`hero-bookshelf.jpg`) và ba ảnh cho các nhóm sách (`sach-cong-nghe.jpg`, `sach-ky-nang.jpg`, `sach-van-hoc.jpg`). Thông tin nguồn do chủ dự án cung cấp: **Unsplash**, các nhiếp ảnh gia **Đào Việt Hoàng, Yen Vu và Nadiia Shuran**. Repository hiện không ghi URL ảnh gốc hoặc ánh xạ từng ảnh đến từng nhiếp ảnh gia; thông tin đối chiếu theo từng tệp: **[Chưa kiểm tra]**.