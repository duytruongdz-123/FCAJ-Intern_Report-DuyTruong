---
title: "Worklog Tuần 5"
date: 2026-05-18
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---



### Mục tiêu tuần 5:

* Kết nối và đồng bộ an toàn dữ liệu giám sát từ AWS sang nền tảng đám mây Grafana Cloud.
* Thiết kế Dashboard hạ tầng tập trung nhằm quản lý song song hiệu năng của các tầng mạng, tính toán và cơ sở dữ liệu.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | ------------ | --------------- | ----------------------------------------- |
| 2 | - Nghiên cứu giải pháp phân quyền bảo mật phân tán giữa các nền tảng đám mây dựa trên nguyên tắc đặc quyền tối thiểu | 18/05/2026 | 18/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Khởi tạo một IAM User chuyên dụng trên AWS, gán chính sách hệ thống `CloudWatchReadOnlyAccess` <br> - Xuất Access Key an toàn để phục vụ kết nối ngoại vi | 19/05/2026 | 19/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Truy cập Grafana Cloud, thêm nguồn dữ liệu (Data Source) AWS CloudWatch và cấu hình xác thực bằng cặp Access Key đã tạo | 20/05/2026 | 20/05/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 5 | - Thiết kế các Panel giám sát lưu lượng cổng vào và hiệu năng tính toán cốt lõi: ALB Response Time, ALB Throughput, và CPU/RAM Utilization của AWS ECS Fargate | 21/05/2026 | 22/05/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 6 | - Xây dựng thêm các Panel chuyên biệt kiểm soát tầng lưu trữ dữ liệu cuối bao gồm Database Connections của Amazon RDS và các chỉ số tải ổ đĩa liên quan | 22/05/2026 | 22/05/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |


### Kết quả đạt được tuần 5:

* Thiết lập thành công ranh giới bảo mật đám mây an toàn nhờ việc cô lập quyền hạn chỉ đọc (Read-only) cho tài khoản liên kết IAM.
* Tích hợp thành công luồng cấp phát dữ liệu (metrics pipeline) từ AWS CloudWatch trực tiếp về không gian làm việc Grafana Cloud.
* Hoàn thiện thiết kế giao diện Infrastructure Dashboard trực quan hóa toàn diện hệ thống gồm ba lớp hạ tầng chính (ALB, ECS Fargate, RDS).
* Nâng cao năng lực giám sát tổng thể, cho phép kiểm tra nhanh trạng thái tài nguyên phần cứng để đưa ra quyết định tối ưu hóa kịp thời.

---

### Hình ảnh minh chứng thực hiện tuần 5

#### 1. Chuẩn bị IAM Access Key trên AWS
![Cấu hình lưu trữ source code trên Amazon S3](/images/1-Worklog/Week5/Picture10.png)

#### 2. Tích hợp AWS CloudWatch vào Grafana
![Tạo CloudFront Distribution cho hệ thống](/images/1-Worklog/Week5/Picture11.png)

#### 3. Cấu hình hoàn thành 3 biểu đồ trên Grafana
![Cấu hình các bản ghi Route 53 thành công](/images/1-Worklog/Week5/Picture12.png)