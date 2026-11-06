---
id: S-<% tp.date.now("YYYYMMDDHHmmss") %>
type: es-session
stage:
date: <% tp.date.now("YYYY-MM-DD") %>
mode: training
total_questions: 10
correct_answers: 0
score: 0
accuracy: 0
created: <% tp.date.now("YYYY-MM-DD HH:mm") %>
tags:
  - elasticsearch/session
---

# Training Session - <% tp.date.now("YYYY-MM-DD HH:mm") %>

## Configuration

- Stage:
- Number of questions: 10
- Mode: training (hoặc review / hands-on)

## Results

- Correct answers: 0
- Incorrect answers: 0
- Score: 0
- Accuracy: 0

## Question log

| #   | Question | My answer | Correct answer | Confidence | Result | Stage |
| --- | -------- | --------- | --------------- | ---------- | ------ | ----- |
| 1   |          |           |                 |            |        |       |

## Analysis

### Strengths

### Weaknesses

### Knowledge gaps

### Strategy mistakes

## Next training priorities

<% tp.file.cursor(1) %>
