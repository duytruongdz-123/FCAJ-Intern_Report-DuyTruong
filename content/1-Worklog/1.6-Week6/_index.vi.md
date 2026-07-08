---
title: "Worklog Tuần 6"
date: 2026-05-25
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---


### Mục tiêu Tuần 6:

* Đánh giá khả năng phục hồi của hạ tầng đám mây và các giới hạn điểm gãy dưới điều kiện lưu lượng truy cập nghiêm trọng.
* Truyền trực tiếp các số liệu tải khi thực thi kiểm thử cục bộ vào bảng điều khiển Grafana Cloud để phân tích mối tương quan.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 2 | - Tìm hiểu cách xây dựng các kịch bản tải nâng cao bằng khung kiểm thử áp lực nguồn mở `k6` | 25/05/2026 | 25/05/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 3 | - Viết kịch bản kiểm thử tải JavaScript chuyên dụng trong `k6` để tăng mạnh lưu lượng truy cập đồng thời từ 50 lên 400 Người dùng ảo (VUs) | 26/05/2026 | 26/05/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 4 | - Chạy các kiểm thử áp lực cục bộ đối với hệ thống mục tiêu và ghi lại tiến trình thực hiện | 27/05/2026 | 27/05/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 5 | - Kiểm toán các giá trị cơ sở của hệ thống so với số liệu đo lường khi chịu tải cao (ghi nhận các trường hợp CPU đạt tối đa 100%, Thời gian phản hồi mục tiêu chạm mức ~7.5 giây, và số phiên cơ sở dữ liệu hoạt động tăng gấp đôi) | 28/05/2026 | 28/05/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 6 | - Cấu hình Endpoint Prometheus Remote Write trong k6 agent cục bộ <br> - Truyền số liệu thực thi cục bộ trực tiếp lên bảng điều khiển Grafana Cloud | 29/05/2026 | 29/05/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |


### Kết quả đạt được trong Tuần 6:

* Phát triển các kịch bản kiểm thử tự động có cấu trúc để bộc lộ các giới hạn chịu tải của hạ tầng hệ thống.
* Xác minh thành công hành vi của hệ thống dưới các đợt tăng tải đột biến gấp 8 lần, ghi lại các mức trễ nghiêm trọng (độ trễ phản hồi khoảng ~7.5 giây) và các điểm nghẽn tính toán.
* Hợp nhất các số liệu tải riêng lẻ bằng cách cấu hình đường truyền Prometheus Remote Write.
* Đạt được khả năng tương quan chéo môi trường, cho phép phân tích hiệu năng thống nhất giữa trình tạo tải và bảng điều khiển hạ tầng phần cứng thực tế.

---

### Hình ảnh minh chứng thực hiện tuần 6

#### 1. Tạo Token và lấy link Token
![Cấu hình OTLP hoặc Spring Boot Metrics trên Grafana Cloud để lấy Endpoint URL và API Token](/images/1-Worklog/Week6/Picture13.png)


![Khởi tạo Quy tắc cảnh báo tự động mới trong Grafana Cloud](/images/1-Worklog/Week6/Picture14.png)


![Thiết lập điều kiện ngưỡng cảnh báo lỗi HTTP 500 hoặc RAM CPU vượt quá 85 phần trăm trong 1 phút](/images/1-Worklog/Week6/Picture15.png)

#### 2. Tạo ứng dụng Backend Local
![Cấu hình và kết nối Contact Points để hệ thống tự động gửi email thông báo](/images/1-Worklog/Week6/Picture16.png)

#### 3. Kích hoạt ứng dụng và đẩy dữ liệu
![Viết kịch bản kiểm thử tải JavaScript chuyên dụng trong k6 từ 50 lên 400 VUs](/images/1-Worklog/Week6/Picture17.png)

#### 4. Đẩy dữ liệu từ máy bạn lên, để hiện thị trên các biểu đồ server Grafana
![Thực thi kiểm thử áp lực cục bộ bằng k6 và ghi lại tiến trình chạy](/images/1-Worklog/Week6/Picture18.png)


![Kiểm toán số liệu đo lường chịu tải cao ghi nhận CPU đạt tối đa 100 phần trăm](/images/1-Worklog/Week6/Picture19.png)


![Ghi nhận hành vi hệ thống với thời gian phản hồi chạm mức 7.5 giây dưới áp lực tải](/images/1-Worklog/Week6/Picture20.png)

![Giám sát số liệu hạ tầng ghi nhận số phiên cơ sở dữ liệu hoạt động tăng gấp đôi](/images/1-Worklog/Week6/Picture21.png)

#### 5. Cấu hình địa chỉ Email nhận cảnh báo
![Cấu hình Endpoint Prometheus Remote Write trong k6 agent cục bộ](/images/1-Worklog/Week6/Picture22.png)

#### 6. Tạo quy tắc cảnh báo (Alert rule)
![Ảnh chụp màn hình Dashboard Grafana Cloud hiển thị biểu đồ số liệu thời gian thực từ local backend](/images/1-Worklog/Week6/Picture23.png)

#### 7. Nhận email cảnh báo tự động được gửi về từ hệ thống Grafana Cloud
![Ảnh chụp màn hình hòm thư điện tử nhận email cảnh báo tự động từ Grafana Cloud](/images/1-Worklog/Week6/Picture24.png)

#### 8. Họp Nhóm
![Họp Nhóm](/images/1-Worklog/Week6/2905_meeting_w6.JPG)