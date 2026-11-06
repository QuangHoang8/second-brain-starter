# Elasticsearch Mentor

AI mentor cá nhân để học Elasticsearch (kiến thức, best practice, tối ưu hiệu năng và dung lượng), xây trên Obsidian + Markdown + AI. Thuần học và thực hành, **không có phần chứng chỉ**.

## Mục tiêu

- Học theo lộ trình có cấu trúc, từ khái niệm nền tảng đến vận hành production.
- Luyện câu hỏi để củng cố kiến thức, theo dõi mức tự tin và reasoning.
- Ghi lại câu sai và insight để ôn lại.
- Thực hành trên môi trường ES thật (Kibana Dev Tools) và ghi benchmark trước/sau cho các thay đổi tuning.
- Kiến thức đã kiểm chứng được lưu ở `04-Knowledge/Elasticsearch/` để dùng chung với phần còn lại của second brain.

## Phiên bản mục tiêu

Elasticsearch **9.x**. Hành vi, API và giá trị mặc định có thể khác 7.x/8.x: mọi chi tiết đặc thù phiên bản phải được đối chiếu với tài liệu chính thức của Elastic cho 9.x trước khi ghi vào note.

## Nguồn lộ trình

Stage 01-11 lấy từ roadmap.sh: https://roadmap.sh/elasticsearch (truy cập 2026-11-06; nhóm node theo stage là suy luận từ thứ tự node trên trang, xem `Roadmap.md`).

Stage 12 (Performance & Storage Tuning) **do người dùng và AI bổ sung, không thuộc roadmap.sh**; nguồn chính là tài liệu Elastic về tune for disk usage / search speed / indexing speed.

## Cấu trúc

```text
Elasticsearch-Mentor/
├── README.md
├── Roadmap.md          # 12 stage + checkbox tiến độ
├── Questions/          # câu hỏi, lọc theo field `stage`
├── Sessions/           # log phiên học (nơi lưu session duy nhất)
├── Mistakes/
├── Insights/
├── Benchmarks/         # đo trước/sau cho tuning
└── Strategies/STRATEGY-LOG.md
```

Cấu trúc phẳng: mỗi note có field `stage` (ví dụ `05-how-search-works`) thay vì thư mục con theo stage.

## Danh sách stage

| stage | Tên |
|---|---|
| 01-introduction | Introduction |
| 02-core-architecture | Core Architecture |
| 03-data-modelling | Data Modelling |
| 04-data-ingestion | Data Ingestion |
| 05-how-search-works | How Search Works |
| 06-text-analysis | Text Analysis |
| 07-aggregations | Aggregations |
| 08-relevance-tuning | Relevance & Tuning |
| 09-production | Production |
| 10-security | Security |
| 11-vector-ai-search | Vector / AI Search |
| 12-performance-storage-tuning | Performance & Storage Tuning (bổ sung) |

## Cách dùng nhanh

1. Đọc `08-AI/Elasticsearch-Mentor/Rules/Mentor-Rules.md`.
2. Mở `Roadmap.md`, chọn stage đang học.
3. Mỗi lần học/luyện, dùng `08-AI/Prompts/Elasticsearch-Mentor/Start-Training.md`.
4. Mỗi lần thực hành tuning, đọc `Benchmark-Rules.md` rồi dùng `Start-Benchmark.md`.
5. Sau phiên, tạo session từ `templates/Elasticsearch-Mentor/SESSION.md`, rồi chạy `Analyze-Session.md`.
6. Câu sai quan trọng: `templates/Elasticsearch-Mentor/MISTAKE.md`.
7. Định kỳ chạy `Weekly-Review.md`.

## Quy tắc vận hành

AI không được coi một factual claim về hành vi/giới hạn/mặc định của Elasticsearch là "verified" nếu chưa có nguồn tài liệu Elastic chính thức (đúng phiên bản 9.x) hoặc chưa được người dùng xác nhận.

Automation mặc định là semi-automatic: AI đề xuất thay đổi knowledge/mistake; người dùng duyệt trước khi ghi chính thức.

Không ghi secrets (API key, mật khẩu, hostname/URL nội bộ, dữ liệu thật của khách hàng hay công ty) vào bất kỳ file nào, xem `Benchmark-Rules.md`.
