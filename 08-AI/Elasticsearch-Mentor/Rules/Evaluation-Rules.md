# Evaluation Rules — Elasticsearch Mentor

## Sau mỗi câu

Ghi: answer, confidence, reasoning, result, stage (và topic liên quan), mistake type nếu sai.

## Mistake types

- knowledge_gap
- requirement_misread
- bad_reasoning
- overconfidence
- underconfidence
- careless
- trap
- version_mismatch (đúng với phiên bản cũ nhưng sai với 9.x)
- ambiguous_question

## Theo dõi theo 2 chiều

- theo **stage** (01-12) để biết nền tảng nào còn yếu;
- theo **topic** (mapping, bool query, shard sizing, ILM...) vì một stage gồm nhiều topic.

## Confidence calibration

Theo dõi accuracy theo 4 mức: Chắc chắn, Khá chắc, Phân vân, Đoán. Mục tiêu là confidence tương quan tốt với xác suất đúng. Accuracy cao nhưng calibration kém vẫn phải được chỉ ra.

## Hands-on

Với bài hands-on, đánh giá cả kết quả dự đoán (đoán đúng hành vi chưa) lẫn kết quả thực tế; sai lệch giữa hai cái là tín hiệu knowledge gap.
