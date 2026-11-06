---
id: inbox-20261030-aws-saa-c03-domain1-secure-architectures
title: "AWS SAA-C03 Exam Guide – Domain 1: Design Secure Architectures"
type: inbox
captured: 2026-10-30
status: unprocessed
tags: []
domain: "cloud-certification (prediction, to confirm)"
source:
  title: "Content Domain 1: Design Secure Architectures — AWS Certified Solutions Architect – Associate (SAA-C03) Exam Guide"
  url: "https://docs.aws.amazon.com/aws-certification/latest/solutions-architect-associate-03/solutions-architect-associate-03-domain1.html"
  accessed: 2026-10-30
---

# Capture

## Raw information

Official AWS exam guide page listing the knowledge and skills covered by **Domain 1: Design Secure Architectures** of the Solutions Architect – Associate (SAA-C03) certification. No author or publication date is shown on the page (standard AWS docs page, publisher = AWS). Three tasks, each split into "Knowledge of" and "Skills in":

**Task 1.1 — Design secure access to AWS resources**
- Knowledge: cross-account access controls, federated access/identity (IAM, IAM Identity Center), AWS global infrastructure (Regions/AZs), AWS security best practices (least privilege), the shared responsibility model.
- Skills: applying IAM best practices (MFA) to users/root; designing flexible authorization (users, groups, roles, policies); role-based access (STS, role switching, cross-account); multi-account security strategy (Control Tower, SCPs); appropriate use of resource policies; when to federate a directory service with IAM roles.

**Task 1.2 — Design secure workloads and applications**
- Knowledge: application config/credential security, AWS service endpoints, controlling ports/protocols/network traffic, secure application access, relevant security services (Cognito, GuardDuty, Macie), external threat vectors (DDoS, SQL injection).
- Skills: VPC security architecture (security groups, route tables, NACLs, NAT gateways); network segmentation (public/private subnets); integrating services to secure apps (Shield, WAF, IAM Identity Center, Secrets Manager); securing external network connections (VPN, Direct Connect).

**Task 1.3 — Determine appropriate data security controls**
- Knowledge: data access/governance, data recovery, data retention/classification, encryption and key management.
- Skills: aligning AWS tech to compliance; encrypting data at rest (KMS); encrypting data in transit (ACM/TLS); access policies for encryption keys; backups/replication; data lifecycle/protection policies; rotating keys and renewing certificates.

## Why this may matter

Reference checklist for SAA-C03 exam prep — maps directly to IAM, VPC, and data-encryption study areas. Useful as a scope/coverage checklist against existing study notes.

## Questions

- Is this being captured for active exam prep, or general reference?

## Processing suggestions

- **Predicted domain:** cloud-certification / aws (unconfirmed — please correct if this should sit under a different area, e.g. a dedicated AWS or certification-prep area note).
- **Predicted tags (unconfirmed):** `aws`, `aws-saa`, `certification`, `cloud-security`, `iam`, `exam-guide`
- Likely candidate for a `learning` note (study checklist / curriculum) rather than a `knowledge` note, since it's an exam scope outline rather than an explained concept. Could later be split into individual `knowledge` notes per topic (IAM, VPC security, KMS/encryption) if deeper notes are written while studying.
