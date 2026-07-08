---
title: "Worklog Tuần 7"
date: 2026-06-01
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---



### Mục tiêu tuần 7:

* Triển khai giải pháp Giám sát hiệu năng ứng dụng chuyên sâu (APM) dựa trên tiêu chuẩn OpenTelemetry.
* Thu thập thông tin vết thực thi mã nguồn bên trong của container ứng dụng đang chạy trên hạ tầng đám mây mà không gây gián đoạn dịch vụ.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | ------------ | --------------- | ----------------------------------------- |
| 2 | - Nghiên cứu cơ chế nhúng agent thu thập dữ liệu của OpenTelemetry (OTel) và các điểm cuối xuất dữ liệu qua giao thức OTLP | 01/06/2026 | 01/06/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 3 | - Khởi tạo một Access Policy bảo mật và trích xuất chuỗi mã hóa Token xác thực OTLP trên bảng điều khiển Grafana Cloud | 02/06/2026 | 02/06/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 4 | - Khai báo cấu hình các biến môi trường OTLP (`OTEL_EXPORTER_OTLP_ENDPOINT`, `OTEL_EXPORTER_OTLP_HEADERS`) trực tiếp vào file Task Definition của AWS ECS | 03/06/2026 | 03/06/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 5 | - Thực hiện cập nhật ứng dụng thông qua tính năng `Force new deployment` trên dịch vụ ECS Service nhằm ép container cập nhật cấu hình telemetry mới mà không gián đoạn dịch vụ | 04/06/2026 | 04/06/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 6 | - Tích hợp và cấu hình bảng điều khiển chuyên sâu JVM Micrometer Dashboard (ID: 4701) trên Grafana Cloud <br> - Theo dõi và phân tích hiệu năng realtime sâu bên trong ứng dụng Java/Spring Boot | 05/06/2026 | 05/06/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |


### Kết quả đạt được tuần 7:

* Chuẩn hóa thành công kiến trúc thu thập dữ liệu vết (telemetry) của hệ thống bằng giải pháp độc lập OpenTelemetry.
* Tích hợp mượt mà các token bảo mật OTLP vào cấu hình triển khai container chịu tải cao.
* Đảm bảo tính liên tục của dịch vụ theo tiêu chuẩn vận hành doanh nghiệp nhờ làm chủ kỹ thuật Rolling Update (`Force new deployment`) trên ECS.
* Đạt năng lực chẩn đoán lỗi chuyên sâu bên trong ứng dụng thông qua việc theo dõi bộ nhớ RAM Heap, luồng xử lý của CPU và hoạt động dọn rác (Garbage Collection) của Java Virtual Machine.

---

### Hình ảnh minh chứng thực hiện tuần 7

#### 1. Khởi tạo và thiết lập API Token cho OpenTelemetry trên Grafana Cloud
![Khởi tạo OpenTelemetry API Token](/images/1-Worklog/Week7/Picture25.png)

#### 2. Sao chép thông tin cấu hình và biến môi trường OpenTelemetry Exporter
![Cấu hình thông số OpenTelemetry](/images/1-Worklog/Week7/Picture26.png)

#### 3. Tạo mới thành công Task Definition tích hợp OpenTelemetry cho Backend trên Amazon ECS
![Tạo thành công ECS Task Definition mới](/images/1-Worklog/Week7/Picture27.png)

#### 4. Trạng thái hoạt động của các cụm Amazon ECS Cluster
![Kiểm tra Amazon ECS Cluster đang chạy](/images/1-Worklog/Week7/Picture28.png)

#### 5. Kiểm tra trạng thái dịch vụ MiniSocial-Backend-Service trên ECS Cluster
![Dịch vụ Backend hoạt động trên ECS](/images/1-Worklog/Week7/Picture29.png)

#### 6. Cập nhật cấu hình triển khai Task mới cho Amazon ECS Service thành công
![Cập nhật và kích hoạt deploy Task mới](/images/1-Worklog/Week7/Picture30.png)

#### 7. Giám sát chi tiết trạng thái Container của Task đang chạy trên AWS Fargate
![Theo dõi thông số Container đang hoạt động](/images/1-Worklog/Week7/Picture31.png)

#### 8. Biểu đồ theo dõi hiệu năng và chỉ số sử dụng CPU (CPU Usage) trên hệ thống
![Biểu đồ giám sát chỉ số CPU](/images/1-Worklog/Week7/Picture32.png)

#### 9. Dashboard chi tiết theo dõi hiệu suất CPU và dung lượng bộ nhớ Memory Utilization
![Dashboard giám sát hiệu năng CPU và Memory](/images/1-Worklog/Week7/Picture33.png)

#### 10. Tra cứu và quản lý Log sự kiện của ứng dụng Spring Boot thông qua Amazon CloudWatch
![Quản lý Log sự kiện trên Amazon CloudWatch](/images/1-Worklog/Week7/Picture34.png)

#### 11. Lên văn phòng AWS
![Group Meeting](/images/1-Worklog/Week7/0406_meeting_w7.JPG)