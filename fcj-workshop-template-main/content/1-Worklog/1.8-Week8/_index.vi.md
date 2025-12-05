---
title: "Worklog Tuần 8"
date: "2025-10-27"
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---


### Mục tiêu tuần 8:

* Xây dựng Core Pipeline: Dữ liệu cảm biến truyền đến Database.
* Hoàn thiện lắp ráp phần cứng và test tất cả cảm biến.
* Thiết lập kết nối AWS IoT Core.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- |
| 2   | - Lắp ráp mạch trên Breadboard: ESP32 + MQ-3 + MAX30102 + Keypad + LCD + AS608 <br> - Unit test từng cảm biến riêng lẻ                                                                     | 27/10/2025   | 28/10/2025      |
| 4   | - Viết firmware ESP32: Đọc dữ liệu MQ-3 (nồng độ cồn) và MAX30102 (nhịp tim) <br> - Triển khai input Keypad và hiển thị LCD                                                                | 29/10/2025   | 30/10/2025      |
| 6   | - Đóng gói dữ liệu cảm biến dạng JSON <br> - Triển khai MQTT publish tới AWS IoT Core                                                                                                       | 31/10/2025   | 31/10/2025      |

| Thứ | Sự kiện/Công việc | Ngày | Hình thức | Nội dung & Kết quả |
| --- | ----------------- | ---- | --------- | ------------------ |
| 7   | **Họp Nhóm #1**<br/>*Hardware & Firmware Sprint* | 01/11/2025 | Offline | **Trọng tâm:**<br/>• Debug vấn đề tích hợp cảm biến<br/>• Test kết nối MQTT tới AWS IoT Core<br/>• Review chất lượng code firmware<br/><br/>**Kết quả:**<br/>✓ Tất cả cảm biến hoạt động ổn định<br/>✓ MQTT publish dữ liệu thành công |

| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- |
| CN   | - Thiết lập AWS IoT Core: Tạo Thing, Policy, Certificate <br> - Cấu hình IoT Rule cho routing dữ liệu <br> - Viết Lambda ProcessViolationFunction <br> - Tạo bảng DynamoDB ViolationsDB <br> - Test end-to-end: Cảm biến → DynamoDB <br> - Viết worklog và review tiến độ tuần | 02/11/2025   | 02/11/2025      |


### Kết quả đạt được tuần 8:

* **Phần cứng**: Tất cả cảm biến hoạt động trên breadboard.
* **Firmware**: ESP32 đọc cảm biến và publish MQTT thành công.
* **AWS**: IoT Core đã cấu hình, Lambda xử lý dữ liệu, DynamoDB lưu trữ vi phạm.
* **Deliverable**: Thổi vào cảm biến MQ-3 → Bản ghi mới xuất hiện trong DynamoDB.
  * ...

* Có khả năng kết nối giữa giao diện web và CLI để quản lý tài nguyên AWS song song.
* ...


