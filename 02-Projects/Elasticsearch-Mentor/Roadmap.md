---
id: elasticsearch-mentor-roadmap
title: Elasticsearch Mentor Roadmap
type: project
status: active
created: 2026-11-06
updated: 2026-11-06
technology:
  - elasticsearch
sources:
  - title: Elasticsearch Roadmap
    url: https://roadmap.sh/elasticsearch
    publisher: roadmap.sh
    accessed: 2026-11-06
tags:
  - elasticsearch/roadmap
---

# Elasticsearch Roadmap

Stage 01-11: node lấy từ roadmap.sh (truy cập 2026-11-06). Danh sách node trên trang bị làm phẳng nên **nhóm node theo stage là suy luận**, chưa đối chiếu với cấu trúc đồ thị gốc; một số node ở cuối trang (Search Analyzer, Boosting, Synonyms, Roles/Users, API Keys, Authentication) được xếp vào stage gần nghĩa nhất.
Stage 12: bổ sung, không thuộc roadmap.sh.

## 01-introduction
- [ ] Pre-requisites: JSON, REST API basics
- [ ] What is Elasticsearch
- [ ] Search engines vs relational DBs
- [ ] The ELK stack
- [ ] Elasticsearch use cases
- [ ] Environment setup: Docker, Elastic Cloud, Kibana Console

## 02-core-architecture
- [ ] Logical concepts: cluster, node, index, document, ID
- [ ] Physical layout: master-eligible, data, coordinating nodes
- [ ] Sharding & scaling: primary shards, replica shards
- [ ] The "split brain" problem

## 03-data-modelling
- [ ] Mappings: explicit, dynamic, mapping explosion
- [ ] Data types: numeric, boolean, text, keyword, dates, geo points
- [ ] Object, nested, flattened
- [ ] Text vs keyword

## 04-data-ingestion
- [ ] CRUD: create/delete index, index/get/update/delete document
- [ ] Bulk index, optimizing bulk indexing
- [ ] Reindex API
- [ ] Update by query, delete by query
- [ ] Migrations & repair

## 05-how-search-works
- [ ] The inverted index, doc values
- [ ] Query languages: Query DSL, EQL, SQL, ES|QL, KQL, Lucene
- [ ] Search contexts: query vs filter
- [ ] Leaf queries: match, exists, term, ID, range, prefix, wildcard
- [ ] Bool (compound) queries: must, must_not, filter, should
- [ ] Controlling results: pagination, source filtering, sorting, highlighting

## 06-text-analysis
- [ ] Analyze API
- [ ] Standard analyzer, custom analyzers
- [ ] Search analyzer
- [ ] fielddata

## 07-aggregations
- [ ] Metric: value count, cardinality, avg/sum/min/max, stats/extended stats
- [ ] Bucket: terms, range/date range, histogram, filter
- [ ] Nested aggregations, pipeline aggregations, advanced aggregations
- [ ] Transformations: pivot, transform API, latest

## 08-relevance-tuning
- [ ] Similarity: BM25
- [ ] Document scoring
- [ ] Improve query precision
- [ ] Boosting queries, function score query
- [ ] Match phrase query
- [ ] Synonyms graph

## 09-production
- [ ] CAT API, cluster monitoring
- [ ] Segment merging
- [ ] ILM, rollover policies, data life cycle
- [ ] Data tiers
- [ ] Snapshots & restore, SLM, data safety
- [ ] Cross-cluster replication
- [ ] Autoscaling

## 10-security
- [ ] Roles & users
- [ ] API keys
- [ ] Authentication

## 11-vector-ai-search
- [ ] Vector search
- [ ] Semantic search
- [ ] Hybrid search
- [ ] AI-powered search

## 12-performance-storage-tuning (bổ sung, không thuộc roadmap.sh)

Nguồn chính: tài liệu Elastic (tune for disk usage / search speed / indexing speed) cho 9.x. Chủ đề dưới đây là đề xuất, cần đối chiếu docs 9.x trước khi dạy.
- [ ] Shard sizing & số lượng shard
- [ ] Mapping để tiết kiệm dung lượng (`_source`, `doc_values`, `index`, kiểu dữ liệu)
- [ ] Tối ưu indexing speed (bulk, `refresh_interval`, replica khi nạp dữ liệu)
- [ ] Tối ưu search speed (filter context, caching, tránh query tốn kém)
- [ ] Force merge, index sorting, nén lưu trữ
- [ ] Đo đạc & benchmark an toàn (xem `Benchmark-Rules.md`)
