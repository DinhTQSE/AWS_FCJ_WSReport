---
title: "Event 3"
date: "2025-11-19"
weight: 3
chapter: false
pre: " <b> 4.3. </b> "
---

# Báo Cáo Tổng Kết: "Workshop: Secure Your Applications - AWS Perimeter Protection"

### Thông Tin Sự Kiện

- **Ngày**: Thứ Ba, 19 tháng 11, 2025
- **Thời gian**: Workshop cả ngày
- **Địa điểm**: AWS Training Center, Thành phố Hồ Chí Minh
- **Đơn vị tổ chức**: AWS Vietnam
- **Loại hình**: Workshop Kỹ thuật Thực hành

### Giảng Viên

- **Mr. Nguyen Gia Hung** – Head of Solutions Architects, AWS Vietnam
- **Mr. Julian Ju** – Regional Edge Security Specialist, AWS APAC
- **Mr. Kevin Lim** – Regional Edge Security Specialist, AWS APAC

### Mục Tiêu Sự Kiện

- Hiểu về các dịch vụ edge security của AWS và chiến lược perimeter protection
- Học cách bảo vệ ứng dụng web khỏi các cuộc tấn công phổ biến (SQL Injection, XSS, DDoS)
- Thành thạo cấu hình AWS WAF (Web Application Firewall) và quản lý rules
- Triển khai AWS Shield cho bảo vệ DDoS và resilience
- Có kinh nghiệm thực hành với các kịch bản security thực tế
- Thiết kế kiến trúc ứng dụng bảo mật sử dụng AWS edge services

### Cấu Trúc Workshop

#### Phiên 1: Giới Thiệu AWS Edge Security (Buổi Sáng)

**Chủ đề:**
- Tổng quan về hệ sinh thái AWS edge security services
- Hiểu shared responsibility model cho application security
- Các lỗ hổng web application phổ biến (OWASP Top 10)
- Patterns kiến trúc AWS edge security

**Khái Niệm Chính:**
- **Edge Security**: Bảo vệ ứng dụng tại network perimeter trước khi threats đến backend infrastructure
- **Defense in Depth**: Phương pháp security multi-layered
- **CloudFront Integration**: Content delivery với security features tích hợp

#### Phiên 2: AWS WAF Deep Dive (Cuối Buổi Sáng)

**AWS WAF Fundamentals:**
- Kiến trúc và components của Web Application Firewall
- Rule groups và rule priority
- WAF managed rules vs custom rules
- Integration với CloudFront, Application Load Balancer, và API Gateway

**Cơ Chế Bảo Vệ Threats:**
1. **SQL Injection Prevention**
   - Pattern matching cho SQL syntax
   - Request body inspection
   - Query string analysis

2. **Cross-Site Scripting (XSS) Protection**
   - Script tag detection
   - JavaScript injection prevention
   - HTML entity encoding

3. **Rate Limiting**
   - Request throttling per IP
   - Bot detection và mitigation
   - Geographic restrictions

#### Phiên 3: Hands-on Lab - Cấu Hình AWS WAF (Buổi Chiều)

**Mục Tiêu Lab:**
Người tham gia cấu hình AWS WAF để bảo vệ sample web application khỏi nhiều loại tấn công.

**Hoạt Động Lab:**

**Phần 1: Thiết Lập Ban Đầu**
- Tạo CloudFront distribution với origin web server
- Deploy sample vulnerable web application để testing
- Thiết lập CloudWatch logging cho security monitoring

**Phần 2: Bảo Vệ SQL Injection**
```
Các bước thực hiện:
1. Tạo WAF Web ACL (Access Control List)
2. Thêm SQL Injection match condition
3. Cấu hình rule để block các SQL patterns đáng ngờ
4. Test với simulated SQL injection attacks
5. Verify blocking behavior trong CloudWatch logs
```

**Cấu Hình Chính:**
- Rule Priority: High
- Action: Block
- Scope: Request body và query strings
- Patterns: Các SQL keywords phổ biến (SELECT, UNION, DROP, v.v.)

**Phần 3: Triển Khai XSS Protection**
```
Các bước thực hiện:
1. Thêm XSS match condition vào Web ACL
2. Cấu hình script tag detection rules
3. Thiết lập JavaScript pattern matching
4. Test với XSS payloads
5. Phân tích blocked requests
```

**Phần 4: Rate Limiting Rules**
```
Các bước thực hiện:
1. Tạo rate-based rule (1000 requests per 5 phút)
2. Cấu hình IP-based throttling
3. Simulate high-volume requests
4. Quan sát automatic blocking behavior
```

#### Phiên 4: AWS Shield cho DDoS Protection (Cuối Buổi Chiều)

**AWS Shield Overview:**
- **Shield Standard**: Automatic protection miễn phí
- **Shield Advanced**: Enhanced DDoS protection với 24/7 support

**Các Loại DDoS Attack:**
1. **Network Layer Attacks (Layer 3/4)**
   - SYN floods
   - UDP reflection attacks
   - TCP connection exhaustion

2. **Application Layer Attacks (Layer 7)**
   - HTTP floods
   - Slowloris attacks
   - Application-specific exploits

**Triển Khai Shield:**
- Bật AWS Shield Advanced cho critical resources
- Cấu hình DDoS Response Team (DRT) access
- Thiết lập CloudWatch alarms cho attack detection
- Review cost protection policies

**Hoạt Động Thực Hành:**
- Phân tích historical DDoS attack patterns
- Cấu hình automatic attack mitigation
- Thiết lập real-time attack notifications
- Review DDoS attack reports và metrics

### Technical Deep Dives

#### AWS WAF Rule Design Best Practices

**1. Chiến Lược Bảo Vệ Nhiều Tầng**
```
Tầng 1: Managed Rule Groups (AWS Managed Rules)
  - Core Rule Set (CRS)
  - Known Bad Inputs
  - Admin Protection

Tầng 2: Rate-based Rules
  - Geographic rate limiting
  - IP reputation lists
  - Custom rate thresholds

Tầng 3: Custom Business Logic Rules
  - Application-specific patterns
  - Authentication bypass prevention
  - Sensitive data exposure protection
```

**2. Thứ Tự Đánh Giá Rule**
- Count rules cho monitoring (không block)
- Allow rules cho trusted sources
- Block rules cho known threats
- Rate-based rules cho volume control
- Default action (thường là Allow)

#### Kiến Trúc Tích Hợp

**CloudFront + WAF + Shield Architecture:**
```
Internet
    ↓
AWS Shield (DDoS Protection)
    ↓
Amazon CloudFront (Edge Locations)
    ↓
AWS WAF (Application Layer Filtering)
    ↓
Application Load Balancer
    ↓
Backend Application (EC2/ECS/Lambda)
```

**Lợi Ích Edge Protection:**
- Threats bị chặn trước khi đến infrastructure
- Giảm backend load và costs
- Cải thiện application performance
- Chia sẻ global threat intelligence

### Monitoring và Incident Response

**CloudWatch Integration:**
- Real-time metrics dashboards
- Blocked request patterns
- Geographic attack sources
- False positive identification

**Logging Strategy:**
- Full request/response logging
- Centralized log aggregation
- Automated threat analysis
- Compliance audit trails

**Quy Trình Incident Response:**
1. Alert triggered bởi CloudWatch alarm
2. Security team review blocked requests
3. Phân tích attack patterns và sources
4. Điều chỉnh WAF rules nếu cần
5. Document incident cho tham khảo sau

### Kịch Bản Thực Tế Thảo Luận

#### Case Study 1: Bảo Vệ E-commerce Platform
**Thách thức**: Nhà bán lẻ online gặp credential stuffing attacks
**Giải pháp**: 
- Triển khai rate-based rules per user session
- Thêm CAPTCHA challenges cho suspicious IPs
- Cấu hình custom rules cho login endpoints
**Kết quả**: Giảm 95% fraudulent login attempts

#### Case Study 2: API Gateway Security
**Thách thức**: RESTful API dễ bị injection attacks
**Giải pháp**:
- Deploy WAF trên API Gateway
- Tạo custom rules cho API-specific threats
- Triển khai request size limits
**Kết quả**: Zero successful injection attacks sau deployment

#### Case Study 3: DDoS Attack Mitigation
**Thách thức**: Media website bị tấn công DDoS 300 Gbps
**Giải pháp**:
- AWS Shield Advanced automatic mitigation
- CloudFront geographic restrictions
- Emergency runbook activation
**Kết quả**: Application vẫn available với < 1% performance impact

### Bài Học Chính

#### Kỹ Năng Kỹ Thuật Thu Được

**AWS WAF Expertise:**
- ✅ Cấu hình Web ACLs với nhiều rule types
- ✅ Triển khai SQL Injection và XSS protection
- ✅ Thiết lập rate-based rules cho bot mitigation
- ✅ Tích hợp WAF với CloudFront và ALB
- ✅ Phân tích security logs và metrics

**DDoS Protection Knowledge:**
- ✅ Hiểu các DDoS attack vectors khác nhau
- ✅ Triển khai AWS Shield protection layers
- ✅ Cấu hình automatic attack response
- ✅ Thiết lập monitoring và alerting systems

**Security Architecture:**
- ✅ Thiết kế defense-in-depth strategies
- ✅ Áp dụng edge security best practices
- ✅ Triển khai zero-trust principles
- ✅ Tối ưu cost vs security trade-offs

#### Best Practices Học Được

**1. Security by Design**
- Triển khai security controls từ ngày đầu
- Regular security testing và updates
- Continuous monitoring và improvement

**2. Automation First**
- Tự động hóa threat detection và response
- Sử dụng managed rules khi có thể
- Triển khai Infrastructure as Code cho consistency

**3. Cost Optimization**
- Bắt đầu với Shield Standard (free tier)
- Dùng managed rules trước custom rules
- Monitor và optimize rule efficiency

**4. Compliance và Governance**
- Document tất cả security configurations
- Regular audit và compliance reviews
- Incident response playbooks

### Ứng Dụng Thực Tiễn

**Kế Hoạch Triển Khai Ngay:**
1. **Tuần 1**: Deploy AWS WAF trên development environment
2. **Tuần 2**: Cấu hình core rule sets và test kỹ lưỡng
3. **Tuần 3**: Enable production deployment với monitoring
4. **Tuần 4**: Review metrics và optimize rules

**Kỹ Năng Cần Thực Hành:**
- Regular WAF rule testing và updates
- Security log analysis và pattern recognition
- Incident response procedures
- Cost monitoring và optimization

### Suy Nghĩ Cá Nhân

Workshop này cực kỳ có giá trị, cung cấp kiến thức kỹ thuật sâu về AWS edge security services. Các hands-on labs với real attack scenarios làm cho việc học trở nên highly practical và engaging.

**Khía Cạnh Có Giá Trị Nhất:**
- **Expert Instruction**: Học từ AWS regional specialists (Julian Ju và Kevin Lim) cung cấp insights không có trong documentation
- **Hands-on Practice**: Cấu hình WAF rules và testing với real attacks củng cố kiến thức lý thuyết
- **Real-world Cases**: Case studies demonstrate practical application trong production environments
- **Architecture Patterns**: Hiểu cách integrate multiple security services effectively

**Thách Thức Gặp Phải:**
- Rule priority và evaluation order ban đầu confusing
- Cân bằng security strictness với false positive prevention
- Hiểu cost implications của different configurations

**Key Learnings:**
- Edge security critical cho modern cloud applications
- AWS provides powerful tools, nhưng proper configuration essential
- Security là ongoing process, không phải one-time setup
- Integration của multiple services (WAF + Shield + CloudFront) cung cấp comprehensive protection

**Ứng Dụng Tương Lai:**
Kiến thức này directly applicable cho:
- Securing microservices architectures
- Protecting API endpoints
- Implementing compliance requirements (PCI-DSS, SOC 2)
- Designing resilient, security-first cloud applications

### Tài Nguyên và Tham Khảo

**AWS Documentation:**
- AWS WAF Developer Guide
- AWS Shield Advanced Best Practices
- CloudFront Security Documentation
- Well-Architected Framework - Security Pillar

**Tools và Services Sử Dụng:**
- AWS WAF (Web Application Firewall)
- AWS Shield (Standard và Advanced)
- Amazon CloudFront
- Application Load Balancer
- AWS CloudWatch
- AWS Config cho compliance

**Additional Learning Resources:**
- AWS Security Hub cho centralized security management
- AWS Firewall Manager cho multi-account governance
- OWASP Top 10 vulnerability guides
- AWS Security Blog cho latest threats và solutions

---

> **Tóm tắt**: Workshop này cung cấp comprehensive, hands-on training về AWS edge security services, đặc biệt là AWS WAF và AWS Shield. Sự kết hợp của expert instruction từ AWS specialists, practical labs với real attack scenarios, và real-world case studies khiến đây trở thành invaluable learning experience. Các kỹ năng thu được immediately applicable cho việc securing production cloud applications và designing resilient, security-first architectures.
