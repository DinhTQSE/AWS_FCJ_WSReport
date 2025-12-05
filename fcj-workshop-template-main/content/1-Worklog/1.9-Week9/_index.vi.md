---
title: "Worklog Tuần 9"
date: "2025-11-03"
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---


### Mục tiêu tuần 9:

* Triển khai Hybrid Authentication (Vân tay + Cloud).
* Xây dựng API cho truy xuất dữ liệu (Dashboard & Tìm kiếm).
* Hoàn thiện tầng business logic.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- |
| 2   | - Tạo bảng DynamoDB DeviceOfficerMap_Pool <br> - Viết Lambda AuthorizeFunction cho xác thực vân tay                                                                                         | 03/11/2025   | 03/11/2025      |
| 3   | - Cấu hình IoT Rule cho luồng authorization <br> - Cập nhật firmware ESP32: Quét vân tay → Gửi SlotID → Nhận lệnh unlock                                                                   | 04/11/2025   | 04/11/2025      |
| 5   | - Tạo 2 GSI trên ViolationsDB (Dashboard & Search indexes) <br> - Viết Lambda GetDashboardFunction và SearchByCCCDFunction                                                                  | 06/11/2025   | 07/11/2025      |

| Thứ | Sự kiện/Công việc | Ngày | Hình thức | Nội dung & Kết quả |
| --- | ----------------- | ---- | --------- | ------------------ |
| 7   | **Họp Nhóm #2**<br/>*API Integration Testing* | 08/11/2025 | Offline | **Trọng tâm:**<br/>• Test xác thực vân tay end-to-end<br/>• Debug Lambda functions API<br/>• Validate hiệu suất query GSI<br/><br/>**Kết quả:**<br/>✓ Xác thực vân tay hoạt động đúng<br/>✓ APIs trả về JSON data đúng format |

| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- |
| CN   | - Thiết lập API Gateway: Tạo endpoints /dashboard và /search/{cccd} <br> - Bật cấu hình CORS <br> - Integration test: Browser → API → JSON response <br> - Viết worklog và review tiến độ tuần | 09/11/2025   | 09/11/2025      |


### Kết quả đạt được tuần 9:

* **Authentication**: Quét vân tay → Thiết bị unlock thành công.
* **API Layer**: Endpoints Dashboard và Search hoạt động.
* **Database**: GSI indexes tối ưu cho query patterns.
* **Deliverable**: Gọi API từ browser trả về dữ liệu vi phạm dạng JSON.
  * ...

* Có khả năng kết nối giữa giao diện web và CLI để quản lý tài nguyên AWS song song.
* ...


