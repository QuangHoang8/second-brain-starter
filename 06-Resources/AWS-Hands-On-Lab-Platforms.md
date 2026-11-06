---
id: aws-hands-on-lab-platforms
title: "AWS Hands-On Lab Platforms"
type: resource
resource_type: documentation
domain: aws
status: to-review
created: 2026-11-06
updated: 2026-11-06
tags:
  - aws
  - hands-on
  - lab
  - free-tier
sources:
  - title: "AWS Free Tier"
    url: "https://aws.amazon.com/free/"
    publisher: "Amazon Web Services"
    accessed: 2026-11-06
  - title: "AWS Skill Builder"
    url: "https://skillbuilder.aws/"
    publisher: "Amazon Web Services"
    accessed: 2026-11-06
  - title: "AWS Builder Center — Workshops"
    url: "https://builder.aws.com/build/workshops"
    publisher: "Amazon Web Services"
    accessed: 2026-11-06
---

# AWS Hands-On Lab Platforms

So sánh các lựa chọn để thực hành hands-on AWS khi luyện thi chứng chỉ, ưu tiên miễn phí. Thông tin về hạn mức/giá có thể thay đổi — luôn kiểm tra trang chính thức trước khi dựa vào con số cụ thể.

## 1. AWS Free Tier (tài khoản AWS cá nhân)

- **Link:** https://aws.amazon.com/free/
- Gồm: dịch vụ **Always Free** trong hạn mức hàng tháng, một khoản credit giới thiệu cho khách hàng mới, và một số **free trial** ngắn hạn cho dịch vụ trả phí.
- **Ưu điểm:** môi trường thật, giống hệt thi/làm việc thực tế, không giới hạn phạm vi lab.
- **Rủi ro:** có thể phát sinh phí nếu vượt hạn mức hoặc dùng dịch vụ ngoài free tier (NAT Gateway, RDS multi-AZ, EC2 ngoài free tier...). **Bắt buộc đọc `08-AI/AWS-Mentor/Rules/Lab-Rules.md` trước khi dùng.**
- Phù hợp nhất cho lab cần quyền kiểm soát đầy đủ (VPC, IAM, networking phức tạp).

## 2. AWS Skill Builder

- **Link:** https://skillbuilder.aws/
- Nền tảng học chính thức của AWS: có khoá học digital miễn phí, một số lab miễn phí, và các gói lab/learning plan trả phí (AWS Builder Labs, subscription).
- Cần kiểm tra trực tiếp trên site phần nào đang miễn phí tại thời điểm dùng, vì danh mục free/paid thay đổi theo thời gian.
- Phù hợp để học có lộ trình bài bản theo từng chứng chỉ.

## 3. AWS Builder Center — Workshops (trước đây là workshops.aws)

- **Link:** https://builder.aws.com/build/workshops
- Kho hướng dẫn hands-on tự học (self-paced) do AWS và cộng đồng AWS xây dựng, theo nhiều chủ đề/service.
- Một số workshop có "free sandbox environment" (môi trường AWS miễn phí cấp sẵn), số khác yêu cầu dùng tài khoản AWS cá nhân (áp dụng rủi ro như mục 1) — kiểm tra ghi chú trên từng workshop trước khi bắt đầu.
- Phù hợp để luyện theo kịch bản thực tế gần với dạng scenario của đề thi.

## Gợi ý thứ tự ưu tiên

1. Workshop có sẵn free sandbox (Builder Center) — rủi ro chi phí thấp nhất, không cần tài khoản riêng.
2. AWS Skill Builder — phần free content/lab, theo lộ trình chứng chỉ.
3. AWS Free Tier trên tài khoản cá nhân — khi cần kiểm soát đầy đủ hoặc lab không có sẵn ở 2 nguồn trên; luôn bật budget alert trước.

## Không đưa vào danh sách (chưa xác minh)

Các nền tảng bên thứ ba (A Cloud Guru, Pluralsight, Tutorials Dojo, KodeKloud...) có thể hữu ích nhưng chưa được xác minh trong note này — thêm sau nếu người dùng thực sự dùng và muốn ghi lại nhận xét từ trải nghiệm thật (type: resource, với source + ngày truy cập).
