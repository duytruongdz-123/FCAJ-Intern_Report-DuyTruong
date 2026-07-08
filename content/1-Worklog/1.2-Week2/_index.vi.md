---
title: "Worklog Tuần 2"
date: 2026-04-27
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---



### Mục tiêu tuần 2:

* Cài đặt và cấu hình CloudWatch Agent trên các instance EC2 để thu thập log.
* Triển khai các bộ lọc giám sát bảo mật để phát hiện các hoạt động tấn công (SQL Injection, XSS, Path Traversal).
* Tối ưu hóa chi phí vận hành thông qua quản lý lưu trữ log và custom metrics.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Nghiên cứu kiến trúc CloudWatch Agent và các giao thức truyền tải log | 27/04/2026 | 27/04/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Cài đặt và cấu hình CloudWatch Agent để thu thập log cụ thể của ứng dụng | 28/04/2026 | 28/04/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Triển khai các Metric Filter để xác định các mối đe dọa bảo mật: <br>&emsp; + SQL Injection <br>&emsp; + XSS Attacks <br>&emsp; + Path Traversal | 29/04/2026 | 29/04/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - Cấu hình CloudWatch Alarms và thông báo SNS cho các mẫu tấn công được phát hiện | 30/04/2026 | 30/04/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - Thiết lập chính sách Log Retention (7-30 ngày) và kiểm soát chi phí custom metrics | 01/05/2026 | 03/05/2026 | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 2:

* Tự động hóa thành công việc thu thập log hệ thống và ứng dụng bằng CloudWatch Agent.
* Triển khai hệ thống giám sát bảo mật mạnh mẽ có khả năng phát hiện các cuộc tấn công SQLi, XSS và Path Traversal.
* Thiết lập quy trình cảnh báo tự động thông qua CloudWatch Alarms và SNS.
* Tối ưu hóa chi phí vận hành bằng cách triển khai chiến lược lưu giữ log và quản lý sử dụng custom metric.

---

### Hình ảnh minh chứng thực hiện tuần 2

#### 1. Hoàn thành bài tập tuần 2 và gửi group
![Hoàn thành bài tập tuần 2 và gửi group](/images/1-Worklog/Week2/Picture2.png)