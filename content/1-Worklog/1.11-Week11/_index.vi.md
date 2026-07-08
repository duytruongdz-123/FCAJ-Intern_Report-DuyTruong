---
title: "Worklog Tuần 11"
date: 2026-06-29
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---


### Mục tiêu tuần 11:
* Thiết lập phân vùng Dashboard cấp cao mang tên "Stress Test Panel" ở vị trí ưu tiên.
* Đánh giá chi tiết sự tương quan giữa các lớp chỉ số hạ tầng khi hệ thống chịu tải cực hạn.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | ------------ | --------------- | ----------------------------------------- |
| 2 | - Khởi tạo nhóm Row chuyên dụng đặt tên "Stress Test Panel" | 29/06/2026 | 29/06/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 3 | - Xây dựng Panel giám sát lưu lượng mạng đầu vào sử dụng `AWS/ApplicationELB` | 30/06/2026 | 30/06/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 4 | - Thiết lập Panel theo dõi lỗi hệ thống | 01/07/2026 | 01/07/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 5 | - Cấu hình Panel theo dõi hiệu năng container ECS Fargate | 02/07/2026 | 02/07/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 6 | - Triển khai Panel đo đạc Database và kích hoạt script K6 kiểm thử | 03/07/2026 | 03/07/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |

### Kết quả đạt được tuần 11:
* Sắp xếp giao diện Dashboard khoa học, giúp phản ứng nhanh trước các biến động lưu lượng.
* Đạt khả năng bao quát toàn diện hệ thống từ biên mạng, container cho tới cơ sở dữ liệu.
* Thu thập thành công các thông số breakpoint, cung cấp cơ sở để tối ưu hóa Auto Scaling.

---

### Hình ảnh minh chứng thực hiện tuần 11

#### 1. Hệ thống Dashboard tổng quan trạng thái ban đầu của hệ thống khi chưa tải (ALB Throughput, Error Rate, ECS Compute, RDS Connections)
![Biểu đồ tổng quan hệ thống trước khi stress test](/images/1-Worklog/Week11/Picture46.png)

#### 2. Thực thi kịch bản kiểm thử áp lực (Stress Test) bằng công cụ K6 với cấu hình lên tới 200 Virtual Users (VUs)
![Khởi chạy stress test với K6](/images/1-Worklog/Week11/Picture47.png)

#### 3. Biểu đồ Dashboard Grafana ghi nhận sự thay đổi trực quan của ALB Throughput và hiệu suất CPU/RAM khi chịu tải cao
![Biểu đồ hệ thống ghi nhận dữ liệu trong quá trình stress test](/images/1-Worklog/Week11/Picture48.png)

#### 4. Họp nhóm
![Họp nhóm](/images/1-Worklog/Week11/Picture5.jpg)