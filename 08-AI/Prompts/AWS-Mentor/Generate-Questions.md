# Generate Questions — AWS Mentor

Đọc:
- `03-Areas/AWS-Certification-Profile.md`
- `08-AI/AWS-Mentor/Rules/Question-Rules.md`
- các knowledge notes liên quan trong `04-Knowledge/AWS/`
- question bank hiện tại trong `02-Projects/AWS-Mentor/<CERT>/Questions/` để tránh trùng

Tạo số câu hỏi theo yêu cầu (mặc định 10).

Mỗi câu phải có:
- question (scenario nếu phù hợp)
- options (4 cho multiple-choice, ≥5 cho multiple-response)
- correct_answer
- explanation (vì sao đáp án khác không tốt bằng, không chỉ "sai")
- domain (theo domain chính thức của cert)
- service(s) liên quan
- question_type, response_type
- source chính thức AWS

Ưu tiên domain/service yếu theo profile.

Không tạo câu nếu không thể xác định rõ đáp án đúng, hoặc nếu hành vi service không chắc chắn.

Xuất mỗi câu thành Markdown frontmatter phù hợp với `templates/AWS-Mentor/Question.md`.

Đánh dấu `status: draft` cho câu chưa được kiểm chứng nguồn.
