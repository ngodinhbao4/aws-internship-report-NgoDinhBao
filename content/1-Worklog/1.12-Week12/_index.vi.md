---
title: "Worklog Tuần 12"
date: 2026-07-09
weight: 1
chapter: false
pre: " <b> 1.12. </b> "
---

### Mục tiêu tuần 12:

* Tiến hành kiểm thử tích hợp (End-to-End Integration Testing) toàn diện hệ thống backend bao gồm luồng nghiệp vụ y tế, luồng giao dịch tài chính và quy trình xác thực chuỗi khối Blockchain.
* Tối ưu hóa cơ chế xử lý ngoại lệ (Exception Handling), củng cố bộ test suite và tổng hợp hệ thống tài liệu kỹ thuật hoàn chỉnh phục vụ nghiệm thu dự án.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 6 | - Kiểm thử luồng tích hợp nghiệp vụ y tế đầu cuối (E2E): Từ khâu đặt lịch, tiếp nhận, khám bệnh, ra y lệnh xét nghiệm, trả kết quả và cập nhật bệnh án. | 03/07/2026 | 03/07/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 2 | - Kiểm thử toàn diện luồng thanh toán thực tế (tạo URL, xử lý callback/IPN, đối soát chữ ký) và xác minh ghi nhận sự kiện thanh toán vào nội bộ ledger. | 06/07/2026 | 06/07/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Kiểm thử chức năng Blockchain: Kiểm tra tính liên tục của chuỗi hash, xác thực trạng thái VALID/INVALID và kiểm tra thông tin giao dịch trên AMB. | 07/07/2026 | 07/07/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Tập trung tối ưu hóa xử lý lỗi hệ thống (lỗi bảo mật, thiếu quyền, sai chữ ký gateway tài chính, lỗi kết nối RPC, lỗi thất bại transaction mạng lưới). | 08/07/2026 | 08/07/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - Viết bổ sung các bộ test case kiểm soát chất lượng (Regression tests); tổng hợp toàn bộ tài liệu kỹ thuật kiến trúc backend bàn giao dự án. | 09/07/2026 | 09/07/2026 | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 12:

* Hoàn thành kiểm thử đầu cuối hệ thống (E2E Testing) đạt độ ổn định cao:
  * Luồng nghiệp vụ y tế chạy mượt mà, dữ liệu không bị thất thoát hoặc sai lệch qua các bước luân chuyển.
  * Phân hệ thanh toán thực tế phản hồi chính xác, xử lý ngoại lệ sai lệch chữ ký hoặc sai số tiền giao dịch an toàn, ghi nhận log đầy đủ vào hệ thống Ledger bảo mật.
  * Kiểm tra và chứng minh được tính toàn vẹn dữ liệu y tế trên Blockchain; phát hiện và cô lập thành công các tác vụ giả mạo dữ liệu cố ý (Đánh dấu trạng thái INVALID chính xác).

* Tối ưu hóa kiến trúc và hoàn thiện hồ sơ dự án:
  * Hệ thống hóa cơ chế bắt lỗi tập trung (Global Exception Handling), nâng cao tính sẵn sàng và khả năng tự phục hồi của ứng dụng trước các lỗi kết nối dịch vụ bên thứ ba (Cổng thanh toán, AMB RPC Node).
  * Hoàn thành bộ tài liệu kỹ thuật backend chi tiết: Sơ đồ thực thể DynamoDB Single-Table, tài liệu API chi tiết, tài liệu phân tích luồng tích hợp AMB và quản lý Private Key an toàn.
  * Đóng hồ sơ và hoàn thành đúng hạn toàn bộ chương trình báo cáo tiến độ khóa học AWS FCAJ.