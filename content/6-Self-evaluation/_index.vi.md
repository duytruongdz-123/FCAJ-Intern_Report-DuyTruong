---
title: "Tự Đánh Giá"
date: 2024-01-01
weight: 6
chapter: false
pre: " <b> 6. </b> "
---

Trong suốt thời gian thực tập tại chương trình Bootcamp từ ngày 20 tháng 4 năm 2026 đến ngày 12 tháng 7 năm 2026, tôi đã có cơ hội thực thi toàn diện chuỗi lộ trình từ Task 1 đến Task 12. Quá trình này giúp tôi chuyển hóa sâu sắc các kiến thức nền tảng về mạng máy tính và hệ thống thành năng lực triển khai thực tế trên môi trường điện toán đám mây AWS và nền tảng giám sát tập trung Grafana Cloud.

Xuyên suốt các nội dung công việc, tôi đã trực tiếp làm chủ các kỹ năng cốt lõi bao gồm: thiết lập hạ tầng giám sát và cảnh báo bảo mật tự động (sử dụng CloudWatch Logs, Metric Filters phát hiện tấn công và kích hoạt Alarms qua Amazon SNS về Email); cấu hình ứng dụng container hóa quy mô doanh nghiệp trên hạ tầng AWS ECS Fargate (tối ưu hóa Task Definition tích hợp các biến môi trường OpenTelemetry OTel và JVM Micrometer để thu thập dữ liệu APM sâu tầng ứng dụng); cho đến Kỹ nghệ hiệu năng hệ thống.

Đặc biệt, tại giai đoạn cuối, tôi đã tự tay xây dựng khu vực giám sát chuyên biệt "Stress Test Panel" trên Grafana, đồng bộ dữ liệu đa tầng từ bộ cân bằng tải ALB (RequestCount, lỗi HTTPCode_Target_5XX_Count và HTTPCode_ELB_5XX_Count), tài nguyên ứng dụng ECS (CPUUtilization, MemoryUtilization) cho tới số lượng kết nối cơ sở dữ liệu RDS (DatabaseConnections trên instance minisocial-sqlserver). Hệ thống đã được kiểm thử áp lực thành công thông qua kịch bản k6 script nâng tải lên đến 200 VUs, đẩy số liệu thời gian thực qua cơ chế Prometheus Remote Write để trực quan hóa dữ liệu và kích hoạt hệ thống Alert Rules cảnh báo vượt ngưỡng.

Về tác phong làm việc, tôi luôn duy trì tính kỷ luật cao, đảm bảo đúng tiến độ đề ra của từng task, phối hợp hiệu quả cùng các thành viên trong nhóm và chủ động trao đổi với Mentor để hoàn thiện giải pháp kỹ thuật tối ưu nhất.

Để đưa ra cái nhìn khách quan về chuỗi trải nghiệm thực tế từ Task 1 đến Task 12 này, tôi tự đánh giá bản thân dựa trên các tiêu chí sau: 


| STT | Tiêu chí                            | Mô tả                                                                                            | Tốt | Khá | TB  |
| --- | ----------------------------------- | ------------------------------------------------------------------------------------------------ | --- | --- | --- |
| 1   | **Kiến thức & kỹ năng chuyên môn** | Hiểu biết về lĩnh vực, áp dụng kiến thức vào thực tế, thành thạo công cụ, chất lượng công việc   | ✅   | ☐   | ☐   |
| 2   | **Khả năng học hỏi** | Khả năng tiếp thu kiến thức mới và học hỏi nhanh chóng                                           | ✅   | ☐   | ☐   |
| 3   | **Sự chủ động** | Chủ động trong công việc, tìm kiếm nhiệm vụ mà không cần đợi hướng dẫn                           | ✅   | ☐   | ☐   |
| 4   | **Tinh thần trách nhiệm** | Hoàn thành công việc đúng hạn và đảm bảo chất lượng                                              | ✅   | ☐   | ☐   |
| 5   | **Kỷ luật** | Tuân thủ thời gian, nội quy và quy trình làm việc                                                | ✅   | ☐   | ☐   |
| 6   | **Tinh thần cầu tiến** | Sẵn sàng tiếp nhận phản hồi và hoàn thiện bản thân                                               | ✅   | ☐   | ☐   |
| 7   | **Kỹ năng giao tiếp** | Trình bày ý tưởng và báo cáo công việc rõ ràng                                                   | ☐   | ✅   | ☐   |
| 8   | **Làm việc nhóm** | Làm việc hiệu quả với đồng nghiệp và tích cực tham gia các hoạt động nhóm                        | ✅   | ☐   | ☐   |
| 9   | **Tác phong chuyên nghiệp** | Tôn trọng đồng nghiệp, đối tác và môi trường làm việc                                            | ✅   | ☐   | ☐   |

### Cần cải thiện

*   **Kỹ năng giao tiếp (Communication):** Cần tối ưu hóa phương pháp truyền đạt thông qua việc cô đọng các luồng phân tích kỹ thuật phức tạp, chủ động cập nhật tiến độ công việc và giải pháp cốt lõi một cách ngắn gọn để Mentor cũng như các thành viên trong nhóm dễ dàng nắm bắt, đưa ra phản hồi nhanh nhất.
*   **Tư duy giải quyết vấn đề (Problem Solving):** Cần hình thành một quy trình chẩn đoán lỗi có cấu trúc chặt chẽ hơn khi xử lý dữ liệu log tập trung, giúp tăng tốc độ khoanh vùng phạm vi ảnh hưởng và rút ngắn thời gian cô lập các sự cố phát sinh trên hạ tầng phân tán.