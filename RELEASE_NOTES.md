# Release Notes — BookNest v3

**Tên phiên bản:** BookNest — Góc Đọc & Trao Đổi Sách Sinh Viên; **Mã phiên bản:** `v3`; **Ngày:** 21/11/2026; **Tác giả:** Đinh Nhật Quang — **MSV:** 2071020158

## Thay đổi

- Hoàn thiện hồ sơ bàn giao với [CHANGELOG.md](CHANGELOG.md) và [docs/evidence-index.md](docs/evidence-index.md).
- Đồng bộ [README.md](README.md), [AI_LOG.md](AI_LOG.md) và tài liệu phát hành với URL repository [dinhquang22489-max/booknest-student-book](https://github.com/dinhquang22489-max/booknest-student-book) và GitHub Pages [booknest-student-book](https://dinhquang22489-max.github.io/booknest-student-book/).
- Ghi nhận chuẩn khung ảnh card `aspect-ratio: 3 / 2; object-fit: cover` và ngắt URL dài bằng `overflow-wrap: anywhere`.

## Kiểm tra đã thực hiện

Trên GitHub Pages công khai:

- `320px`: không tràn ngang; vùng bảng cuộn ngang nội bộ.
- `640px` và `960px`: lưới lần lượt có 2 và 3 cột; ảnh card đồng đều chiều cao.
- Form chặn dữ liệu trống/email sai và gửi dữ liệu kiểm thử giả hợp lệ qua GET tới `ket-qua.html`.
- `Tab` / `Shift + Tab` hiển thị viền `:focus-visible`.
- Trang chủ, `css/style.css` và bốn ảnh JPG đều tải với HTTP `200`.

Chi tiết kết quả và placeholder ảnh chụp trong trường hợp chưa có tệp nằm tại [docs/evidence-index.md](docs/evidence-index.md). Changelog các phiên bản trước: [CHANGELOG.md](CHANGELOG.md).

## Hạn chế

Đây là website tĩnh thuần HTML5/CSS3. Form chỉ mô phỏng kiểm tra dữ liệu phía trình duyệt và hiển thị `ket-qua.html`; website chưa lưu dữ liệu hoặc gửi email thật. Workspace chưa có ảnh chụp trong `evidence/`; sinh viên cần tự chụp và điền đường dẫn minh chứng sau.
