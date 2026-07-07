---
title: "Worklog Tuần 8"
date: 2026-06-11
weight: 1
chapter: false
pre: " <b> 1.8. </b> "
---

### Mục tiêu tuần 8:

* Tìm hiểu khái niệm cốt lõi và quy trình thiết lập chu trình Tích hợp liên tục / Triển khai liên tục (CI/CD) trên môi trường điện toán đám mây AWS.
* Nghiên cứu và thực hành phối hợp bộ ba công cụ AWS CodePipeline, AWS CodeBuild và AWS CodeDeploy nhằm tự động hóa hoàn toàn các giai đoạn từ biên dịch, đóng gói đến triển khai ứng dụng, đảm bảo khả năng cập nhật không gây gián đoạn hệ thống (Zero-downtime deployment).

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 5 | - Tìm hiểu lý thuyết tổng quan về CI/CD; nghiên cứu cách lập lịch và tự động hóa quy trình phát hành phần mềm trên AWS. | 05/06/2026 | 05/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 2 | - Tìm hiểu dịch vụ AWS CodeBuild; viết file cấu hình `buildspec.yml` để tự động hóa quá trình biên dịch mã nguồn và đóng gói ứng dụng. | 08/06/2026 | 08/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Nghiên cứu dịch vụ AWS CodeDeploy; viết file cấu hình `appspec.yml` và tìm hiểu các chiến lược triển khai an toàn (In-place, Blue/Green). | 09/06/2026 | 09/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - **Thực hành:** <br>Cấu hình AWS CodePipeline để kết nối các giai đoạn (Source, Build, Deploy) thành một luồng tự động hóa hoàn chỉnh từ kho lưu trữ. | 10/06/2026 | 10/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - **Thực hành:** <br>Tiến hành thay đổi mã nguồn để kích hoạt tự động pipeline; kiểm thử tính năng cập nhật ứng dụng không gây gián đoạn và nghiệm thu báo cáo tuần 8. | 11/06/2026 | 11/06/2026 | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 8:

* Nắm vững tư duy thiết kế chuỗi cung ứng phần mềm tự động (Automated Software Release Pipeline):
  * Hiểu rõ vai trò từng giai đoạn trong một mô hình CI/CD tiêu chuẩn trên đám mây và lợi ích của việc tự động hóa hạ tầng kiểm thử/triển khai.
  * Phân biệt rõ ràng chức năng độc lập và cách liên kết giữa ba dịch vụ: CodeBuild (CI), CodeDeploy (CD) và CodePipeline (Bộ điều phối).

* Làm chủ kỹ năng cấu hình và đóng gói mã nguồn tự động với AWS CodeBuild:
  * Tự tay viết và tối ưu hóa thành công file cấu hình `buildspec.yml` để định nghĩa môi trường chạy, cài đặt các package phụ thuộc và biên dịch ứng dụng ra các artifact sẵn sàng triển khai.

* Triển khai ứng dụng an toàn với AWS CodeDeploy:
  * Cấu hình chính xác file `appspec.yml` nhằm quản lý các vòng đời triển khai (Deployment lifecycle hooks) của ứng dụng trên hạ tầng (EC2/ECS).
  * Hiểu và áp dụng thành công cơ chế triển khai giảm thiểu rủi ro, hướng tới mục