# Question Rules — Elasticsearch Mentor

## Stage

Câu hỏi thuộc một trong 12 stage trong `02-Projects/Elasticsearch-Mentor/Roadmap.md` (field `stage`, ví dụ `05-how-search-works`).

## Response types

- **multiple-choice**: 1 đáp án đúng, 3 distractor.
- **multiple-response**: ≥2 đáp án đúng trên ≥5 lựa chọn.
- **hands-on**: yêu cầu chạy lệnh trên Kibana Dev Tools và quan sát kết quả (dùng index tạm).

## Question types

- knowledge: nhớ khái niệm/hành vi
- scenario: chọn mapping/query/kiến trúc phù hợp cho tình huống
- best-practice-selection: nhiều cách chạy được nhưng một cách đúng best practice
- troubleshooting: tìm nguyên nhân (query chậm, shard unassigned, mapping explosion...)
- calculation: ước lượng dung lượng, số shard, throughput đơn giản

## Distractor pattern cần luyện nhận diện

Đây là kinh nghiệm học tập, **không phải tài liệu chính thức Elastic**:

- wrong_feature: dùng tính năng không phù hợp (vd `nested` khi `object`/`flattened` đủ dùng)
- right_feature_wrong_config: đúng tính năng nhưng cấu hình sai
- query_vs_filter_confusion: dùng query context khi chỉ cần filter (không cần scoring)
- text_vs_keyword_confusion: nhầm field `text` và `keyword`
- ignores_stated_constraint: bỏ qua ràng buộc đề nêu (dung lượng, độ trễ, throughput...)
- outdated_approach: cách làm của phiên bản cũ, không còn đúng với 9.x

## Quality gate

Không chấp nhận câu hỏi nếu:
- số đáp án đúng không khớp response type;
- một distractor cũng bảo vệ được theo tài liệu Elastic 9.x;
- source không phải tài liệu Elastic chính thức (hoặc không ghi phiên bản);
- phụ thuộc hành vi có thể đã đổi giữa các phiên bản mà không ghi version/ngày kiểm tra;
- explanation mâu thuẫn với đáp án.

Câu chưa có source chính thức phải để `status: draft`.
