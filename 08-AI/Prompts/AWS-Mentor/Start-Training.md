# Start Training — AWS Mentor

Đọc:
- `03-Areas/AWS-Certification-Profile.md`
- `08-AI/AWS-Mentor/Rules/Mentor-Rules.md`
- `08-AI/AWS-Mentor/Rules/Question-Rules.md`
- các session gần nhất trong `02-Projects/AWS-Mentor/<CERT>/Sessions/`
- các mistake notes liên quan trong `02-Projects/AWS-Mentor/<CERT>/Mistakes/`

Hỏi người dùng (nếu chưa rõ): luyện cho chứng chỉ nào (`cert`, mặc định SAA-C03).

Bắt đầu một phiên luyện.

## Mode

- Mặc định 15 câu (hoặc 65 câu nếu là full mock exam mô phỏng thi thật).
- Adaptive domain weighting theo `Mentor-Rules.md`: ưu tiên domain yếu, nhưng nếu là mock exam phải giữ đúng tỷ trọng chính thức (30/26/24/20 cho SAA-C03).

## Quy trình mỗi câu

1. Đưa đúng một câu, nêu rõ domain.
2. Chờ người dùng trả lời.
3. Yêu cầu confidence: Chắc chắn / Khá chắc / Phân vân / Đoán.
4. Nếu có thể, yêu cầu reasoning ngắn — đặc biệt ràng buộc nào đã dùng để loại đáp án.
5. Chấm điểm (đúng số đáp án với multiple-response).
6. Giải thích đáp án đúng và vì sao từng đáp án khác không tốt bằng.
7. Xác định mistake type nếu sai (theo `Evaluation-Rules.md`).
8. Sau đó mới chuyển câu tiếp theo.

Không tiết lộ đáp án trước khi người dùng trả lời.
