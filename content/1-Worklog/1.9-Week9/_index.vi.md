---
title: "Worklog Tuần 9"
date: 2026-06-15
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---


### Mục tiêu tuần 9:
* Triển khai giám sát hiệu năng ứng dụng (APM) dựa trên chuẩn mã nguồn mở OpenTelemetry.
* Nhúng cấu hình token bảo mật vào môi trường container đám mây để thu thập các thông số vết code.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | ------------ | --------------- | ----------------------------------------- |
| 2 | - Hoàn thiện bài blog 2 | 15/06/2026 | 15/06/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 3 | - Hoàn thiện bài blog 2 | 16/06/2026 | 16/06/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 4 | - Trực Grafana và quan sát biểu đồ | 17/06/2026 | 17/06/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 5 | - Trực Grafana và quan sát biểu đồ | 18/06/2026 | 18/06/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 6 | - Trực Grafana và quan sát biểu đồ | 19/06/2026 | 19/06/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |

### Kết quả đạt được tuần 9:
* Nghiên cứu thành công kiến trúc **OpenTelemetry (OTel)** và ứng dụng hiệu quả vào việc tích hợp hệ thống giám sát hiệu năng ứng dụng (APM) nâng cao.
* Chuẩn hóa thành công hạ tầng thu thập dữ liệu telemetry tập trung bằng cách nhúng các biến môi trường OTLP vào **AWS ECS Task Definition** và thực hiện cập nhật **ECS Service** trơn tru.
* Tăng cường tính bảo mật và kiểm soát luồng dữ liệu truyền nhận thông qua việc cấu hình nghiêm ngặt các chính sách truy cập (Access Policies) trên **Grafana Cloud**.
* Hoàn thiện tùy biến bảng điều khiển **JVM Micrometer** trên Grafana, giúp nâng cao năng lực giám sát thời gian thực và chẩn đoán lỗi chuyên sâu (bộ nhớ, luồng xử lý) trực tiếp từ bên trong mã nguồn ứng dụng.
---

### Hình ảnh minh chứng thực hiện tuần 9

#### 1. Họp nhóm
![Group Meeting](/images/1-Worklog/Week9/1906_meeting_w10.JPG)