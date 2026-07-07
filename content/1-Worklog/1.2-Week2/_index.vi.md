---
title: "Worklog Tuần 2"
date: 2026-04-30
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---

### Mục tiêu tuần 2:

* Tìm hiểu kiến thức nền tảng về mạng (VPC, Subnet) và các phương thức kết nối Internet an toàn (IGW, NAT)
* Phân biệt và áp dụng thực tế các lớp bảo mật hạ tầng mạng (Security Groups & NACLs) và triển khai dịch vụ lưu trữ đối tượng (S3) và thiết lập cơ sở dữ liệu quan hệ (RDS).

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 6   | - Tìm hiểu các khái niệm và thiết lập VPC (Chia Subnet Public/Private).                                                                                             | 24/04/2026   | 24/04/2026      |
| 2   | - Tìm hiểu và cấu hình Internet Gateway & NAT Gateway.<br>                                            | 27/04/2026   | 27/04/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 3   | - So sánh và cấu hình Security Groups & NACLs.| 28/04/2026   | 28/04/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - Tìm hiểu S3 Bucket (Policies) & Thiết lập, quản lý RDS <br>                  | 29/04/2026   | 29/04/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - **Thực hành:** <br>Thực hành: Dựng kiến trúc mạng đa tầng (Multi-tier network architecture).                                                                                       | 30/04/2026   | 30/04/2026      | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 2:

* Nắm vững kiến thức cốt lõi về mạng trên AWS và tự tay thiết lập hệ thống mạng tùy chỉnh bao gồm:

  * Khởi tạo VPC, phân chia dải IP (CIDR Block).
  * Thiết lập và phân biệt rõ ràng giữa Public Subnet và Private Subnet.
  * Cấu hình Route Table (Bảng định tuyến) cho từng vùng mạng.
* Cấu hình thành công các phương thức kết nối mạng và điều hướng luồng dữ liệu:
  * Cài đặt Internet Gateway (IGW) để mở đường kết nối ra ngoài cho Public Subnet.
  * Triển khai NAT Gateway/NAT Instance tại Public Subnet để giúp máy ảo ở Private Subnet cập nhật Internet an toàn.
* Khả năng làm chủ và áp dụng linh hoạt các lớp bảo mật hạ tầng mạng:
  * Phân biệt rõ cơ chế hoạt động của Security Groups (Stateful - mức Instance) và NACLs (Stateless - mức Subnet).
  * Thiết lập các luật Inbound/Outbound chuẩn bảo mật để cô lập và bảo vệ tài nguyên.

* Quản lý thành công dịch vụ Lưu trữ và Cơ sở dữ liệu:
  * Tạo S3 Bucket, hiểu cách cấu hình các chính sách (Bucket Policies) để phân quyền truy cập tập tin.
  * Khởi tạo, quản lý và kết nối hệ quản trị cơ sở dữ liệu quan hệ Amazon RDS (MySQL/PostgreSQL) đặt an toàn trong Private Subnet.

