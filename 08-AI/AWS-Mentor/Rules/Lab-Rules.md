# Lab Rules — AWS Mentor

Chứng chỉ AWS đòi hỏi kinh nghiệm thực hành (hands-on), không chỉ lý thuyết. Lab thường chạy trên tài khoản AWS cá nhân → có rủi ro **chi phí** và **rò rỉ secrets** mà phần luyện câu hỏi không có.

## Bắt buộc trước lab đầu tiên (cost safety gate)

Trước khi làm lab đầu tiên trên một tài khoản AWS, phải xác nhận đã:
- [ ] Bật AWS Budgets với ít nhất 1 budget alert (vd alert ở mức rất thấp, ví dụ 5 USD).
- [ ] Bật Billing alarm qua CloudWatch (chi phí ước tính > ngưỡng).
- [ ] Biết cách xem Billing Dashboard / Cost Explorer.

Nếu chưa xác nhận, Mentor phải nhắc lại bước này trước khi hướng dẫn bất kỳ lab nào động tới resource có thể tính phí (EC2, RDS, NAT Gateway, Elastic IP, data transfer...).

## Trong lúc lab

- Ưu tiên dịch vụ nằm trong Always Free / Free Tier khi có thể.
- Nếu lab cần resource có thể phát sinh phí (NAT Gateway, RDS, EC2 ngoài free tier...), nói rõ trước khi hướng dẫn, và nhắc tắt/xoá ngay sau khi xong.
- Không tự ý giả định hạn mức Free Tier hiện tại là chính xác nếu không chắc — đề xuất người dùng kiểm tra trang AWS Free Tier chính thức, vì hạn mức có thể thay đổi.

## Sau lab (teardown bắt buộc)

Trước khi coi một lab là "completed", phải xác nhận:
- [ ] Đã xoá/terminate toàn bộ resource đã tạo (EC2, RDS, NAT Gateway, EIP chưa gắn, EBS volume mồ côi, load balancer...).
- [ ] Đã kiểm tra lại Billing/Cost Explorer sau lab để phát hiện resource còn sót.

Ghi lại estimated cost (nếu biết) vào lab log.

## Secrets — không được ghi vào vault

Tuyệt đối không ghi vào bất kỳ lab log hay note nào trong vault này:
- Access key / secret access key
- Account ID thật (dùng placeholder như `<ACCOUNT_ID>` nếu cần minh hoạ)
- Mật khẩu, MFA secret
- URL console đã login/tokenized, presigned URL thật

Đây là yêu cầu bắt buộc của `CLAUDE.md` mục "Mandatory safety rules" (#1), áp dụng cho toàn bộ AWS Mentor.

## Chọn nền tảng lab

Xem `06-Resources/AWS-Hands-On-Lab-Platforms.md` để so sánh các lựa chọn, ưu tiên miễn phí.
