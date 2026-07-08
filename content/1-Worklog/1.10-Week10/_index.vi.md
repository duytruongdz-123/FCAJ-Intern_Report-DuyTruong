---
title: "Worklog Tuần 10"
date: 2026-06-22
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---


### Mục tiêu tuần 10:
* Liên kết các phân vùng dữ liệu hạ tầng từ AWS CloudWatch vào cổng kết nối dữ liệu Grafana Cloud.
* Thiết lập các biểu đồ tài nguyên cốt lõi và luật tự động gửi thư báo động.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | ------------ | --------------- | ----------------------------------------- |
| 2 | - Khởi tạo mã định danh xác thực để vận hành trên AWS | 22/06/2026 | 22/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Thêm nguồn dữ liệu (Data Source) CloudWatch vào Grafana | 23/06/2026 | 23/06/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 4 | - Thiết lập Panel biểu đồ từ các Namespace: `AWS/EC2`, `AWS/ApplicationELB`, `ECS/ContainerInsights` | 24/06/2026 | 25/06/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 5 | - Cấu hình Contact Point trong phân hệ Alerting để nhận thông báo | 26/06/2026 | 26/06/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 6 | - Khởi tạo Alert Rule ràng buộc chỉ số RequestCount và thiết lập chu kỳ quét dữ liệu | 27/06/2026 | 27/06/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |

### Kết quả đạt được tuần 10:
* Kết nối thành công luồng truyền dẫn chỉ số giữa AWS và Grafana Cloud.
* Hoàn thiện thiết kế bảng điều khiển tập trung cho cả tầng tính toán, cân bằng tải và bộ nhớ.
* Tự động hóa hoàn toàn quy trình cảnh báo sự cố hạ tầng.

---

### Hình ảnh minh chứng thực hiện tuần 10

#### 1. Khởi tạo mã cấu hình bảo mật OTLP Token (otlp-token) trong danh mục Cloud Access Policies trên Grafana Cloud
![Khởi tạo otlp-token trên Grafana Cloud](/images/1-Worklog/Week10/Picture43.png)

#### 2. Thiết lập và quản lý trạng thái hoạt động của cặp mã bảo mật Access Key ứng với tài khoản AWS IAM
![Quản lý thông tin AWS IAM Access Key](/images/1-Worklog/Week10/Picture44.png)

#### 3. Hệ thống biểu đồ giám sát đa chiều hiển thị tần suất Request Count, CPU Utilization và mức độ tiêu thụ RAM của dịch vụ
![Hệ thống Dashboard theo dõi CPU, Request và RAM](/images/1-Worklog/Week10/Picture45.png)