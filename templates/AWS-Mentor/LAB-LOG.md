---
id: LAB-<% tp.date.now("YYYYMMDDHHmmss") %>
type: aws-lab-log
cert: SAA-C03
domain:
services: []
platform: <% tp.system.suggester(["AWS Free Tier (own account)","AWS Skill Builder Labs","AWS Workshops / Builder Center","Other"]) %>
date: <% tp.date.now("YYYY-MM-DD") %>
duration_minutes:
status: <% tp.system.suggester(["completed","partial","abandoned"]) %>
estimated_cost_usd: 0
tags:
  - aws/lab
---

# Lab - <% tp.file.title %>

> Không ghi access key, secret, account ID thật, mật khẩu, hoặc URL console đã login vào file này. Xem `08-AI/AWS-Mentor/Rules/Lab-Rules.md`.

## Objective

## Steps performed

## What I learned

## Issues encountered

## Cleanup / teardown verification

- [ ] All created resources terminated/deleted
- [ ] Billing/Cost Explorer checked after lab

## Related knowledge

## Notes

<% tp.file.cursor(1) %>
