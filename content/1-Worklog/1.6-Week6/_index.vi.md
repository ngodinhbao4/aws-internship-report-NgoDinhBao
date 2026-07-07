---
title: "Worklog Tuần 6"
date: 2026-05-28
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu tuần 6:

* Tìm hiểu cơ chế truyền thông điệp mã nguồn mở, phi tập trung và quản lý sự kiện thời gian thực thông qua các dịch vụ Amazon SQS, Amazon SNS và Amazon EventBridge.
* Nghiên cứu cách xây dựng quy trình nghiệp vụ tự động (Workflows) phức tạp bằng AWS Step Functions và thực hành triển khai kiến trúc hướng sự kiện (Event-driven Architecture) để tối ưu hóa khả năng giao tiếp bất đồng bộ trong hệ thống Cloud.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 6 | - Tìm hiểu lý thuyết cốt lõi, cơ chế truyền thông điệp (Messaging) và phân biệt giữa dịch vụ Amazon SQS (Simple Queue Service) và Amazon SNS (Simple Notification Service). | 22/05/2026 | 22/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 2 | - Nghiên cứu giải pháp bus sự kiện (Event Bus), định tuyến và quản lý các sự kiện thời gian thực bằng Amazon EventBridge. | 25/05/2026 | 25/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Tìm hiểu cách xây dựng, phối hợp và quản lý các quy trình nghiệp vụ tự động (Workflows/State Machines) sử dụng dịch vụ AWS Step Functions. | 26/05/2026 | 26/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - **Thực hành:** <br>Thiết kế và triển khai mô hình kiến trúc hướng sự kiện (Event-driven Architecture) kết hợp SQS, SNS và EventBridge để xử lý luồng dữ liệu bất đồng bộ. | 27/05/2026 | 27/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - Tối ưu hóa kiến trúc, kiểm thử khả năng chịu tải (Decoupling) của hệ thống, hoàn thiện tài liệu kỹ thuật và tổng hợp báo cáo tiến độ tuần 6. | 28/05/2026 | 28/05/2026 | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 6:

* Nắm vững tư duy kiến trúc hướng sự kiện (Event-driven Architecture) và các dịch vụ Messaging cốt lõi:
  * Phân biệt rõ ràng cơ chế hoạt động của Amazon SQS (Message Queue - mô hình Pull) và Amazon SNS (Pub/Sub - mô hình Push).
  * Hiểu cách kết hợp SNS và SQS (Mô hình Fan-out) để truyền tải thông điệp song song đến nhiều thành phần xử lý độc lập.

* Làm chủ giải pháp quản lý sự kiện và điều phối quy trình tự động:
  * Cấu hình thành công các quy tắc định tuyến (Rules) trên Amazon EventBridge để chụp và điều hướng các sự kiện hệ thống theo thời gian thực một cách chính xác.
  * Thiết kế được các chuỗi trạng thái (State Machines) trực quan bằng AWS Step Functions, xử lý tốt các logic rẽ nhánh, vòng lặp và quản lý lỗi (Error handling) trong quy trình nghiệp vụ.

* Triển khai thực hành thành công hệ thống phi tập trung (Decoupled System):
  * Tự tay xây dựng hoàn chỉnh một mô hình Event-driven tích hợp mượt mà bộ ba SQS, SNS và EventBridge.
  * Giảm thiểu thành công sự phụ thuộc trực tiếp (Tight coupling) giữa các microservices, giúp hệ thống tăng khả năng mở rộng (Scalability) và tối ưu độ tin cậy khi có sự cố tại từng thành phần.

* Hoàn thiện tài liệu và kỹ năng chuyên môn:
  * Đánh giá và đo lường thành công độ trễ, luồng đi của dữ liệu bất đồng bộ để hoàn thiện tài liệu kiến trúc vận hành.
  * Hoàn thành đúng hạn báo cáo tiến độ tuần 6 của khóa học AWS FCAJ.