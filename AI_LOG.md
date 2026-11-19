# AI_LOG.md — Nhật ký sử dụng AI

Tài liệu này ghi nhận các tình huống trong lượt rà soát và soạn tài liệu `v2` hiện tại. Lịch sử trước đó không được cung cấp; nội dung dưới đây không khẳng định các trao đổi AI trước phiên này. Những kiểm tra chưa chạy được đánh dấu rõ, không suy diễn thành kết quả.

## Tình huống 1 — Đối chiếu nguồn bốn ảnh Unsplash

- **Hiện tượng và dữ kiện ban đầu:** `assets/images/` có bốn tệp JPG: `hero-bookshelf.jpg`, `sach-cong-nghe.jpg`, `sach-ky-nang.jpg`, `sach-van-hoc.jpg`. Yêu cầu của chủ dự án nêu nguồn Unsplash và tên Đào Việt Hoàng, Yen Vu, Nadiia Shuran. Mã nguồn và lịch sử Git hiện có không chỉ ra URL trang ảnh gốc hay ánh xạ tên nhiếp ảnh gia cho từng tệp.
- **Nhận định trước AI:** Có thể ghi nhận nguồn và các tên được cung cấp, nhưng không nên tự gán tên cho từng ảnh hoặc dựng URL ảnh gốc khi thiếu dữ kiện.
- **Công cụ / prompt hoặc phản hồi mẫu đã dùng:** Hỗ trợ AI trong phiên này rà soát cấu trúc dự án và các ảnh có trong workspace; yêu cầu của chủ dự án: “kèm ghi nguồn 4 ảnh Unsplash (Đào Việt Hoàng, Yen Vu, Nadiia Shuran)”.
- **Gợi ý nhận được:** Liệt kê bốn tên tệp thực tế, ghi nguồn/tên theo thông tin được cung cấp và nêu rõ chưa xác minh ánh xạ theo ảnh.
- **Quyết định của sinh viên:** Theo yêu cầu của chủ dự án, ghi nguồn ở mức thông tin hiện có; không gán từng nhiếp ảnh gia cho từng tệp vì không có bằng chứng trong repository.
- **Phần sinh viên tự sửa trong mã nguồn / tài liệu:** Không ghi nhận chỉnh sửa độc lập nào của sinh viên trong phiên này. Trợ lý AI soạn mục nguồn ảnh trong `README.md` và ghi rõ giới hạn xác minh; chủ dự án cần rà soát nội dung.
- **Cách thử lại và kết quả thực tế:** Đã đối chiếu bốn tên tệp trong thư mục ảnh và các đường dẫn ảnh trong `index.html`. Đối chiếu trang Unsplash gốc, URL nguồn và tác giả tương ứng với từng tệp: **[Chưa kiểm tra]**.

## Tình huống 2 — Rà soát semantic HTML5 và responsive

- **Hiện tượng và dữ kiện ban đầu:** `index.html` có cấu trúc `header`, `nav`, `main`, `section`, `article`, `table` và `form`; `css/style.css` có media query tại `640px` và `960px`. Mã CSS đặt ảnh thẻ sách ở `aspect-ratio: 3 / 2` và `object-fit: cover`, đồng thời đặt `overflow-wrap: anywhere` cho liên kết thẻ sách.
- **Nhận định trước AI:** Mã nguồn biểu thị bố cục một cột mặc định, hai cột từ 640px, ba cột từ 960px; đọc mã chưa đủ để kết luận giao diện đã được kiểm thử trên trình duyệt ở các kích thước cụ thể.
- **Công cụ / prompt hoặc phản hồi mẫu đã dùng:** Hỗ trợ AI rà soát trực tiếp `index.html` và `css/style.css`; yêu cầu của chủ dự án: “kiểm tra cấu trúc HTML5 semantic & breakpoint responsive `640px`/`960px`”.
- **Gợi ý nhận được:** Hướng dẫn kiểm tra ba ngưỡng 320px, 640px, 960px; kiểm tra điều hướng, bảng cuộn ngang và các ràng buộc form HTML5. Phân biệt dữ kiện đọc từ mã với kết quả chạy trình duyệt.
- **Quyết định của sinh viên:** Theo yêu cầu của chủ dự án, đưa các bước kiểm tra vào README; không sửa mã hiện có vì các thuộc tính/breakpoint liên quan đã có trong source.
- **Phần sinh viên tự sửa trong mã nguồn / tài liệu:** Không ghi nhận chỉnh sửa độc lập nào của sinh viên trong phiên này. Trợ lý AI không thay đổi HTML/CSS và soạn hướng dẫn responsive, kiểm thử biểu mẫu trong `README.md`; kiểm thử trình duyệt được ghi là chưa xác nhận.
- **Cách thử lại và kết quả thực tế:** Đã đọc source để xác nhận breakpoint 640px/960px, form `action="ket-qua.html" method="get"` và các thuộc tính validation. Chạy trình duyệt tại 320px/640px/960px, xác nhận không tràn ngang và xác nhận luồng gửi form: **[Chưa kiểm tra]**.

## Tình huống 3 — Soạn đồng bộ bộ tài liệu `v2`

- **Hiện tượng và dữ kiện ban đầu:** `README.md` tồn tại nhưng rỗng; `AI_LOG.md` và `RELEASE_NOTES.md` chưa có. Git remote là `https://github.com/dinhquang22489-max/booknest-student-book.git`; nhánh hiện tại là `main`, HEAD trước thay đổi là `5bf03960ed656de4319683d90e1897266953cf8e`. Workspace chưa cung cấp trạng thái cấu hình Pages hay thư mục minh chứng.
- **Nhận định trước AI:** Có thể ghi tên repository, cây thư mục, mã SHA hiện tại và những gì đọc trực tiếp từ source. Không thể kết luận Pages đã xuất bản, cũng không thể gọi SHA đầu vào là commit chứa tài liệu `v2` mới.
- **Công cụ / prompt hoặc phản hồi mẫu đã dùng:** Hỗ trợ AI rà soát mã nguồn, cây thư mục và Git; yêu cầu của chủ dự án: “tạo mới hoặc cập nhật đồng bộ 3 tệp tài liệu ở thư mục gốc repository cho mốc phiên bản `v2`”.
- **Gợi ý nhận được:** Tạo README hướng dẫn mở/kiểm tra website, nhật ký AI nêu quyết định và kiểm thử có căn cứ, cùng ghi chú phát hành có giới hạn rõ ràng; dùng placeholder cho URL Pages chưa xác minh.
- **Quyết định của sinh viên:** Theo yêu cầu của chủ dự án, tạo/cập nhật ba tài liệu. Ghi SHA là commit nền tại thời điểm rà soát và nói rõ tài liệu mới chưa nằm trong commit đó; để placeholder Pages vì chưa xác minh trạng thái xuất bản.
- **Phần sinh viên tự sửa trong mã nguồn / tài liệu:** Không ghi nhận chỉnh sửa độc lập nào của sinh viên trong phiên này. Trợ lý AI soạn `README.md`, `AI_LOG.md` và `RELEASE_NOTES.md` theo dữ kiện đã kiểm tra; chủ dự án cần rà soát trước khi bàn giao.
- **Cách thử lại và kết quả thực tế:** Đã đọc `index.html`, `ket-qua.html`, `css/style.css`, cây thư mục, remote và log Git. Kiểm tra chéo ba tài liệu sau khi tạo: **[Chưa kiểm tra]**. Kiểm tra URL Pages công khai/tài nguyên HTTP 200: **[Chưa kiểm tra]**.
