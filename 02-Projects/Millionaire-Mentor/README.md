# Millionaire Mentor v1

AI mentor cá nhân để luyện thi "Ai là triệu phú", xây trên Obsidian + Markdown + AI.

## Mục tiêu
- Luyện câu hỏi theo độ khó thích ứng.
- Theo dõi đáp án, mức tự tin và reasoning.
- Phân tích điểm mạnh/yếu.
- Ghi lại câu sai để ôn lại.
- Huấn luyện chiến thuật sử dụng quyền trợ giúp.
- Duy trì toàn bộ dữ liệu ở dạng Markdown local.

## Cấu trúc

```text
Millionaire-Mentor-v1/
├── 00-System/
│   └── Millionaire-Mentor/
├── 01-Knowledge/
│   └── Millionaire/
├── 02-Millionaire/
│   ├── Questions/
│   ├── Sessions/
│   ├── Mistakes/
│   ├── Insights/
│   └── Strategies/
├── 03-Profile/
└── 04-Prompts/
```

## Cách dùng nhanh

1. Copy toàn bộ thư mục vào vault Obsidian.
2. Mở `03-Profile/Millionaire-Profile.md` và chỉnh mục tiêu cá nhân.
3. Đọc `00-System/Millionaire-Mentor/Mentor-Rules.md`.
4. Mỗi lần luyện, dùng `04-Prompts/Start-Training.md`.
5. Sau phiên luyện, tạo session từ `02-Millionaire/Sessions/SESSION-TEMPLATE.md`.
6. Chạy `04-Prompts/Analyze-Session.md` với AI để phân tích.
7. Với câu sai quan trọng, tạo note từ `02-Millionaire/Mistakes/MISTAKE-TEMPLATE.md`.
8. Định kỳ chạy `04-Prompts/Weekly-Review.md`.

## Quy tắc vận hành

AI không được tự coi một factual claim là "verified" nếu chưa có nguồn đáng tin cậy hoặc chưa được người dùng xác nhận.

Automation mặc định là semi-automatic: AI đề xuất thay đổi profile/knowledge/mistake; người dùng kiểm tra trước khi ghi chính thức.
