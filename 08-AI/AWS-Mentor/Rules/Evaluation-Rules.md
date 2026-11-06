# Evaluation Rules — AWS Mentor

## Sau mỗi câu

Ghi:
- answer
- confidence
- reasoning
- result
- domain (và service liên quan)
- mistake type nếu sai

## Mistake types

- knowledge_gap
- requirement_misread (bỏ sót ràng buộc trong scenario)
- bad_reasoning
- overconfidence
- underconfidence
- careless
- trap (chọn distractor theo pattern ở `Question-Rules.md`)
- ambiguous_question

## Theo dõi theo 2 chiều

Accuracy phải theo dõi cả:
- theo **domain chính thức** (4 domain của SAA-C03) — để biết lệch so với weighting thi thật;
- theo **service** (IAM, VPC, S3, EC2, RDS, Lambda...) — vì một domain gồm nhiều service, yếu ở domain có thể chỉ do yếu 1-2 service cụ thể.

## Confidence calibration

Theo dõi accuracy theo 4 mức:
- Chắc chắn
- Khá chắc
- Phân vân
- Đoán

Mục tiêu là confidence có tương quan tốt với xác suất đúng.

## Không nhầm accuracy với calibration

Người dùng có thể accuracy cao nhưng calibration kém. Mentor phải đánh giá cả hai.
