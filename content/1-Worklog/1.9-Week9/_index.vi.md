---
title: "Worklog Tuần 9"
date: 2026-06-18
weight: 1
chapter: false
pre: " <b> 1.9. </b> "
---

### Mục tiêu tuần 9:

* Phân tích luồng nghiệp vụ backend toàn diện cho hệ thống quản lý bệnh viện đa tầng và thiết kế cấu trúc cơ sở dữ liệu DynamoDB Single-table cho toàn bộ thực thể.
* Nghiên cứu giải pháp tích hợp cổng thanh toán trực tuyến (VNPay/MoMo) và thiết kế kiến trúc bảo mật toàn vẹn dữ liệu hồ sơ y tế sử dụng Amazon Managed Blockchain (AMB) / Ethereum.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 6 | - Phân tích nghiệp vụ backend cho toàn bộ luồng bệnh viện từ đăng ký, khám bệnh, xét nghiệm, kê đơn cho đến lập hóa đơn và thanh toán. | 12/06/2026 | 12/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 2 | - Thiết kế domain backend trên DynamoDB single-table; định nghĩa cấu trúc phân vùng cho các loại thực thể (USER, PATIENT, DOCTOR, INVOICE, MEDICAL_LEDGER_BLOCK,...). | 15/06/2026 | 15/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Xác định chuẩn hóa các khóa dữ liệu `pk`/`sk` và các trường liên kết hệ thống (patientId, citizenId, recordId, doctorId, appointmentId,...) để tối ưu truy vấn theo vai trò. | 16/06/2026 | 16/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Lập kế hoạch chuyển đổi mã hồ sơ bệnh án cũ sang định danh CCCD làm gốc, đảm bảo các tài liệu y tế liên quan đều trỏ chung về một `recordId` thống nhất. | 17/06/2026 | 17/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - Phân tích đặc tả kỹ thuật API thanh toán VNPay/MoMo (paymentUrl, IPN/callback); thiết kế luồng băm hash tài liệu y tế để đẩy lên Blockchain qua dịch vụ AMB. | 18/06/2026 | 18/06/2026 | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 9:

* Hoàn thành phân tích nghiệp vụ và kiến trúc dữ liệu DynamoDB Single-Table:
  * Đặc tả thành công luồng xử lý dữ liệu liên tầng của 12 thực thể cốt lõi trong hệ thống quản lý bệnh viện.
  * Thiết lập bảng ánh xạ các mẫu truy vấn (Access Patterns) tương ứng với các cặp khóa `pk`/`sk`, hỗ trợ tối ưu hóa hiệu năng và chi phí đọc/ghi trên DynamoDB.
  * Đồng bộ hóa kiến trúc định danh hồ sơ bệnh án dựa trên CCCD (`citizenId`), giải quyết triệt để vấn đề phân mảnh dữ liệu lịch sử khám bệnh.

* Thiết kế thành công giải pháp tích hợp thanh toán và bảo mật Blockchain:
  * Xây dựng sơ đồ tuần tự (Sequence Diagram) cho luồng giao dịch qua cổng VNPay/MoMo, xác định rõ quy trình xử lý chữ ký bảo mật và cơ chế nhận tin IPN.
  * Hoàn thiện mô hình toán học băm dữ liệu (Payload Hashing) và thiết kế cấu trúc khối nội bộ trước khi thực hiện neo dữ liệu lên mạng lưới Ethereum thông qua Amazon Managed Blockchain (AMB).