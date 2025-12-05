---
title: "Worklog Tuần 11"
date: "2025-11-17"
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---



### Mục tiêu tuần 11:

* Triển khai Infrastructure as Code với Terraform.
* Thiết lập CI/CD pipeline tự động hóa.
* Áp dụng best practices bảo mật (WAF, giám sát).
* Tham gia các workshop AWS Cloud Mastery Series.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- |
| 2   | - Viết code Terraform cho toàn bộ tài nguyên: Lambda, API Gateway, DynamoDB, IoT Core <br> - Test triển khai hạ tầng qua Terraform                                                         | 17/11/2025   | 18/11/2025      |

| Thứ | Sự kiện/Công việc | Ngày | Hình thức | Nội dung & Kết quả Đạt được |
| --- | ----------------- | ---- | --------- | --------------------------- |
| 2   | **AWS Cloud Mastery Series #2**<br/>*DevOps & Container Orchestration* | 17/11/2025 | Offline | **Chủ đề chính:**<br/>• Containerization: So sánh Docker vs VM, tối ưu hóa Dockerfile<br/>• Orchestration: Kiến trúc Amazon ECS (Fargate vs EC2) so với Kubernetes<br/>• CI/CD: Sử dụng CloudFormation và CodePipeline cho triển khai tự động<br/><br/>**Kết quả học tập:**<br/>✓ Thành thạo các khái niệm containerization và best practices Docker<br/>✓ Hiểu rõ orchestration ECS và chiến lược deployment<br/>✓ Triển khai CI/CD pipelines tự động hóa |
| 4   | **Workshop: Secure Your Applications**<br/>*AWS Perimeter Protection (Edge Security)*<br/><br/>**Giảng viên:**<br/>• Mr. Nguyen Gia Hung (Head of SA VN)<br/>• Mr. Julian Ju (Regional Edge Specialist)<br/>• Mr. Kevin Lim (Regional Edge Specialist) | 19/11/2025 | Offline | **Chủ đề chính:**<br/>• Hands-on Lab: Cấu hình AWS WAF chống SQL Injection/XSS<br/>• Resilience: Triển khai AWS Shield để giảm thiểu tấn công DDoS<br/>• Best practices và patterns cho edge security<br/><br/>**Kết quả học tập:**<br/>✓ Cấu hình AWS WAF rules để bảo vệ web application<br/>✓ Triển khai AWS Shield cho phòng chống DDoS<br/>✓ Hiểu thiết kế kiến trúc perimeter security |

| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- |
| 6   | - Thiết lập AWS CodePipeline kết nối GitHub <br> - Cấu hình auto-deploy khi push code Terraform <br> - Setup AWS Amplify cho Frontend CI/CD                                                | 21/11/2025   | 21/11/2025      |

| Thứ | Sự kiện/Công việc | Ngày | Hình thức | Nội dung & Kết quả |
| --- | ----------------- | ---- | --------- | ------------------ |
| 7   | **Họp Nhóm #4**<br/>*Review IaC & Pipeline* | 22/11/2025 | Offline | **Trọng tâm:**<br/>• Review chất lượng code Terraform<br/>• Test trigger CI/CD pipeline<br/>• Checklist audit bảo mật<br/><br/>**Kết quả:**<br/>✓ IaC deploy thành công toàn bộ tài nguyên<br/>✓ Pipeline tự động deploy khi push code |

| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- |
| CN   | - Bật AWS WAF trên API Gateway/CloudFront <br> - Cấu hình CloudWatch Dashboard giám sát <br> - Thiết lập alarm cho lỗi hệ thống <br> - Viết worklog và review tiến độ tuần                                                            | 23/11/2025   | 23/11/2025      |


### Kết quả đạt được tuần 11:

#### 🏗️ Infrastructure as Code
* **Triển khai Terraform:**
  * Toàn bộ tài nguyên AWS được định nghĩa bằng code
  * Hạ tầng version-controlled
  * Deployments có thể lặp lại

#### 🔄 Tự động hóa CI/CD
* **Pipeline đã thiết lập:**
  * Tự động deploy khi push GitHub
  * Frontend qua AWS Amplify
  * Backend qua CodePipeline

#### 🔒 Bảo mật & Giám sát
* **AWS WAF**: Bảo vệ API khỏi các tấn công phổ biến.
* **CloudWatch**: Dashboard giám sát real-time.

#### 🤖 Workshop AWS Đã Tham Gia
* **Generative AI với Amazon Bedrock:**
  * Kiến trúc RAG cho AI doanh nghiệp
  * AI Agents với Runtime & Memory
  * Tối ưu hóa few-shot prompting

* **DevOps & Container Orchestration:**
  * Docker vs VM, tối ưu Dockerfile
  * Orchestration Amazon ECS & Kubernetes
  * CI/CD với CloudFormation & CodePipeline

* **Workshop Bảo mật - AWS Perimeter Protection:**
  * AWS WAF: Chống SQL Injection/XSS
  * AWS Shield: Giảm thiểu DDoS
  * Best practices kiến trúc edge security


