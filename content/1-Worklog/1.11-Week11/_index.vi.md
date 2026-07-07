---
title: "Worklog Tuần 11"
date: 2026-07-02
weight: 1
chapter: false
pre: " <b> 1.11. </b> "
---

### Mục tiêu tuần 11:

* Giải quyết triệt để lỗi đồng bộ dữ liệu hồ sơ bệnh án, hoàn thiện phân hệ xử lý giao dịch thanh toán trực tuyến thời gian thực với VNPay/MoMo.
* Xây dựng module kiểm tra tính toàn vẹn dữ liệu y tế (Medical Integrity Ledger), phát triển cơ chế backfill khối dữ liệu và triển khai tích hợp gửi giao dịch lên mạng lưới AMB/Ethereum.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 6 | - Sửa lỗi bất đồng bộ mã hồ sơ bệnh án giữa Backend và Frontend, chuẩn hóa việc ưu tiên sử dụng `recordId`/`citizenId` theo định dạng CCCD. | 26/06/2026 | 26/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 2 | - Hoàn thiện mã nguồn backend xử lý thanh toán thực qua VNPay/MoMo (tạo link thanh toán, mã hóa dữ liệu với Checksum Key, xử lý IPN/Callback). | 29/06/2026 | 29/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Triển khai logic xác minh thanh toán nâng cao (xác thực chữ ký, số tiền, mã hóa đơn) và cập nhật đồng bộ trạng thái PAYMENT, INVOICE, APPOINTMENT. | 30/06/2026 | 30/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Thiết kế và xây dựng module Medical Integrity Ledger (chuẩn hóa payload, tính toán chuỗi hash liên kết `previousHash` - `blockHash`). | 01/07/2026 | 01/07/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - Xây dựng cơ chế backfill dữ liệu ledger từ dataset có sẵn; tích hợp gọi RPC URL, lấy Private Key bảo mật từ AWS Secrets Manager để ký và đẩy transaction lên AMB. | 02/07/2026 | 02/07/2026 | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 11:

* Khắc phục lỗi hệ thống và hoàn thiện phân hệ thanh toán trực tuyến:
  * Xử lý dứt điểm lỗi hiển thị sai lệch mã hồ sơ y tế, đưa `citizenId` (CCCD) thành khóa định danh gốc xuyên suốt các thực thể liên quan.
  * Tích hợp thành công bộ mã hóa SHA256/HMAC để ký số các cổng giao dịch, xử lý mượt mà dữ liệu trả về từ `returnUrl` và webhook `IPN`, cập nhật trạng thái giao dịch đồng bộ theo thời gian thực.

* Triển khai thành công cấu trúc Ledger và tích hợp Blockchain đám mây:
  * Xây dựng thành công hệ thống khối nội bộ (Internal Ledger) liên kết dạng chuỗi, chống giả mạo cho các tài liệu y tế phát sinh.
  * Phát triển thành công tính năng backfill dữ liệu khối từ kho dữ liệu cũ sau mỗi chu kỳ reset dataset.
  * Tích hợp thành công module tương tác Web3, lấy thông tin xác thực an toàn từ AWS Secrets Manager để thực hiện gửi transaction neo dữ liệu lên Amazon Managed Blockchain, lưu vết thành công `transactionHash` và `blockNumber`.