---
title: "Worklog Tuần 4"
date: 2026-05-14
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu tuần 4:
* Nắm vững lý thuyết cốt lõi về tự động co giãn hệ thống (Auto Scaling) và kiến trúc tính sẵn sàng cao (High Availability).
* Khởi tạo thành công Launch Template từ Amazon Machine Image (AMI) để làm khuôn mẫu chuẩn cho máy chủ.
* Triển khai cấu hình Auto Scaling Group (ASG) trong môi trường VPC và tích hợp linh hoạt với Elastic Load Balancing (ELB).
* Thiết lập chính sách co giãn tự động (Scaling Policies) dựa trên các ngưỡng kích hoạt của CloudWatch Alarms.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 6   | - Tìm hiểu lý thuyết về Auto Scaling, cơ chế Vertical vs Horizontal Scaling. <br> - Nghiên cứu nguyên lý thiết kế hệ thống có tính sẵn sàng cao (High Availability). | 08/05/2026   | 08/05/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 2   | - Tạo Amazon Machine Image (AMI) từ máy chủ EC2 hiện tại. <br> - Khởi tạo Launch Template cấu hình đầy đủ thông số (loại instance, key pair, security group) dựa trên AMI vừa tạo. | 11/05/2026   | 11/05/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 3   | - Cấu hình Auto Scaling Group (ASG) trong môi trường Custom VPC. <br> - Thiết lập các tham số tài nguyên cơ bản cho nhóm máy chủ (Desired, Minimum, Maximum capacity). | 12/05/2026   | 12/05/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - Thực hiện tích hợp cơ chế phân phối tải của Elastic Load Balancing (ELB) vào nhóm ASG. <br> - Tìm hiểu các loại Scaling Policies (Target Tracking, Step Scaling). | 13/05/2026   | 13/05/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - **Thực hành:** <br>Thiết lập chính sách co giãn tự động (Scaling Policies) dựa trên các ngưỡng cảnh báo của AWS CloudWatch Alarms và tiến hành test tải hệ thống. | 14/05/2026   | 14/05/2026      | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 4:
* **Tư duy kiến trúc:** Hiểu sâu sắc cách thức xây dựng hệ thống High Availability (Đa phân vùng Multi-AZ) để loại bỏ điểm lỗi đơn lẻ (Single Point of Failure).
* **Chuẩn hóa cấu hình:** Tạo thành công Launch Template hoàn chỉnh từ Custom AMI, giúp tự động hóa quá trình nhân bản máy chủ mà không cần cấu hình thủ công.
* **Tự động hóa hạ tầng:** Triển khai thành công Auto Scaling Group, quản lý hiệu quả số lượng máy chủ dựa trên nhu cầu thực tế của hạ tầng VPC.
* **Hệ thống co giãn linh hoạt:** Tích hợp trơn tru bộ đôi ASG và ELB; thiết lập các Scaling Policies kích hoạt chuẩn xác dựa theo tín hiệu cảnh báo CloudWatch Alarms khi hệ thống bị tăng/giảm tải.


