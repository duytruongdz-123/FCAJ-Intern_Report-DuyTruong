---
title: "Worklog Tuần 12"
date: 2026-07-05
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

### Mục tiêu Tuần 12:

- Trích xuất và phân tích các biểu đồ giám sát đã được cấu hình sẵn cho ứng dụng, tài nguyên AWS và hạ tầng tổng quan.
- Trích xuất và phân tích log hệ thống từ AWS CloudWatch để chẩn đoán các sự cố về kết nối cơ sở dữ liệu và connection pool.

### Các công việc thực hiện trong tuần:
| Thứ | Công việc | Ngày bắt đầu | Ngày kết thúc | Tài liệu tham khảo |
| :--- | :--- | :--- | :--- | :--- |
| 2 | - Lấy và xem xét biểu đồ Ứng dụng và biểu đồ Tài nguyên AWS  | 06/07/2026 | 06/07/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04> |
| 3 | - Phân tích biểu đồ Hạ tầng Tổng quan bao gồm các chỉ số ALB, ECS và RDS  | 07/07/2026 | 07/07/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04> |
| 4 | - Trích xuất log CloudWatch để xử lý lỗi hệ thống <br> - Chẩn đoán lỗi timeout của SQL Server và HikariPool  | 08/07/2026 | 08/07/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04> |

### Kết quả đạt được Tuần 12:

- **Phân tích Biểu đồ:** Đã trích xuất và đánh giá thành công 3 biểu đồ Grafana về tình trạng Ứng dụng, Tài nguyên AWS và các chỉ số Hạ tầng.
- **Giám sát Hệ thống:** Trích xuất log lỗi trực tiếp từ bảng điều khiển AWS CloudWatch cho log group `ecs/minisocial-backend`.
- **Xử lý sự cố (Database):** Xác định các lỗi `SQLServerException` nghiêm trọng do quá thời gian kết nối TCP/IP tới phiên bản RDS trên cổng 1433.
- **Xử lý sự cố (Connection Pool):** Chẩn đoán vấn đề cạn kiệt kết nối cơ sở dữ liệu khi `HikariPool-1` không thể xác thực kết nối hoặc bị timeout sau 30000ms.
- **Xử lý sự cố (Xác thực):** Phát hiện nhiều lỗi `ExpiredJwtException` cho thấy các sự cố về việc token của client bị hết hạn trong quá trình xác thực WebSocket.

### Hình ảnh minh chứng thực hiện tuần 12

#### 1. Biểu đồ giám sát Hạ tầng tổng quan (Application Dashboard) trên Grafana
![Biểu đồ giám sát hiệu năng Ứng dụng (Application Dashboard) trên Grafana](/images/1-Worklog/Week12/Picture1.png)

#### 2. Biểu đồ giám sát Hiệu năng ứng dụng (AWS Resources Dashboard) trên Grafana
![Biểu đồ giám sát Tài nguyên AWS (AWS Resources Dashboard) trên Grafana](/images/1-Worklog/Week12/Picture2.png)

#### 3. Biểu đồ giám sát Tài nguyên AWS (Infrastructure Dashboard) trên Grafana
![Biểu đồ giám sát Hạ tầng tổng quan (Infrastructure Dashboard) trên Grafana](/images/1-Worklog/Week12/Picture3.png)

#### 4. Giao diện danh sách các nhóm nhật ký (Log groups) trên Amazon CloudWatch
![Giao diện danh sách các nhóm nhật ký (Log groups) trên Amazon CloudWatch](/images/1-Worklog/Week12/Picture4.png)

#### 5. Hoàn thành Task tuần 12 và gửi group
![ Hoàn thành Task tuần 12 và gửi group](/images/1-Worklog/Week12/Picture123.png)

#### 6. Họp nhóm
![Họp nhóm](/images/1-Worklog/Week12/Picture432.jpg)
