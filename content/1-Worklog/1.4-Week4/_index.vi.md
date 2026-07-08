---
title: "Worklog Tuần 4"
date: 2026-05-11
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---



### Mục tiêu tuần 4:

* Giám sát nhật ký vận hành (log) của ứng dụng theo thời gian thực để phát hiện sớm các ngoại lệ và lỗi thực thi phần mềm.
* Thiết lập ngưỡng cảnh báo lỗi tự động và tiến hành giả lập sự cố thực tế để kiểm tra độ nhạy của hệ thống báo động.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | ------------ | --------------- | ----------------------------------------- |
| 2 | - Khảo sát cấu trúc nhật ký ứng dụng được lưu trữ tập trung trên dịch vụ CloudWatch Logs | 11/05/2026 | 11/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Cấu hình bộ lọc CloudWatch Metric Filter quét log theo thời gian thực để bắt các từ khóa lỗi đặc thù bao gồm `?Exception` và `?SQL_INJECTION` | 12/05/2026 | 12/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Thiết lập một CloudWatch Alarm liên kết chặt chẽ với chỉ số lỗi vừa bóc tách từ Metric Filter <br> - Cấu hình ngưỡng báo động kích hoạt khi tần suất lỗi vượt mức lớn hơn hoặc bằng 1 vụ trong vòng 1 phút | 13/05/2026 | 13/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - Cấu hình điều hướng hành động khi Alarm chuyển trạng thái sang `In Alarm` để tự động đẩy email thông báo lỗi qua kênh SNS đã thiết lập | 14/05/2026 | 14/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - Sử dụng công cụ Postman liên tục gửi request vào các URL sai định dạng nhằm ép ứng dụng sinh log lỗi hệ thống <br> - Xác thực trạng thái chuyển đổi danh mục Alarm và kiểm tra kết quả email nhận được | 15/05/2026 | 15/05/2026 | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 4:

* Triển khai thành công bộ lọc dữ liệu thông minh trên CloudWatch Logs nhằm xử lý log thời gian thực với độ chính xác cao.
* Tự động hóa quá trình nhận diện lỗi hệ thống nguy hiểm dựa trên việc ánh xạ từ khóa đặc thù từ mã nguồn.
* Làm chủ kỹ năng cấu hình các điều kiện ràng buộc thời gian ngắn (1 phút) phục vụ giám sát nghiêm ngặt cho môi trường production.
* Xác thực hoàn chỉnh mức độ tin cậy và tốc độ phản hồi của hệ thống cảnh báo thông qua các bài kiểm thử ép sinh lỗi bằng Postman.

---

### Hình ảnh minh chứng thực hiện tuần 4

#### 1. Khởi tạo bộ lọc dữ liệu (Metric Filter) trên CloudWatch
![Khởi tạo thành công Spring Boot Error Filter](/images/1-Worklog/Week4/Picture5.png)

#### 2. Thiết lập trạng thái Alarm ban đầu cho hệ thống Spring Boot Fargate
![Khởi tạo Alarm trạng thái ban đầu](/images/1-Worklog/Week4/Picture6.png)

#### 3. Xác nhận Đăng ký nhận thông báo (Subscription Confirmation) từ AWS
![Xác nhận Subscription thành công](/images/1-Worklog/Week4/Picture7.png)

#### 4. Hệ thống phát hiện lỗi và kích hoạt trạng thái báo động (In Alarm)
![CloudWatch Alarm chuyển sang trạng thái In Alarm](/images/1-Worklog/Week4/Picture8.png)

#### 5. Email thông báo chi tiết lỗi hệ thống thực tế gửi về hộp thư quản trị viên
![Email cảnh báo lỗi Spring Boot Fargate thực tế](/images/1-Worklog/Week4/Picture9.png)

#### 6. Họp nhóm
![Họp nhóm](/images/1-Worklog/Week4/1505_meeting_w4.JPG)