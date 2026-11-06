# Benchmark Rules — Elasticsearch Mentor

Tối ưu hiệu năng và dung lượng cần số đo. Thực hành chạy trên cluster/Kibana thật của người dùng, nên có rủi ro **mất dữ liệu**, **tốn tài nguyên** và **rò rỉ thông tin nhạy cảm**.

## An toàn trước khi chạy

- Ưu tiên chạy trên **index tạm** (ví dụ tiền tố `mentor-bench-`), không đụng index dữ liệu thật.
- Cảnh báo trước các thao tác nặng hoặc phá hủy: delete index, `_delete_by_query`, `_update_by_query`, `_reindex` lớn, force merge, thay đổi `number_of_replicas`/`refresh_interval` trên index đang phục vụ.
- Nếu cluster dùng chung hoặc là production, hỏi người dùng xác nhận trước khi hướng dẫn thao tác tốn tài nguyên.
- Sau khi xong: nhắc xoá index tạm và hoàn tác setting đã đổi.

## Đo cho đúng

- Ghi rõ điều kiện: phiên bản ES, kích thước dataset, số shard/replica, mapping/setting liên quan, loại máy (mô tả chung, không ghi hostname).
- Đo trước và sau mỗi thay đổi, chỉ đổi **một biến** mỗi lần.
- Lặp lại đo ít nhất vài lần và ghi cả độ biến thiên khi có thể. Một lần đo đơn lẻ là chưa đủ kết luận.
- Công cụ gợi ý: CAT API, `_stats`, `_cat/indices`, `_cat/segments`, `_disk_usage` (nếu có ở 9.x), profile API. Mọi API phải kiểm tra lại với docs 9.x trước khi dạy.

## Cách gắn nhãn kết quả

- Mọi benchmark mới để `verified: false` và `status: needs-verification`.
- Chỉ nâng lên verified khi đã đo lặp lại hoặc đối chiếu được với tài liệu Elastic 9.x.
- **Không** khẳng định một con số là "best practice chung" nếu chỉ đo trên một dataset/một máy. Ghi là "quan sát trong môi trường này".

## Secrets & dữ liệu nhạy cảm, không được ghi vào vault

Tuyệt đối không ghi vào note:
- API key, mật khẩu, token, chứng chỉ, Cloud ID
- hostname, IP, URL nội bộ của cluster
- dữ liệu thật của khách hàng/công ty trong document mẫu (dùng dữ liệu giả)

Nếu người dùng dán output có vẻ chứa thông tin nhạy cảm, cảnh báo và không lưu nguyên văn; thay bằng placeholder như `<ES_HOST>`.

Đây là yêu cầu bắt buộc của `CLAUDE.md` mục "Mandatory safety rules" (#1).
