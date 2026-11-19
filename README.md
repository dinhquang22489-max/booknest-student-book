# BookNest — Góc Đọc & Trao Đổi Sách Sinh Viên

**Tác giả:** Đinh Nhật Quang — **MSV:** 2071020158

BookNest là website tĩnh giới thiệu tủ sách dùng chung cho sinh viên: xem các nhóm sách gợi ý, lịch mở tủ sách và gửi biểu mẫu mô phỏng đăng ký mượn hoặc góp sách.

## Liên kết

- **Repository:** [github.com/dinhquang22489-max/booknest-student-book](https://github.com/dinhquang22489-max/booknest-student-book)
- **GitHub Pages:** [dinhquang22489-max.github.io/booknest-student-book/](https://dinhquang22489-max.github.io/booknest-student-book)
## Cấu trúc dự án

```text
booknest-student-book/
├── README.md
├── AI_LOG.md
├── RELEASE_NOTES.md
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

1. Mở `index.html`, xem phần giới thiệu và dùng thanh điều hướng để đến **Giới thiệu**, **Kệ sách gợi ý**, **Lịch trao đổi** và **Đăng ký mượn**.
2. Kiểm tra ba thẻ sách khi thay đổi chiều rộng cửa sổ:
   - **320px:** một cột; kiểm tra không tràn ngang. Bảng lịch nằm trong vùng cuộn ngang riêng.
   - **640px:** breakpoint chuyển thẻ sách sang hai cột.
   - **960px trở lên:** breakpoint chuyển thẻ sách sang ba cột.
3. Kiểm tra bảng lịch trao đổi: có ba hoạt động và trên màn hình hẹp có thể cuộn bảng theo chiều ngang.
4. Để thử biểu mẫu, nhập thông tin giả hợp lệ (tên từ 2 đến 80 ký tự, email đúng định dạng, nội dung từ 10 đến 500 ký tự), rồi chọn **Kiểm tra biểu mẫu**. Trình duyệt kiểm tra các ràng buộc HTML5 (`required`, `type="email"`, `minlength`, `maxlength`) trước khi chuyển bằng GET đến `ket-qua.html`. Thử bỏ trống hoặc nhập sai định dạng để thấy kiểm tra phía trình duyệt chặn gửi.
5. Trang kết quả chỉ mô phỏng trạng thái hợp lệ; không lưu dữ liệu và không gửi email.

Các breakpoint và ràng buộc trên được đọc từ mã nguồn; việc kiểm tra giao diện thực tế ở các kích thước và trên URL Pages công khai chưa được xác nhận trong tài liệu này.

## Ảnh và nguồn

Thư mục `assets/images/` hiện có bốn ảnh JPG được dùng trong trang: ảnh kệ sách (`hero-bookshelf.jpg`) và ba ảnh cho các nhóm sách (`sach-cong-nghe.jpg`, `sach-ky-nang.jpg`, `sach-van-hoc.jpg`). Thông tin nguồn do chủ dự án cung cấp: **Unsplash**, các nhiếp ảnh gia **Đào Việt Hoàng, Yen Vu và Nadiia Shuran**. Repository hiện không ghi URL ảnh gốc hoặc ánh xạ từng ảnh đến từng nhiếp ảnh gia; thông tin đối chiếu theo từng tệp: **[Chưa kiểm tra]**.

## Hồ sơ và minh chứng

- [AI_LOG.md](AI_LOG.md) — ghi nhận các tình huống dùng AI, quyết định và trạng thái kiểm thử.
- [RELEASE_NOTES.md](RELEASE_NOTES.md) — ghi chú phiên bản `v2`.
- **Thư mục minh chứng:** chưa có trong cấu trúc repository hiện tại.
