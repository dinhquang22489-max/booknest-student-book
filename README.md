# BookNest — Góc Đọc & Trao Đổi Sách Sinh Viên

## Sản phẩm này là gì?
Website tĩnh giới thiệu góc đọc sách, danh mục sách gợi ý và lịch trao đổi sách miễn phí dành cho sinh viên năm nhất. Tác giả: Đinh Nhật Quang — MSV: 2071020158.

## Demo
https://dinhquang22489-max.github.io/booknest-student-book/

## Tính năng
- Bấm `Giới thiệu`, `Kệ sách gợi ý`, `Lịch trao đổi` hoặc `Đăng ký mượn` trên thanh điều hướng để cuộn tới nội dung tương ứng.
- Xem ba nhóm sách gợi ý (Kỹ năng học tập, Tư duy công nghệ, Văn học & Tản văn) kèm ảnh minh họa và bảng lịch mở tủ sách hằng tuần.
- Điền biểu mẫu rồi bấm **Kiểm tra biểu mẫu** để kiểm tra HTML5 và chuyển tới trang kết quả mô phỏng `ket-qua.html`.

## Cách mở
1. Mở URL ở mục **Demo** bằng trình duyệt, hoặc mở `index.html` trên máy cá nhân.
2. Bấm **Kệ sách gợi ý** trên thanh menu để xem ba nhóm sách.
3. Bấm **Lịch trao đổi** để xem thời gian và địa điểm mở tủ sách.
4. Bấm **Đăng ký mượn**, nhập các trường **Họ và tên người mượn**, **Email liên hệ**, **Tên sách muốn mượn & ngày nhận dự kiến**, rồi bấm **Kiểm tra biểu mẫu**.

## Cấu trúc thư mục
- `index.html`: Trang chủ BookNest.
- `ket-qua.html`: Trang kết quả mô phỏng sau khi kiểm tra biểu mẫu.
- `css/style.css`: Giao diện Flexbox, CSS Grid và Responsive Mobile-First.
- `assets/images/`: Bốn ảnh `hero-bookshelf.jpg`, `sach-ky-nang.jpg`, `sach-cong-nghe.jpg`, `sach-van-hoc.jpg`.
- `docs/evidence-index.md`: Bảng minh chứng kiểm thử; `evidence/`: ảnh chụp minh chứng.
- `CHANGELOG.md`, `docs/AI_LOG.md`, `RELEASE_NOTES.md`: Lịch sử phiên bản, nhật ký AI và ghi chú phát hành.

## Đã kiểm tra
Xem [docs/evidence-index.md](docs/evidence-index.md): đã kiểm tra GitHub Pages, bấm đủ bốn mục menu, thử responsive tại `320px`, `640px`, `960px` và kiểm tra form hợp lệ/không hợp lệ.

## Hạn chế / Chưa kiểm tra
- Website tĩnh HTML5/CSS3; biểu mẫu chỉ kiểm tra dữ liệu phía trình duyệt, chưa lưu vào cơ sở dữ liệu hoặc gửi email.
- Chưa kiểm thử trên iPhone vật lý; responsive được kiểm tra bằng Playwright trên trình duyệt.

## Khai báo AI & Nguồn tài nguyên
- Nhật ký sử dụng AI và tự kiểm chứng: [AI_LOG.md](docs/AI_LOG.md).
- Ảnh từ Unsplash (Unsplash License): `hero-bookshelf.jpg` (Đào Việt Hoàng), `sach-ky-nang.jpg` và `sach-cong-nghe.jpg` (Yen Vu), `sach-van-hoc.jpg` (Nadiia Shuran).
