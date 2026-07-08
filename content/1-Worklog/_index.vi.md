---
title: "Nhật ký công việc"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1. </b> "
---



<style>
  .force-justify-align, 
  .force-justify-align p, 
  .force-justify-align ul, 
  .force-justify-align li {
    text-align: justify !important;
  }
</style>

<div class="force-justify-align">

Chào mừng bạn đến với Nhật ký công việc (Worklog) của mình. Trang tài liệu này tổng hợp lại toàn bộ hành trình nghiên cứu, triển khai và tối ưu hóa hệ thống giám sát trong suốt 3 tháng (12 tuần) thực hiện dự án. Mình đã tập trung hoàn toàn vào việc xây dựng, vận hành và quản lý hệ thống đo lường hiệu suất cũng như cảnh báo trên môi trường điện toán đám mây.

Lộ trình công việc được thiết kế từ cơ bản đến nâng cao: bắt đầu bằng việc làm quen với các dịch vụ AWS cốt lõi, sau đó đi sâu vào thiết lập và tích hợp hệ thống giám sát toàn diện, sử dụng hai công cụ chủ lực là Amazon CloudWatch và Grafana.

Dưới đây là chi tiết các hạng mục công việc được thực hiện theo từng tuần:

* **Tuần 1:** [Làm quen AWS và các dịch vụ cơ bản](1.1-week1/)
* **Tuần 2:** [Cấu hình CloudWatch Agent & Giám sát bảo mật](1.2-week2/)
* **Tuần 3:** [Triển khai SNS & Thông báo Email](1.3-week3/)
* **Tuần 4:** [Metric Filters & Cấu hình Cảnh báo](1.4-week4/)
* **Tuần 5:** [Chính sách IAM & Thiết lập nguồn dữ liệu Grafana](1.5-week5/)
* **Tuần 6:** [Tích hợp đo lường OpenTelemetry](1.6-week6/)
* **Tuần 7:** [Triển khai Container trên ECS Fargate](1.7-week7/)
* **Tuần 8:** [Kiểm thử tải K6 & Prometheus Remote Write](1.8-week8/)
* **Tuần 9:** [Tích hợp APM & Cập nhật Rolling trên ECS](1.9-week9/)
* **Tuần 10:** [Tích hợp CloudWatch đa tầng](1.10-week10/)
* **Tuần 11:** [Tối ưu hóa Stress Test & Kiểm toán lưu lượng](1.11-week11/)
* **Tuần 12:** [Giám sát hệ thống & Phân tích Log CloudWatch](1.12-week12/)

</div>