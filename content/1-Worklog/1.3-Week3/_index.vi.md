---
title: "Worklog Tuần 3"
date: 2026-05-07
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---
### Mục tiêu tuần 3:

* Tìm hiểu và triển khai giải pháp điều phối lưu lượng mạng tự động bằng Elastic Load Balancing (ELB).
* Làm chủ dịch vụ giám sát hệ thống AWS CloudWatch (Thiết lập Dashboard và cấu hình cảnh báo Alarms).
* Quản trị định danh, phân quyền và bảo mật tài khoản nâng cao với AWS Identity and Access Management (IAM).

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 6   | - Tìm hiểu khái niệm, phân loại các dòng Load Balancer (ALB, NLB, CLB). <br> - Cấu hình Target Group và triển khai Elastic Load Balancing (ELB). | 01/05/2026   | 01/05/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 2   | - Tìm hiểu dịch vụ AWS CloudWatch (Metrics, Logs). <br> - Thiết lập Dashboard giám sát trực quan cho tài nguyên hệ thống (EC2, ELB). | 04/05/2026   | 04/05/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 3   | - Cấu hình hệ thống cảnh báo tự động (CloudWatch Alarms). <br> - Kết nối thông báo qua Amazon SNS (Simple Notification Service) về Email. | 05/05/2026   | 05/05/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - Quản trị định danh và truy cập (IAM): Tìm hiểu IAM User, Group, Role và Policy. <br> - Áp dụng nguyên tắc đặc quyền tối thiểu (Least Privilege). | 06/05/2026   | 06/05/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - **Thực hành:** <br>Cấu hình ELB phân phối tải cho cụm Web Server, thiết lập CloudWatch cảnh báo khi CPU quá tải, và phân quyền IAM Roles bảo mật cho EC2. | 07/05/2026   | 07/05/2026      | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 3:
* **Cân bằng tải:** Triển khai thành công Elastic Load Balancing (ELB/ALB) để tự động điều phối lưu lượng truy cập, tối ưu khả năng chịu tải của cụm máy chủ.
* **Giám sát hệ thống:** Tự tay thiết lập CloudWatch Dashboard trực quan hóa các thông số vận hành (CPU, Network, Memory) theo thời gian thực.
* **Cảnh báo tự động:** Cấu hình thành công CloudWatch Alarms tự động kích hoạt và gửi email cảnh báo (qua SNS) khi tài nguyên hệ thống gặp sự cố hoặc quá tải.
* **Quản trị bảo mật:** Sử dụng thành thạo IAM để khởi tạo User, Group, phân rã quyền hạn bằng Policies và gán IAM Role an toàn cho EC2 instance mà không cần dùng Access Key bừa bãi.