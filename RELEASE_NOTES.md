# Release Notes — BookNest

## v2

- **Tên phiên bản:** BookNest — Góc Đọc & Trao Đổi Sách Sinh Viên
- **Mã phiên bản:** `v2`
- **Ngày cập nhật:** 19/11/2026
- **Trạng thái:** Bản bổ sung tài liệu và ghi nhận kiểm thử, chưa phải bản nộp cuối.

### Nội dung chính

- Ghi nhận bốn ảnh JPG đang có trong `assets/images/` và dùng trong trang: `hero-bookshelf.jpg`, `sach-cong-nghe.jpg`, `sach-ky-nang.jpg`, `sach-van-hoc.jpg`. Theo thông tin chủ dự án cung cấp, nguồn là Unsplash, gồm Đào Việt Hoàng, Yen Vu và Nadiia Shuran. Ánh xạ tác giả và URL gốc cho từng ảnh chưa được xác minh.
- Giao diện HTML5/CSS3 responsive và form tĩnh với trang kết quả mô phỏng `ket-qua.html` hiện có trong source. Form dùng kiểm tra ràng buộc HTML5 và phương thức GET.
- Bổ sung bộ ba tài liệu gốc repository: [README.md](README.md), [AI_LOG.md](AI_LOG.md), [RELEASE_NOTES.md](RELEASE_NOTES.md).

### Lỗi đã xử lý / trạng thái mã hiện tại

- Ảnh các thẻ sách dùng `aspect-ratio: 3 / 2` và `object-fit: cover` để giữ cùng tỷ lệ khung ảnh.
- Liên kết dài trong thẻ dùng `overflow-wrap: anywhere` để hỗ trợ ngắt dòng ở màn hình hẹp như 320px.
- Các quy tắc trên được xác nhận trong mã CSS hiện tại. Lịch sử Git chỉ có một commit gốc; không đủ bằng chứng để xác định chính xác commit hoặc thời điểm các chỉnh sửa CSS này được thực hiện.

### Commit liên quan

- Commit hiện tại tại thời điểm rà soát: `5bf03960ed656de4319683d90e1897266953cf8e` (`first commit`, nhánh `main`).
- Đây là SHA nền đọc từ `git log`; các thay đổi tài liệu `v2` trong workspace chưa nằm trong commit này. Không xem SHA trên là commit phát hành `v2`.

### Hạn chế còn lại

- Đây là website tĩnh thuần HTML5/CSS3. Biểu mẫu chỉ mô phỏng kiểm tra dữ liệu ở trình duyệt; không lưu dữ liệu và không gửi email.
- Chưa xác minh URL GitHub Pages công khai, trạng thái bật Pages, tải tài nguyên HTTP 200, hay giao diện thực tế ở các độ rộng mục tiêu.
- Cần tiếp tục rà soát và kiểm thử trên URL GitHub Pages công khai trong các phiên bản tiếp theo trước khi chốt bản nộp cuối.

### Tiếp tục kiểm tra và bàn giao

1. Đối chiếu mã commit của bản sẽ bàn giao trên repository; không dùng SHA nền nêu trên thay cho commit `v2` nếu chưa commit các thay đổi.
2. Sau khi xác nhận/cấu hình GitHub Pages từ nhánh `main`, thư mục `/(root)`, cập nhật URL công khai vào [README.md](README.md).
3. Mở URL Pages, kiểm tra trang chủ, ảnh và CSS được tải thành công (HTTP 200), rồi thử điều hướng và biểu mẫu bằng dữ liệu giả.
4. Kiểm tra responsive tại 320px, 640px và 960px; xác nhận bảng lịch, ba thẻ sách và luồng GET đến `ket-qua.html`.
5. Đọc chéo [README.md](README.md), [AI_LOG.md](AI_LOG.md) và [RELEASE_NOTES.md](RELEASE_NOTES.md) để xác nhận liên kết, trạng thái kiểm thử và thông tin phiên bản nhất quán.
