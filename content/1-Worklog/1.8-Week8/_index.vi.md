---
title: "Worklog Tuần 8"
date: 2026-06-08
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---


### Mục tiêu tuần 8:
* Khởi tạo tài khoản phân quyền tối thiểu phục vụ trích xuất dữ liệu đám mây ngoại vi an toàn.
* Thiết lập kịch bản giả lập tải đột biến và đồng bộ luồng metrics từ local lên Grafana Cloud.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | ------------ | --------------- | ----------------------------------------- |
| 2 | - Đăng nhập AWS IAM Console để cấu hình tài khoản định danh kết nối tự động | 08/06/2026 | 08/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Gán chính sách `CloudWatchReadOnlyAccess` tuân thủ nguyên tắc đặc quyền tối thiểu | 09/06/2026 | 09/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Viết tệp kịch bản JavaScript (`stress_test.js`) bằng `k6` cấu hình chu kỳ ép tải | 10/06/2026 | 10/06/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 5 | - Trích xuất các thông số định danh Prometheus Remote Write từ Grafana Cloud | 11/06/2026 | 11/06/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 6 | - Thiết lập biến môi trường hệ thống và kích hoạt công cụ chạy tải | 12/06/2026 | 12/06/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |

### Kết quả đạt được tuần 8:
* Đảm bảo an toàn bảo mật luồng tích hợp liên đám mây bằng các chính sách IAM được kiểm duyệt.
* Xây dựng thành công bộ công cụ tự động hóa sinh tải cao nhằm đánh giá độ bền bỉ.
* Tập trung hóa các chỉ số hiệu năng phân tán từ local lên bảng điều khiển Grafana Cloud.

---

### Hình ảnh minh chứng thực hiện tuần 8

#### 1. Khởi tạo người dùng IAM User mới thành công trên bảng điều khiển AWS
![Khởi tạo IAM User thành công](/images/1-Worklog/Week8/Picture35.png)

#### 2. Gán chính quyền hạn đọc dữ liệu CloudWatch (CloudWatchReadOnlyAccess) cho người dùng
![Gán quyền CloudWatchReadOnlyAccess cho IAM User](/images/1-Worklog/Week8/Picture36.png)

#### 3. Tạo và truy xuất thành công cặp Access Key và Secret Access Key của IAM User
![Tạo AWS Access Key cho IAM User](/images/1-Worklog/Week8/Picture37.png)

#### 4. Tích hợp và kiểm tra kết nối thành công CloudWatch Data Source trên Grafana Cloud
![Kết nối thành công CloudWatch trên Grafana Cloud](/images/1-Worklog/Week8/Picture38.png)

#### 5. Cấu hình hệ thống Dashboard theo dõi các chỉ số trễ phản hồi của ALB và tài nguyên CPU/RAM
![Cấu hình hệ thống Dashboard giám sát hiệu năng](/images/1-Worklog/Week8/Picture39.png)

#### 6. Tra cứu thông tin định danh và Endpoint dịch vụ Prometheus trên Grafana Labs
![Tra cứu thông tin Prometheus Instance Details](/images/1-Worklog/Week8/Picture40.png)

#### 7. Lấy thông tin Remote Write Endpoint và API Token kết nối Grafana Cloud Metrics
![Lấy thông số Remote Write Endpoint](/images/1-Worklog/Week8/Picture41.png)

#### 8. Dashboard hoàn chỉnh theo dõi trực quan số lượng kết nối RDS và kết quả kiểm thử tải K6
![Hệ thống Dashboard theo dõi kiểm thử tải K6 và RDS](/images/1-Worklog/Week8/Picture42.png)

#### 9. Lên văn phòng AWS
![Group Meeting](/images/1-Worklog/Week8/1206_meeting_w9.JPG)