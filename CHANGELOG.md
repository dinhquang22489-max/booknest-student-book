# Changelog — BookNest

Lịch sử thay đổi từ mới nhất đến cũ nhất.

## v3 (Release Note bản bàn giao cuối — 21/11/2026)

### Thay đổi chính

- Bổ sung `CHANGELOG.md` và [docs/evidence-index.md](docs/evidence-index.md), đồng bộ toàn bộ liên kết tài liệu và đối chiếu phiên bản triển khai GitHub Pages: [dinhquang22489-max.github.io/booknest-student-book](https://dinhquang22489-max.github.io/booknest-student-book/).
- Cập nhật [README.md](README.md), [AI_LOG.md](AI_LOG.md) và [RELEASE_NOTES.md](RELEASE_NOTES.md) lên mốc `v3`.

### Lỗi đã sửa

- Đồng bộ liên kết GitHub Pages trong `README.md` (commit `3bd310f`).
- Chuẩn hóa tỉ lệ khung ảnh card (`aspect-ratio: 3 / 2; object-fit: cover`) và xử lý ngắt dòng URL dài (`overflow-wrap: anywhere`) để chống tràn ngang ở `320px`.

### Hạn chế còn lại

- Website tĩnh thuần HTML5/CSS3 nên biểu mẫu chỉ mô phỏng kiểm tra dữ liệu phía trình duyệt (`ket-qua.html`), chưa lưu trữ dữ liệu hay gửi email thật.

## v2

- Tích hợp bốn ảnh thực tế từ Unsplash vào `assets/images/`.
- Hoàn thiện giao diện responsive và tạo bộ ba tài liệu `README.md`, `AI_LOG.md`, `RELEASE_NOTES.md`.

## v1 (first commit)

- Khởi tạo khung HTML5 semantic (`index.html`, `ket-qua.html`) và CSS3 Mobile-First (`css/style.css`).
