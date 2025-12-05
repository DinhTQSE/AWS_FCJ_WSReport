---
title: "Worklog Tuần 6"
date: "2025-10-13"
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---


### Mục tiêu tuần 6:

* Học các dịch vụ AWS Security nâng cao cho ứng dụng doanh nghiệp.
* Thực hiện các chiến lược quản lý thông tin đăng nhập và bảo vệ ứng dụng.
* Hoàn thành và finalize tài liệu đề xuất thực tập.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                       | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - **Lab 1: Quản lý thông tin đăng nhập với AWS Secrets Manager** <br>&emsp; + Tạo kho lưu trữ bí mật <br>&emsp; + Cấu hình tự động xoay mật khẩu <br>&emsp; + Tích hợp với ứng dụng          | 13/10/2025   | 13/10/2025      | AWS Secrets Manager Documentation         |
| 3   | - **Lab 2: Bảo vệ ứng dụng với AWS WAF** <br>&emsp; + Cấu hình web ACLs <br>&emsp; + Thiết lập giới hạn tốc độ <br>&emsp; + Chặn các yêu cầu độc hại                                         | 14/10/2025   | 14/10/2025      | AWS WAF User Guide                       |
| 4   | - **Lab 3: Phát hiện mối đe dọa với AWS GuardDuty** <br>&emsp; + Kích hoạt phát hiện mối đe dọa <br>&emsp; + Cấu hình kết quả tìm kiếm <br>&emsp; + Thiết lập thông báo                        | 15/10/2025   | 15/10/2025      | AWS GuardDuty Documentation              |
| 5   | - **Lab 4: Tuân thủ bảo mật với AWS Security Hub** <br>&emsp; + Kích hoạt tiêu chuẩn bảo mật <br>&emsp; + Xem xét kết quả tuân thủ <br>&emsp; + Tạo báo cáo                                    | 16/10/2025   | 16/10/2025      | AWS Security Hub User Guide             |
| 6   | - **Hoàn thành Đề xuất Thực tập** <br>&emsp; + Hoàn thiện mục tiêu dự án <br>&emsp; + Xác định các sản phẩm bàn giao <br>&emsp; + Đặt timeline và mốc quan trọng                              | 17/10/2025   | 17/10/2025      | FCJ Proposal Template                    |
| 7   | - **Xem lại & Tài liệu cuối tuần** <br>&emsp; + Xem lại tất cả triển khai lab bảo mật <br>&emsp; + Ghi chú bài học kinh nghiệm <br>&emsp; + Chuẩn bị tài liệu thuyết trình                     | 18/10/2025   | 18/10/2025      | Tài liệu Cá nhân                        |
| CN  | - **Tổng kết tuần & Lập kế hoạch** <br>&emsp; + Viết worklog tổng hợp chi tiết <br>&emsp; + Phân tích kết quả bảo mật <br>&emsp; + Lập kế hoạch hoạt động tuần tới                            | 19/10/2025   | 19/10/2025      | FCJ Worklog Template                    |


### Kết quả đạt được tuần 6:

**Triển khai các Dịch vụ AWS Security:**

* **Lab AWS Secrets Manager:**
  * Tạo và cấu hình thành công kho lưu trữ thông tin đăng nhập an toàn
  * Triển khai tự động xoay mật khẩu cho cơ sở dữ liệu RDS
  * Tích hợp việc lấy thông tin bí mật với các hàm Lambda
  * Học các phương pháp hay nhất để quản lý API keys và thông tin đăng nhập database

* **Lab AWS WAF (Web Application Firewall):**
  * Cấu hình danh sách Access Control Lists (ACLs) cho bảo vệ ứng dụng
  * Triển khai các quy tắc giới hạn tốc độ để ngăn chặn tấn công DDoS
  * Thiết lập chặn theo vị trí địa lý và lọc danh tiếng IP
  * Chặn thành công các mẫu tấn công SQL injection và XSS

* **Lab AWS GuardDuty:**
  * Kích hoạt phát hiện mối đe dọa thông minh trên toàn bộ tài khoản AWS
  * Cấu hình nguồn cung cấp thông tin mối đe dọa và phát hiện malware
  * Thiết lập tích hợp CloudWatch Events để phản hồi tự động
  * Phân tích các kết quả bảo mật và chỉ số mối đe dọa

* **Lab AWS Security Hub:**
  * Kích hoạt AWS Config và giám sát tuân thủ AWS Security Hub
  * Xem xét các kết quả CIS AWS Foundations Benchmark
  * Tạo báo cáo tổng thể về tình trạng bảo mật
  * Triển khai các chiến lược khắc phục cho các vấn đề quan trọng

**Quản lý Dự án:**

* **Hoàn thành Đề xuất Thực tập:**
  * Xác định rõ ràng mục tiêu và phạm vi dự án
  * Thiết lập các sản phẩm bàn giao và tiêu chí thành công
  * Tạo timeline chi tiết với các mốc quan trọng hàng tuần
  * Xác định tài nguyên cần thiết và thách thức tiềm ẩn

**Kết quả Học tập Chính:**

* Hiểu sâu về kiến trúc bảo mật AWS
* Học cách triển khai chiến lược bảo mật nhiều lớp
* Phát triển kỹ năng phát hiện mối đe dọa và ứng phó sự cố
* Thành thạo các kỹ thuật giám sát và báo cáo tuân thủ
* Nâng cao khả năng lập kế hoạch và documentation dự án

**Kỹ năng Kỹ thuật Đạt được:**
* Cấu hình và quản lý chính sách bảo mật
* Triển khai phản hồi mối đe dọa tự động
* Hiểu biết về framework tuân thủ
* Chiến lược đánh giá và giảm thiểu rủi ro

**Hoạt động Cuối tuần & Xem lại:**

* **Thứ 7 - Tài liệu & Phân tích:**
  * Xem lại và phân tích tất cả các triển khai lab bảo mật
  * Ghi chú chi tiết các bước và cấu hình để tham khảo sau này
  * Tạo bảng so sánh giữa các dịch vụ bảo mật khác nhau
  * Xác định cơ hội tích hợp tiềm năng giữa các dịch vụ

* **Chủ nhật - Tổng kết & Lập kế hoạch:**
  * Viết worklog tuần toàn diện với chi tiết kỹ thuật
  * Phân tích kết quả bảo mật và tạo khuyến nghị cải tiến
  * Chuẩn bị tài liệu thuyết trình cho buổi review tiến độ tuần tới
  * Lập kế hoạch chiến lược tích hợp cho các chủ đề AWS nâng cao sắp tới


