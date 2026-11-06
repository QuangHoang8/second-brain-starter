---
id: Q-<% tp.date.now("YYYYMMDDHHmmss") %>
type: es-question
title: <% tp.file.title %>
stage: <% tp.system.suggester(["01-introduction","02-core-architecture","03-data-modelling","04-data-ingestion","05-how-search-works","06-text-analysis","07-aggregations","08-relevance-tuning","09-production","10-security","11-vector-ai-search","12-performance-storage-tuning"], ["01-introduction","02-core-architecture","03-data-modelling","04-data-ingestion","05-how-search-works","06-text-analysis","07-aggregations","08-relevance-tuning","09-production","10-security","11-vector-ai-search","12-performance-storage-tuning"]) %>
topic:
es_version: "9.x"
question_type: <% tp.system.suggester(["knowledge","scenario","best-practice-selection","troubleshooting","calculation"], ["knowledge","scenario","best-practice-selection","troubleshooting","calculation"]) %>
response_type: <% tp.system.suggester(["multiple-choice","multiple-response","hands-on"], ["multiple-choice","multiple-response","hands-on"]) %>
status: draft
correct_answer:
source:
created: <% tp.date.now("YYYY-MM-DD") %>
times_seen: 0
times_correct: 0
tags:
  - elasticsearch/question
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

TODO: Add an official Elastic documentation source (version 9.x) before setting status to verified.
