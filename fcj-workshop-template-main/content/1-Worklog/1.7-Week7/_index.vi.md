---
title: "Worklog Tuần 7"
date: "2025-10-20"
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---


### Mục tiêu tuần 7:

* Thành thạo các dịch vụ AWS storage và container orchestration nâng cao.
* Hoàn thành bản vẽ kiến trúc kỹ thuật cho đề xuất dự án.
* Chuẩn bị toàn diện cho bài đánh giá và kiểm tra tuần 8.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                           | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - **Lab 1: Bảo vệ dữ liệu với AWS Backup** <br>&emsp; + Cấu hình kế hoạch backup <br>&emsp; + Thiết lập backup cross-region <br>&emsp; + Kiểm tra quy trình restore                            | 20/10/2025   | 20/10/2025      | AWS Backup User Guide                    |
| 3   | - **Lab 2: Tự động hóa Snapshot với Amazon EBS Data Lifecycle Manager** <br>&emsp; + Tạo lifecycle policies <br>&emsp; + Cấu hình snapshot tự động <br>&emsp; + Quản lý quy tắc retention      | 21/10/2025   | 21/10/2025      | Amazon EBS Data Lifecycle Manager Guide |
| 4   | - **Lab 3: Quản lý Container với Amazon ECS** <br>&emsp; + Tạo ECS clusters <br>&emsp; + Cấu hình task definitions <br>&emsp; + Deploy ứng dụng container                                       | 22/10/2025   | 22/10/2025      | Amazon ECS Developer Guide              |
| 5   | - **Lab 4: Shared Storage với Amazon EBS Multi-Attach** <br>&emsp; + Cấu hình multi-attach volumes <br>&emsp; + Thiết lập cluster file systems <br>&emsp; + Test truy cập đồng thời           | 23/10/2025   | 23/10/2025      | Amazon EBS Multi-Attach Documentation   |
| 6   | - **Hoàn thành Bản vẽ Kiến trúc Kỹ thuật AWS** <br>&emsp; + Thiết kế kiến trúc hệ thống <br>&emsp; + Tạo network topology <br>&emsp; + Tài liệu tích hợp services                              | 24/10/2025   | 24/10/2025      | AWS Architecture Center                  |
| 7   | - **Xem lại & Học tập cuối tuần** <br>&emsp; + Review tất cả tài liệu các tuần trước <br>&emsp; + Tạo ghi chú học tập tổng hợp <br>&emsp; + Thực hành các scenario hands-on                    | 25/10/2025   | 25/10/2025      | Tài liệu Học tập Cá nhân                |
| CN  | - **Chuẩn bị Đánh giá** <br>&emsp; + Review cuối cùng và làm đề thi thử <br>&emsp; + Củng cố các khoảng trống kiến thức <br>&emsp; + Chuẩn bị cho bài đánh giá tuần 8                         | 26/10/2025   | 26/10/2025      | FCJ Assessment Guidelines               |


### Kết quả đạt được tuần 7:

**Triển khai các Dịch vụ AWS Nâng cao:**

* **Lab AWS Backup:**
  * Cấu hình thành công các kế hoạch backup toàn diện cho EC2 instances và RDS databases
  * Triển khai chiến lược backup cross-region cho disaster recovery
  * Kiểm tra quy trình restore và xác thực tính toàn vẹn backup
  * Học các chính sách retention backup và chiến lược tối ưu hóa chi phí

* **Lab Amazon EBS Data Lifecycle Manager:**
  * Tạo các lifecycle policies tự động cho EBS volumes
  * Cấu hình copy snapshot cross-region để đảm bảo độ bền dữ liệu
  * Triển khai quy tắc retention để quản lý chi phí storage hiệu quả
  * Thiết lập tự động hóa snapshot dựa trên tag để quản lý dữ liệu có tổ chức

* **Lab Amazon ECS Container Orchestration:**
  * Tạo và cấu hình ECS clusters với EC2 và Fargate launch types
  * Phát triển task definitions toàn diện với thông số kỹ thuật tài nguyên
  * Deploy thành công ứng dụng multi-container với load balancing
  * Triển khai service auto-scaling và cấu hình health check

* **Lab Amazon EBS Multi-Attach:**
  * Cấu hình EBS volumes với khả năng multi-attach cho shared storage
  * Thiết lập cluster-aware file systems (OCFS2) cho truy cập đồng thời
  * Kiểm tra các scenario high-availability với nhiều EC2 instances
  * Triển khai cơ chế đảm bảo tính nhất quán dữ liệu và locking

**Phát triển Dự án:**

* **Hoàn thành Bản vẽ Kiến trúc Kỹ thuật AWS:**
  * Thiết kế kiến trúc hệ thống toàn diện cho dự án thực tập
  * Tạo network topology chi tiết với VPC, subnets, và security groups
  * Tài liệu hóa tích hợp services và data flow giữa các components
  * Chuẩn bị thông số kỹ thuật cho giai đoạn implementation

**Chuẩn bị Đánh giá:**

* **Học tập và Xem lại Toàn diện:**
  * Củng cố kiến thức từ tất cả 7 tuần học AWS
  * Tạo ghi chú học tập chi tiết bao phủ tất cả các AWS services chính
  * Thực hành các scenario hands-on và bài tập troubleshooting
  * Xác định và giải quyết các khoảng trống kiến thức thông qua review có mục tiêu

**Kết quả Học tập Chính:**

* Thành thạo các chiến lược quản lý storage nâng cao và bảo vệ dữ liệu
* Có chuyên môn về container orchestration và kiến trúc microservices
* Phát triển kỹ năng lập kế hoạch disaster recovery và business continuity
* Nâng cao hiểu biết về tối ưu hóa chi phí AWS và quản lý tài nguyên
* Cải thiện khả năng tài liệu hóa kỹ thuật và thiết kế kiến trúc

**Kỹ năng Kỹ thuật Đạt được:**
* Triển khai backup và disaster recovery nâng cao
* Deploy và orchestration container
* Tối ưu hóa storage và quản lý lifecycle
* Thiết kế và tài liệu hóa kiến trúc hệ thống
* Sẵn sàng đánh giá và tích hợp kiến thức AWS toàn diện


