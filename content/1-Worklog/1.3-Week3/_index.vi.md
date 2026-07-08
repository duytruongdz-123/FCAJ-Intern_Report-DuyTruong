---
title: "Worklog Tuần 3"
date: 2026-05-04
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---


### Mục tiêu tuần 3:

* Nghiên cứu cơ chế hoạt động và các mô hình truyền tin của dịch vụ AWS SNS (Simple Notification Service).
* Xây dựng và xác thực luồng gửi nhận thông báo tự động từ hệ thống đám mây về hộp thư email.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | ------------ | --------------- | ----------------------------------------- |
| 2 | - Tìm hiểu tổng quan kiến trúc AWS SNS, phân biệt các đặc tính giữa Standard Topic và FIFO Topic | 04/05/2026 | 04/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Khởi tạo một AWS SNS Topic sử dụng loại Standard để đảm bảo khả năng tương thích tối đa với phương thức gửi qua email | 05/05/2026 | 05/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Thiết lập một Subscription liên kết với email cá nhân để đăng ký nhận thông báo từ Topic vừa tạo | 06/05/2026 | 06/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - Tiến hành truy cập vào hòm thư điện tử cá nhân để thực hiện thủ tục xác nhận bắt buộc (Confirm Subscription) | 07/05/2026 | 07/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - Sử dụng tính năng Publish Message trực tiếp trên AWS Management Console để giả lập gửi thông báo thử nghiệm <br> - Kiểm tra và đánh giá độ ổn định của luồng gửi nhận email tự động | 08/05/2026 | 08/05/2026 | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 3:

* Nắm vững nguyên lý cấu hình và tích hợp các điểm cuối (endpoints) nhận tin của dịch vụ AWS SNS.
* Triển khai thành công hạ tầng SNS Standard Topic đáp ứng yêu cầu truyền thông tin báo động nhanh chóng.
* Hoàn thành quy trình quản lý vòng đời subscription, đảm bảo tính bảo mật và cấp quyền nhận dữ liệu chính xác cho email.
* Xác thực thành công luồng truyền tin khép kín thông qua việc xuất bản và nhận thông điệp kiểm thử trực quan trên console.

---

### Hình ảnh minh chứng thực hiện tuần 3

#### 1. Khởi tạo Amazon SNS Topic thành công
![Khởi tạo SNS Topic thành công](/images/1-Worklog/Week3/Picture1.png)

#### 2. Danh sách Subscriptions trong Amazon SNS hiển thị trạng thái đã xác nhận
![Trạng thái Subscription đã Confirmed](/images/1-Worklog/Week3/Picture2.png)

#### 3. Giao diện xác nhận Đăng ký dịch vụ thành công từ AWS
![Xác nhận đăng ký dịch vụ thành công](/images/1-Worklog/Week3/Picture3.png)

#### 4. Kiểm tra Email thông báo Test kết nối thành công từ hệ thống AWS SNS
![Kiểm tra Email thông báo từ AWS SNS](/images/1-Worklog/Week3/Picture4.png)