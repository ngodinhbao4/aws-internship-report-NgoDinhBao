---
title: "Worklog Tuần 5"
date: 2026-05-21
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---

### Mục tiêu tuần 5:

* Tìm hiểu kiến thức nền tảng về tính năng tự động co giãn hệ thống (AWS Auto Scaling Group) và các cơ chế giám sát tài nguyên (Amazon CloudWatch Alarms).
* Thực hành thiết lập, giả lập tải thực tế để kiểm thử và đánh giá khả năng tự động mở rộng (Scale-out) cũng như thu hẹp (Scale-in) của hạ tầng nhằm tối ưu hóa chi phí và đảm bảo tính sẵn sàng cao (High Availability).

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 6 | - Tìm hiểu tài liệu và cấu hình các chính sách tự động co giãn (Auto Scaling Policies) dựa trên các ngưỡng cảnh báo từ AWS CloudWatch (Ví dụ: CPU Utilization > 70%). | 15/05/2026 | 15/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 2 | - Cài đặt công cụ `stress` trên các EC2 instance; thiết lập kịch bản và tiến hành giả lập tình trạng quá tải CPU để kiểm thử tính năng Scale-out. | 18/05/2026 | 18/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Theo dõi, kiểm tra và đánh giá khả năng tự động khởi chạy instance mới của hệ thống khi gặp tải cao; kiểm tra log hoạt động của ASG. | 19/05/2026 | 19/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Ngắt giả lập tải trên công cụ `stress`; tiến hành theo dõi và xác minh tính năng tự động thu hẹp (Scale-in) để hủy bỏ các thực thể dư thừa. | 20/05/2026 | 20/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - **Thực hành:** <br>Kiểm tra tính chính xác của thời gian chờ hạ nhiệt (Cooldown period); xác nhận hệ thống tự động giảm số lượng instance về mức cấu hình ban đầu (Desired capacity) và tổng hợp số liệu báo cáo. | 21/05/2026 | 21/05/2026 | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 5:

* Nắm vững kiến thức cốt lõi và làm chủ quy trình cấu hình tính năng tự động co giãn động trên AWS:
  * Hoàn thành cấu hình các ngưỡng cảnh báo điều kiện trên Amazon CloudWatch và liên kết thành công với Auto Scaling Group (ASG).
  * Hiểu sâu sắc cơ chế hoạt động của các thông số cấu hình cốt lõi: Min capacity, Max capacity và Desired capacity.

* Khả năng giả lập tải thực tế và kiểm thử tính năng tự động mở rộng (Scale-out):
  * Sử dụng thành thạo công cụ `stress` trên EC2 để đẩy CPU Utilization lên ngưỡng kích hoạt cảnh báo theo đúng kịch bản thiết lập.
  * Hệ thống tự động nhận diện chính xác tín hiệu từ CloudWatch và thực hiện Scale-out (thêm EC2 instance mới) thành công, đảm bảo hiệu năng hệ thống không bị gián đoạn.

* Xác minh và tối ưu hóa chi phí thông qua tính năng tự động thu hẹp (Scale-in):
  * Xác minh thành công khả năng nhận biết giảm tải của ASG sau khi ngắt công cụ giả lập, hệ thống kích hoạt chính xác thời gian chờ hạ nhiệt (Cooldown period).
  * Tính năng Scale-in hoạt động chuẩn xác, các EC2 instance dư thừa được hủy bỏ một cách an toàn để đưa hệ thống về trạng thái mong muốn ban đầu, giúp tối ưu hóa chi phí tài nguyên.

* Quản lý tài liệu và đánh giá hiệu năng hệ thống:
  * Tổng hợp thành công các số liệu kiểm thử thực tế, đánh giá toàn diện hiệu năng co giãn và hoàn thiện tài liệu hướng dẫn vận hành hệ thống có tính sẵn sàng cao (High Availability).
  * Hoàn thành đúng hạn báo cáo tiến độ tuần 5 của khóa học AWS FCAJ.