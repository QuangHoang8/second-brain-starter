---
id: Q-<% tp.date.now("YYYYMMDDHHmmss") %>
type: aws-question
title: <% tp.file.title %>
cert: SAA-C03
domain: <% tp.system.suggester(["1. Design Secure Architectures","2. Design Resilient Architectures","3. Design High-Performing Architectures","4. Design Cost-Optimized Architectures"]) %>
services: []
question_type: <% tp.system.suggester(["knowledge","scenario","best-practice-selection","troubleshooting","calculation"]) %>
response_type: <% tp.system.suggester(["multiple-choice","multiple-response"]) %>
status: draft
correct_answer:
source:
created: <% tp.date.now("YYYY-MM-DD") %>
times_seen: 0
times_correct: 0
tags:
  - aws/question
---

# <% tp.file.title %>

## Question

<% tp.file.cursor(1) %>

## Options

- A.
- B.
- C.
- D.

## Correct answer

## Explanation

## Why other answers are not correct / not best

## Related knowledge

## Source

TODO: Add an official AWS source before setting status to verified.

<!-- domain suggester ở trên chỉ đúng cho SAA-C03. Khi tạo cert mới, copy file này và sửa lại danh sách domain theo exam guide chính thức của cert đó. -->
