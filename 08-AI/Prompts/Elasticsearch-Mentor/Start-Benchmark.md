# Start Benchmark — Elasticsearch Mentor

Đọc trước:
- `08-AI/Elasticsearch-Mentor/Rules/Benchmark-Rules.md` (bắt buộc: an toàn, cách đo, secrets)
- `02-Projects/Elasticsearch-Mentor/Roadmap.md`, mục stage 12 và stage liên quan

Xác nhận với người dùng trước khi bắt đầu:
- Mục tiêu đo là gì (dung lượng, indexing speed, search latency...) và **một** biến sẽ thay đổi.
- Cluster đang dùng là gì (local/dev hay dùng chung); có chạy được trên index tạm không.
- Phiên bản ES (kỳ vọng 9.x).

Trong lúc đo:
- Hướng dẫn từng bước trên Kibana Dev Tools; cảnh báo trước lệnh nặng hoặc phá hủy.
- Đo trước, thay đổi một biến, đo sau; lặp lại để biết độ biến thiên.
- Không yêu cầu hay lưu API key, hostname, dữ liệu thật; dùng dữ liệu giả và placeholder.
- Kiểm tra tên API/tham số với tài liệu Elastic 9.x nếu không chắc.

Sau khi đo:
- Nhắc xoá index tạm và hoàn tác setting đã đổi.
- Tạo benchmark note từ `templates/Elasticsearch-Mentor/BENCHMARK.md` với `verified: false`.
- Đề xuất knowledge note mới trong `04-Knowledge/Elasticsearch/` nếu có kết luận đáng lưu (chờ người dùng duyệt).
