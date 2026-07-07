---
title: "Worklog Tuần 10"
date: 2026-06-25
weight: 1
chapter: false
pre: " <b> 1.10. </b> "
---

### Mục tiêu tuần 10:

* Triển khai xây dựng hệ thống API backend nền tảng phục vụ các phân hệ chức năng cho Bệnh nhân, Bác sĩ, Hồ sơ y tế và phân hệ Hóa đơn ban đầu.
* Cấu hình phân quyền truy cập hệ thống dựa trên Cognito User Group và chuẩn bị dữ liệu mẫu (Seed data) phục vụ kiểm thử tích hợp.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 6 | - Tri triển khai nhóm API nền tảng cho bệnh nhân và người dùng (lấy thông tin hiện tại, cập nhật hồ sơ cá nhân, đặt và xem lịch hẹn). | 19/06/2026 | 19/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 2 | - Phát triển các endpoint cho phân hệ Bác sĩ bao gồm: Đăng ký lịch làm việc, quản lý hàng chờ khám, tìm kiếm dữ liệu bệnh án qua CCCD. | 22/06/2026 | 22/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Xây dựng hệ thống API nghiệp vụ y tế cốt lõi: Lập phiếu khám, kê đơn thuốc và tạo yêu cầu xét nghiệm gắn chặt với định danh `recordId`. | 23/06/2026 | 23/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Phát triển phân hệ API hóa đơn ban đầu (tạo hóa đơn từ lịch hẹn/dịch vụ, quản lý danh sách trạng thái chờ/đã thanh toán). | 24/06/2026 | 24/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - Cấu hình kiểm tra quyền truy cập API (RBAC) thông qua Amazon Cognito Group; viết script seed dữ liệu mẫu và kiểm tra bằng AWS CLI. | 25/06/2026 | 25/06/2026 | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 10:

* Hoàn thành xây dựng và đóng gói hệ thống API nghiệp vụ lõi:
  * Triển khai thành công chuỗi API cho Bệnh nhân và Bác sĩ, đảm bảo các luồng thông tin vận hành đúng tiến độ (quản lý hàng chờ, tra cứu hồ sơ theo định danh CCCD).
  * Đóng gói các endpoint nghiệp vụ y tế (Phiếu khám, đơn thuốc, xét nghiệm), đảm bảo lưu trữ đầy đủ siêu dữ liệu (metadata) liên kết đa bên.
  * Phát triển hoàn chỉnh phân hệ quản lý trạng thái hóa đơn ban đầu trên DynamoDB.

* Tối ưu hóa bảo mật và kiểm thử dữ liệu:
  * Tích hợp thành công bộ lọc Authorizer sử dụng Amazon Cognito Groups, phân định rạch ròi quyền hạn giữa các nhóm vai trò (Admin, Doctor, Staff, Patient).
  * Viết và thực thi thành công các script tự động seed dữ liệu mẫu; thực hiện truy vấn kiểm tra cấu trúc DynamoDB items bằng AWS CLI nhằm bảo đảm dữ liệu đầu ra chuẩn hóa cho Frontend.