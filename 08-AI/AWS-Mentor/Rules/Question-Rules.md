# Question Rules — AWS Mentor

## Domain & weighting (SAA-C03)

Nguồn: AWS exam guide chính thức, truy cập 2026-11-06.
https://docs.aws.amazon.com/aws-certification/latest/solutions-architect-associate-03/solutions-architect-associate-03.html

| Domain | Weighting |
|---|---:|
| 1. Design Secure Architectures | 30% |
| 2. Design Resilient Architectures | 26% |
| 3. Design High-Performing Architectures | 24% |
| 4. Design Cost-Optimized Architectures | 20% |

Với chứng chỉ khác, lấy domain/weighting từ exam guide chính thức của chứng chỉ đó, không suy đoán.

## Response types (theo exam guide)

- **Multiple choice**: 1 đáp án đúng, 3 distractor.
- **Multiple response**: ≥2 đáp án đúng trên ≥5 lựa chọn.

## Question types

- knowledge: nhớ hành vi/giới hạn service
- scenario: chọn kiến trúc/service phù hợp nhất cho một tình huống
- best-practice-selection: nhiều đáp án "chạy được" nhưng chỉ 1 đáp án đúng best practice/Well-Architected
- troubleshooting: xác định nguyên nhân/khắc phục sự cố
- calculation: tính toán cost/capacity/throughput đơn giản

## Distractor pattern cần luyện nhận diện

Đây là kinh nghiệm luyện thi phổ biến, **không phải tài liệu chính thức AWS** — không trích dẫn như fact kỹ thuật:

- wrong_service: service không phù hợp với yêu cầu
- right_service_wrong_config: đúng service nhưng cấu hình sai (vd đúng S3 nhưng sai storage class)
- violates_least_privilege: vi phạm nguyên tắc least privilege/security best practice
- ignores_stated_constraint: bỏ qua ràng buộc đề bài nêu rõ (cost, operational overhead, no code changes, multi-region...)
- higher_cost_than_needed: đáp án đúng về kỹ thuật nhưng không phải lựa chọn cost-effective nhất
- outdated_approach: cách làm cũ/không còn best practice (vd dùng access key thay vì IAM role)

## Quality gate

Không chấp nhận câu hỏi nếu:
- số đáp án đúng không khớp với response type đã khai báo;
- một distractor cũng có thể bảo vệ hợp lý theo tài liệu chính thức;
- source không đáng tin hoặc không phải AWS chính thức;
- câu hỏi phụ thuộc hành vi/giới hạn service có thể đã thay đổi mà không ghi ngày kiểm tra;
- explanation mâu thuẫn với đáp án đã chọn.
