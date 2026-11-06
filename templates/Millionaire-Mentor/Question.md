---
id: Q-<% tp.date.now("YYYYMMDDHHmmss") %>
type: millionaire-question
title: <% tp.file.title %>
topic: <% tp.system.suggester(["History","Geography","Science","Literature","Arts","Technology","Culture","Sports","Vietnam"]) %>
subtopic:
difficulty: <% tp.system.suggester(["Easy","Medium","Hard","Expert"]) %>
status: draft
correct_answer:
source:
created: <% tp.date.now("YYYY-MM-DD") %>
tags:
  - millionaire/question
---

# <% tp.file.title %>

## Question

<% tp.file.cursor(1) %>

## Answers

- A.
- B.
- C.
- D.

## Correct answer

## Explanation

## Why other answers are incorrect

## Related knowledge

## Source

TODO: Add a reliable source before setting status to verified.
