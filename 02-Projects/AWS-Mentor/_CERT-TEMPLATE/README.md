# Cert Template

Hướng dẫn thêm một chứng chỉ AWS mới vào AWS Mentor.

## Các bước

1. Lấy exam guide chính thức của chứng chỉ từ AWS (docs.aws.amazon.com/aws-certification hoặc trang certification tương ứng). Ghi lại: tên domain, % weighting, số câu, thời gian thi, định dạng câu hỏi, lệ phí. Không suy đoán các con số này.
2. Tạo thư mục `02-Projects/AWS-Mentor/<CERT-CODE>/` với cấu trúc giống `SAA-C03/`:
   ```text
   <CERT-CODE>/
   ├── Questions/<Domain-N-Ten-Domain>/   # một thư mục con cho mỗi domain chính thức
   ├── Sessions/
   ├── Mistakes/
   ├── Insights/
   ├── Labs/
   └── Strategies/STRATEGY-LOG.md
   ```
3. Thêm một section mới cho `<CERT-CODE>` trong `03-Areas/AWS-Certification-Profile.md` (roadmap table + section performance riêng).
4. Nếu domain/question style khác biệt đáng kể (ví dụ chứng chỉ Specialty có nhiều câu troubleshooting hơn), cân nhắc tạo `08-AI/AWS-Mentor/Rules/<CERT-CODE>-Question-Rules.md` riêng; nếu không, dùng chung `Question-Rules.md`.
5. Cập nhật `01-Dashboard/AWS-Mentor.md` nếu cần thêm bảng riêng cho cert mới (thường không cần, vì dashboard đã group theo trường `cert`).
6. Copy `templates/AWS-Mentor/Question.md` và sửa suggester `domain` cho đúng domain của cert mới.

## Nguyên tắc

Không tạo domain list hoặc % weighting cho một chứng chỉ nếu chưa đọc exam guide chính thức — tránh fabricate technical facts.
