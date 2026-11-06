# AWS Certification Mentor

AI mentor cá nhân để luyện thi các chứng chỉ AWS, xây trên Obsidian + Markdown + AI. Hỗ trợ nhiều chứng chỉ song song (multi-cert).

## Mục tiêu

- Luyện câu hỏi bám sát domain & tỷ trọng (weighting) chính thức của từng kỳ thi.
- Theo dõi đáp án, mức tự tin và reasoning theo từng domain/service.
- Phân tích điểm mạnh/yếu theo domain và theo service AWS.
- Ghi lại câu sai và insight để ôn lại.
- Theo dõi lab thực hành (hands-on) và đảm bảo an toàn chi phí/secrets.
- Duy trì toàn bộ dữ liệu ở dạng Markdown local.

## Cấu trúc

```text
AWS-Mentor/
├── README.md
├── _CERT-TEMPLATE/          # Hướng dẫn thêm một chứng chỉ mới
│   └── README.md
└── SAA-C03/                 # Một thư mục con cho mỗi chứng chỉ đang luyện
    ├── Questions/
    │   ├── Domain1-Secure-Architectures/
    │   ├── Domain2-Resilient-Architectures/
    │   ├── Domain3-High-Performing-Architectures/
    │   └── Domain4-Cost-Optimized-Architectures/
    ├── Sessions/
    ├── Mistakes/
    ├── Insights/
    ├── Labs/
    └── Strategies/STRATEGY-LOG.md
```

Kiến thức dùng chung giữa các chứng chỉ (IAM, VPC, S3, EC2...) nằm ở `04-Knowledge/AWS/`, không lặp lại trong từng cert.

## Chứng chỉ đang active

- **SAA-C03** — AWS Certified Solutions Architect – Associate. 4 domain chính thức (nguồn: AWS exam guide, truy cập 2026-11-06):
  1. Design Secure Architectures — 30%
  2. Design Resilient Architectures — 26%
  3. Design High-Performing Architectures — 24%
  4. Design Cost-Optimized Architectures — 20%
  - 65 câu hỏi (50 tính điểm + 15 không tính điểm), 130 phút, multiple choice/multiple response, lệ phí 150 USD, thi tại Pearson VUE hoặc online proctored.

## Cách dùng nhanh

1. Mở `03-Areas/AWS-Certification-Profile.md` và chỉnh mục tiêu/cert đang theo đuổi.
2. Đọc `08-AI/AWS-Mentor/Rules/Mentor-Rules.md`.
3. Mỗi lần luyện câu hỏi, dùng `08-AI/Prompts/AWS-Mentor/Start-Training.md`.
4. Mỗi lần thực hành lab, đọc `08-AI/AWS-Mentor/Rules/Lab-Rules.md` trước, rồi dùng `08-AI/Prompts/AWS-Mentor/Start-Lab.md`.
5. Sau phiên luyện, tạo session từ `templates/AWS-Mentor/SESSION.md`.
6. Chạy `08-AI/Prompts/AWS-Mentor/Analyze-Session.md` với AI để phân tích.
7. Với câu sai quan trọng, tạo note từ `templates/AWS-Mentor/MISTAKE.md`.
8. Định kỳ chạy `08-AI/Prompts/AWS-Mentor/Weekly-Review.md`.
9. Muốn thêm chứng chỉ mới, làm theo `_CERT-TEMPLATE/README.md`.

## Quy tắc vận hành

AI không được tự coi một factual claim về hành vi/giới hạn của AWS service là "verified" nếu chưa có nguồn tài liệu AWS chính thức hoặc chưa được người dùng xác nhận.

Automation mặc định là semi-automatic: AI đề xuất thay đổi profile/knowledge/mistake; người dùng kiểm tra trước khi ghi chính thức.

Không ghi secrets (access key, account ID, mật khẩu, URL console cá nhân...) vào bất kỳ file nào trong dự án này — xem `08-AI/AWS-Mentor/Rules/Lab-Rules.md`.
