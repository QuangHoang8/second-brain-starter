# AWS Knowledge Base

Đây là knowledge layer dùng chung cho mọi chứng chỉ AWS (SAA-C03, và các cert thêm sau).

Mỗi note nên tập trung vào một service/concept, có thể tái sử dụng cho nhiều cert khác nhau (vd note về IAM dùng được cho cả SAA-C03 và DVA-C02).

## Quy ước

Theo `90-Metadata/CONVENTIONS.md`:
- Tên file: English technical vocabulary, không ngày tháng — ví dụ `AWS-VPC.md`, `AWS-IAM-Roles.md`.
- ID: kebab-case — `aws-vpc`, `aws-iam-roles`.
- `type: knowledge`, `domain: aws`.

## Template tối thiểu

```yaml
---
id: aws-<slug>
type: knowledge
domain: aws
category:        # vd: networking, security, compute, storage, database, cost
status: draft
certs:            # chứng chỉ nào dùng đến concept này, vd [SAA-C03]
created:
updated:
sources: []
---
```

## Nguyên tắc

- Một note = một service hoặc một concept có thể tái sử dụng.
- Link các concept liên quan bằng `[[WikiLink]]`.
- Ghi source chính thức AWS (docs.aws.amazon.com, whitepapers) cho mọi factual claim quan trọng — hành vi/giới hạn service có thể thay đổi theo thời gian, luôn kèm ngày truy cập.
- Không biến knowledge note thành danh sách câu hỏi thi (đó là việc của `02-Projects/AWS-Mentor/<CERT>/Questions/`).
- Khi một claim có thể đã lỗi thời (limit, pricing, tên service), thêm field `reviewed` và ghi rõ cần kiểm tra lại thay vì đoán.

## Subfolders hiện có

- `IAM-Security/`
- `Networking-VPC/`
- `Compute/`
- `Storage/`
- `Database/`
- `Resilience-HA-DR/`
- `Cost-Management/`
- `Monitoring-Observability/`
