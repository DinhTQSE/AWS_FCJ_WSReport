---
title: "Worklog Tuần 12"
date: "2025-11-24"
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---
### Mục tiêu tuần 12:

* Hoàn thiện testing, tuning và tối ưu hóa.
* Chuẩn bị tài liệu toàn diện.
* Quay video demo và hoàn tất các deliverable.
* Tham gia workshop AWS Cloud Mastery Series.

### Các công việc cần triển khai trong tuần này:


| Thứ | Công việc                                                                                                                                                       | Ngày bắt đầu | Ngày hoàn thành |
| ------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------ | -------------------- |
| 2    | - Stress test: Chạy thử nghiệm ổn định toàn hệ thống<br> - Hiệu chỉnh cảm biến nếu sai số quá lớn <br> - Cải thiện UI/UX web (tinh chỉnh CSS) | 24/11/2025       | 26/11/2025         |
| 5    | - Viết tài liệu Final Report<br> - Cập nhật sơ đồ kiến trúc phiên bản mới nhất <br> - Chuẩn bị tài liệu kỹ thuật                              | 27/11/2025       | 27/11/2025         |


| Thứ | Sự kiện/Công việc                                                             | Ngày      | Hình thức | Nội dung & Kết quả Đạt được                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| ------ | ----------------------------------------------------------------------------------- | ------------ | ------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 7    | **AWS Cloud Mastery Series #3**<br/>*Advanced Security & Networking Architecture* | 29/11/2025 | Offline     | **Chủ đề chính:**<br/><br/>**Quản lý Danh tính & Truy cập:**<br/>• Quản lý quyền hạn quy mô lớn với Service Control Policies (SCPs)<br/>• Triển khai Short-term credentials sử dụng AWS STS (Security Token Service)<br/>• Best practices cho least-privilege access ở cấp độ tổ chức<br/><br/>**Kiến trúc Phòng thủ Mạng:**<br/>• Nguyên tắc thiết kế kiến trúc Defense-in-Depth<br/>• Kiểm soát traffic East-West bằng AWS Network Firewall<br/>• Kiểm tra traffic nội bộ và ngăn chặn mối đe dọa<br/><br/>**Chiến lược Microsegmentation:**<br/>• Kỹ thuật Security Group Referencing cho kiểm soát truy cập chi tiết<br/>• Tích hợp Transit Gateway cho bảo mật multi-VPC<br/>• Triển khai kiến trúc mạng zero-trust<br/><br/>**Kết quả học tập:**<br/>✓ Thành thạo quản trị danh tính quy mô doanh nghiệp với SCPs<br/>✓ Triển khai access patterns bảo mật tạm thời với STS<br/>✓ Thiết kế kiến trúc mạng defense-in-depth<br/>✓ Áp dụng Network Firewall cho kiểm tra traffic nội bộ<br/>✓ Cấu hình microsegmentation bằng Security Group Referencing<br/>✓ Tích hợp Transit Gateway cho kết nối multi-VPC bảo mật |
| 7    | **Họp Nhóm #5**<br/>*Review Cuối & Tổng duyệt*                               | 29/11/2025 | Offline     | **Trọng tâm:**<br/>• Review checklist toàn bộ deliverable<br/>• Tổng duyệt bài thuyết trình demo<br/>• Sửa lỗi cuối và đánh bóng<br/><br/>**Kết quả:**<br/>✓ Tất cả component hoạt động ổn định<br/>✓ Tài liệu hoàn chỉnh<br/>✓ Sẵn sàng nộp bài                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |


| Thứ | Công việc                                                                                                                                                                         | Ngày bắt đầu | Ngày hoàn thành |
| ------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------ | -------------------- |
| CN   | - Quay video demo sản phẩm<br> - Đóng gói toàn bộ source code nộp bài <br> - Nộp cuối cùng: Source code, Report, Video <br> - Viết worklog và review tiến độ tuần | 30/11/2025       | 30/11/2025         |

### Kết quả đạt được tuần 12:

#### ✅ Testing & Đảm bảo Chất lượng

* **Stress Testing**: Hệ thống ổn định dưới tải.
* **Hiệu chỉnh Cảm biến**: Độ chính xác trong phạm vi chấp nhận.
* **Đánh bóng UI**: Giao diện web chuyên nghiệp.

#### 📄 Tài liệu Hoàn chỉnh

* **Final Report**: Tài liệu dự án toàn diện.
* **Sơ đồ Kiến trúc**: Cập nhật v7 với đầy đủ component.
* **API Documentation**: Tài liệu tham chiếu endpoint đầy đủ.

#### 🎥 Deliverable Sẵn sàng

* **Video Demo**: Trình diễn workflow hoàn chỉnh.
* **Source Code**: Sạch, có documentation, version-controlled.
* **Deployment**: Hệ thống production live và hoạt động.

#### 🎓 Workshop Đã Tham Gia

* **Bảo mật & Networking Nâng cao:**
  * Enterprise IAM: SCPs quản lý quyền multi-account
  * AWS STS: Temporary credentials & cross-account access
  * Least Privilege: IAM policies zero-trust quy mô lớn
  * Defense-in-Depth: Kiến trúc bảo mật mạng đa tầng
  * AWS Network Firewall: Kiểm tra traffic East-West & ngăn chặn mối đe dọa
  * Microsegmentation: Security Group Referencing & Transit Gateway integration
  * **Bảo vệ Mối đe dọa Tiên tiến:**

    * Chặn traffic độc hại giữa các resources nội bộ
    * Áp dụng deep packet inspection để ngăn chặn lateral movement
    * Cấu hình custom rule sets cho mối đe dọa cụ thể tổ chức
    * Tích hợp với AWS Firewall Manager cho centralized policies

#### 🌐 Microsegmentation & Zero-Trust Networking

* **Security Group Referencing:**

  * Triển khai microsegmentation sử dụng Security Group references
  * Tạo security rules tự động cập nhật, dynamic
  * Giảm overhead quản lý với logical security boundaries
  * Áp dụng kiểm soát truy cập chi tiết giữa các application tiers
* **Tích hợp Transit Gateway:**

  * Thiết kế kiến trúc kết nối multi-VPC có khả năng mở rộng
  * Tập trung hoá network routing và security inspection
  * Triển khai network topology hub-and-spoke
  * Áp dụng Transit Gateway security best practices
* **Kiến trúc Mạng Zero-Trust:**

  * Loại bỏ implicit trust giữa các network segments
  * Xác thực mọi kết nối bất kể nguồn gốc
  * Triển khai identity-based access controls ở tầng network
  * Áp dụng nguyên tắc xác thực liên tục và least-privilege

#### 🎯 Năng lực Bảo mật Tiên tiến

* **Bảo mật Quy mô Doanh nghiệp:** Thành thạo các patterns bảo mật áp dụng cho môi trường AWS phức tạp, quy mô lớn
* **Thiết kế Kiến trúc:** Đạt chuyên môn trong thiết kế kiến trúc cloud bảo mật, có khả năng mở rộng
* **Best Practices:** Áp dụng các nguyên tắc AWS Well-Architected Framework security pillar
* **Compliance:** Hiểu các kiểm soát bảo mật cần thiết cho các ngành có quy định nghiêm ngặt
