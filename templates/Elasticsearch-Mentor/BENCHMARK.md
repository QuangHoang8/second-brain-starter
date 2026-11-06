---
id: B-<% tp.date.now("YYYYMMDDHHmmss") %>
type: es-benchmark
stage: 12-performance-storage-tuning
topic:
goal: <% tp.system.suggester(["storage","indexing-speed","search-latency","other"], ["storage","indexing-speed","search-latency","other"]) %>
change:
es_version: "9.x"
dataset_desc:
metric_name:
metric_before:
metric_after:
runs: 1
verified: false
status: needs-verification
date: <% tp.date.now("YYYY-MM-DD") %>
tags:
  - elasticsearch/benchmark
---

# Benchmark - <% tp.file.title %>

> Không ghi API key, mật khẩu, Cloud ID, hostname/IP, hay dữ liệu thật vào file này (dùng placeholder như `<ES_HOST>`). Xem `08-AI/Elasticsearch-Mentor/Rules/Benchmark-Rules.md`.
> Kết quả chỉ phản ánh môi trường này, không phải best practice chung.

## Objective

## Environment (mô tả chung)

- Phiên bản ES:
- Số shard / replica:
- Mapping / setting liên quan:
- Kích thước dataset (dữ liệu giả):
- Loại máy (mô tả chung):

## Change (một biến duy nhất)

## Commands run (Kibana Dev Tools, đã loại thông tin nhạy cảm)

```json
```

## Measurements

| Run | Trước | Sau | Ghi chú |
| --- | ----- | --- | ------- |
| 1   |       |     |         |

## Observations

## Cleanup

- [ ] Đã xoá index tạm
- [ ] Đã hoàn tác setting đã đổi

## Related knowledge

## Source / verification

TODO: Đối chiếu với tài liệu Elastic 9.x hoặc đo lặp lại trước khi đặt `verified: true`.

<% tp.file.cursor(1) %>
