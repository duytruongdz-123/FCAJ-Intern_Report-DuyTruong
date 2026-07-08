---
title: "Worklog Tuần 1"
date: 2026-04-20
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---



### Mục tiêu tuần 1:

* Thiết lập hệ thống giám sát log bảo mật và phát hiện bất thường tự động bằng AWS CloudWatch.
* Cấu hình luồng cảnh báo bảo mật theo thời gian thực qua Amazon SNS để thông báo cho quản trị viên khi có tấn công.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | ------------ | --------------- | ----------------------------------------- |
| 2 | - Đẩy các tệp log hệ thống và ứng dụng từ EC2 vào CloudWatch Logs | 20/04/2026 | 20/04/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Tạo Log Group trên CloudWatch Logs <br> - Cấu hình bộ lọc Metric Filter tổng quát với cú pháp `{ $.type = "SECURITY" }` để bắt toàn bộ sự kiện bảo mật | 21/04/2026 | 21/04/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Thiết lập chi tiết các bộ lọc Metric Filter nhằm đếm từng loại tấn công: <br> &emsp; + SQL Injection: `{ $.msg = "*type=SQL_INJECTION*" }` <br> &emsp; + XSS: `{ $.msg = "*type=XSS_ATTACK*" }` <br> &emsp; + Path Traversal: `{ $.msg = "*type=PATH_TRAVERSAL*" }` <br> - Cấu hình Metric value là 1 và Default value là 0 | 22/04/2026 | 22/04/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - Khởi tạo một Amazon SNS Topic loại Standard với tên `Security-Alerts` <br> - Tạo Subscription chọn giao thức Email hướng tới địa chỉ `duytruongsb30@gmail.com` <br> - Thực hiện đăng nhập hòm thư để nhấn Confirm Subscription kích hoạt luồng nhận tin | 23/04/2026 | 23/04/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - Khởi tạo CloudWatch Alarm liên kết với metric `SecurityAttackCount` vừa tạo <br> - Thiết lập ngưỡng kích hoạt báo động lớn hơn hoặc bằng 1 trong vòng 1 phút <br> - Cấu hình hành động gửi thông báo tới SNS Topic `Security-Alerts` khi trạng thái chuyển sang `In Alarm` | 24/04/2026 | 24/04/2026 | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 1:

* Xây dựng thành công đường ống tập trung log từ máy chủ EC2 về CloudWatch Logs.
* Làm chủ cú pháp lọc dữ liệu trong Metric Filter để nhận diện và phân loại chính xác các hành vi tấn công web nguy hiểm (SQLi, XSS, Path Traversal).
* Triển khai hoàn chỉnh hạ tầng thông báo khẩn cấp Amazon SNS và xác thực thành công hòm thư tiếp nhận.
* Cài đặt thành công cơ chế tự động kích hoạt trạng thái `In Alarm` của CloudWatch khi xuất hiện dấu hiệu xâm nhập, giúp rút ngắn thời gian phản ứng sự cố.
* Xác thực tính toàn vẹn của mô hình luồng kết nối: `[Log File] -> [CloudWatch Metric Filter] -> [Alarm] -> [SNS Topic] -> [Admin Email]`.

---

### Hình ảnh minh chứng thực hiện tuần 1

#### 1. Họp nhóm online trên Google Meet
![Họp meeting online](/images/1-Worklog/Week1/2604_meetingOnl_w1.png)