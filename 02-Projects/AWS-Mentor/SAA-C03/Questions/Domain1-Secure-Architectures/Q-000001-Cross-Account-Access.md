---
id: Q-000001
type: aws-question
cert: SAA-C03
domain: "1. Design Secure Architectures"
services: [iam, sts]
question_type: scenario
response_type: multiple-choice
status: draft
correct_answer: B
source: "https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles_common-scenarios_aws-accounts.html"
created: 2026-11-06
times_seen: 0
times_correct: 0
tags:
  - aws/question
---

# Q-000001 — Cross-Account Access via IAM Role

## Question

A company has two AWS accounts: Account A (production) and Account B (security tooling). An application running in Account B needs to read objects from an S3 bucket in Account A. The company wants to avoid storing long-term AWS access keys for this access. Which approach meets this requirement with the LEAST operational overhead?

## Options

- A. Create an IAM user in Account A, generate access keys, and share them with the team managing Account B.
- B. Create an IAM role in Account A with a trust policy that allows Account B to assume it, and have the application in Account B assume that role using AWS STS.
- C. Make the S3 bucket public and restrict access using a bucket policy that checks the source IP of Account B.
- D. Copy the S3 bucket's data into Account B on a schedule using a cron job with stored access keys.

## Correct answer

B

## Explanation

A cross-account IAM role with a trust policy lets a principal in Account B assume a role in Account A via AWS STS, issuing short-term temporary credentials. This avoids long-term access keys entirely and is the AWS-documented pattern for cross-account access (IAM User Guide — "Access for an IAM user in another AWS account that you own").

## Why other answers are not correct / not best

- A: Long-term access keys shared between teams violate least-privilege/credential-hygiene best practice and create ongoing key-rotation overhead.
- C: A public bucket restricted only by source IP doesn't authenticate identity, is fragile (IPs change), and violates least privilege.
- D: Duplicating data on a schedule adds operational overhead, storage cost, and consistency lag, and still requires stored long-term credentials.

## Related knowledge

- [[AWS-IAM-Roles]]
- [[AWS-STS]]
- [[AWS-Shared-Responsibility-Model]]

## Source

AWS IAM User Guide — "Access for an IAM user in another AWS account that you own" — https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles_common-scenarios_aws-accounts.html

Nội dung trang đã được AI kiểm tra qua fetch trực tiếp ngày 2026-11-06 và khớp với explanation ở trên. `status` vẫn để `draft` cho đến khi người dùng tự xác nhận và đổi sang `verified`.
