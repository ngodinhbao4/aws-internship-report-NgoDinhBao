---
title: "Worklog Tuần 7"
date: 2026-06-04
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu tuần 7:

* Tìm hiểu các khái niệm cơ bản về công nghệ đóng gói ứng dụng bằng Docker (Container, Image, Dockerfile) và dịch vụ lưu trữ Amazon ECR.
* Nghiên cứu kiến trúc, cơ chế quản lý cụm container bằng Amazon ECS và thực hành đóng gói, đẩy image lên ECR, từ đó triển khai ứng dụng web thực tế trên hạ tầng Amazon ECS.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 5 | - Tìm hiểu các khái niệm cốt lõi về Docker (Container, Image, Dockerfile); viết thử nghiệm Dockerfile để đóng gói ứng dụng. | 29/05/2026 | 29/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 2 | - Nghiên cứu dịch vụ Amazon ECR; thực hành khởi tạo kho lưu trữ riêng tư (Private Repository) và quản lý các Docker Image. | 01/06/2026 | 01/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Tìm hiểu kiến thức nền tảng và thành phần kiến trúc của Amazon ECS (Cluster, Task Definition, Service, Fargate/EC2 launch type). | 02/06/2026 | 02/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - **Thực hành:** <br>Đóng gói ứng dụng web hoàn chỉnh thành Docker Image, thực hiện tag và đẩy (push) image lên Amazon ECR. | 03/06/2026 | 03/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - **Thực hành:** <br>Triển khai, chạy thực tế ứng dụng web trên Amazon ECS từ image trên ECR; hoàn thiện tài liệu kỹ thuật và nộp báo cáo tuần 7. | 04/06/2026 | 04/06/2026 | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 7:

* Làm chủ công nghệ Container hóa (Containerization) cơ bản với Docker:
  * Hiểu rõ cơ chế hoạt động và cách phân biệt giữa Docker Image và Docker Container.
  * Tự viết thành công Dockerfile chuẩn hóa để đóng gói ứng dụng web gọn nhẹ, tối ưu dung lượng layer.

* Thành thạo quy trình lưu trữ và quản lý Image trên AWS Cloud:
  * Khởi tạo thành công Private Repository trên Amazon ECR.
  * Sử dụng thành thạo AWS CLI để xác thực (login), gắn thẻ (tag) và đẩy (push) Docker Image từ môi trường local lên ECR an toàn.

* Nắm vững kiến thức kiến trúc và triển khai ứng dụng trên Amazon ECS:
  * Phân biệt rõ ràng các khái niệm trong hệ sinh thái ECS bao gồm: Task Definition (bản thiết kế), Task (thực thể chạy), Service (quản lý số lượng task) và Cluster.
  * Hiểu rõ sự khác biệt và ưu nhược điểm giữa hai loại Launch Type: Amazon EC2 và AWS Fargate (Serverless).

* Triển khai thực tế và hoàn thiện kỹ năng:
  * Cấu hình và chạy thành công ứng dụng web trên hạ tầng ECS (Fargate/EC2), kiểm tra ứng dụng hoạt động ổn định thông qua IP/DNS được cấp phát.
  * Hoàn thành đúng hạn tài liệu hướng dẫn vận hành container và báo cáo tiến độ tuần 7 của khóa học AWS FCAJ.