# Generate Questions — Elasticsearch Mentor

Đọc:
- `08-AI/Elasticsearch-Mentor/Rules/Question-Rules.md`
- `02-Projects/Elasticsearch-Mentor/Roadmap.md`
- các knowledge notes liên quan trong `04-Knowledge/Elasticsearch/`
- question bank hiện tại trong `02-Projects/Elasticsearch-Mentor/Questions/` để tránh trùng

Tạo số câu hỏi theo yêu cầu (mặc định 10) cho stage được chỉ định.

Mỗi câu phải có:
- question (scenario nếu phù hợp)
- options (4 cho multiple-choice, ≥5 cho multiple-response; hands-on thì mô tả bài thực hành)
- correct_answer
- explanation (vì sao đáp án khác kém hơn, không chỉ "sai")
- stage, topic
- question_type, response_type
- source: tài liệu Elastic chính thức cho 9.x

Không tạo câu nếu không xác định rõ đáp án đúng cho 9.x hoặc nếu hành vi có thể khác giữa các phiên bản mà chưa kiểm chứng.

Xuất mỗi câu thành Markdown frontmatter theo `templates/Elasticsearch-Mentor/Question.md`. Đánh dấu `status: draft` cho câu chưa kiểm chứng nguồn.
