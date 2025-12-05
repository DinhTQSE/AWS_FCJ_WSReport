---
title: "Event 3"
date: "2025-11-19"
weight: 3
chapter: false
pre: " <b> 4.3. </b> "
---

# Summary Report: "Workshop: Secure Your Applications - AWS Perimeter Protection"

### Event Information

- **Date**: Tuesday, November 19th, 2025
- **Time**: Full-day workshop
- **Location**: AWS Training Center, Ho Chi Minh City
- **Organizer**: AWS Vietnam
- **Event Type**: Hands-on Technical Workshop

### Instructors

- **Mr. Nguyen Gia Hung** – Head of Solutions Architects, AWS Vietnam
- **Mr. Julian Ju** – Regional Edge Security Specialist, AWS APAC
- **Mr. Kevin Lim** – Regional Edge Security Specialist, AWS APAC

### Event Objectives

- Understand AWS edge security services and perimeter protection strategies
- Learn how to protect web applications from common attacks (SQL Injection, XSS, DDoS)
- Master AWS WAF (Web Application Firewall) configuration and rule management
- Implement AWS Shield for DDoS protection and resilience
- Gain hands-on experience with real-world security scenarios
- Design secure application architectures using AWS edge services

### Workshop Structure

#### Session 1: Introduction to AWS Edge Security (Morning)

**Topics Covered:**
- Overview of AWS edge security services ecosystem
- Understanding the shared responsibility model for application security
- Common web application vulnerabilities (OWASP Top 10)
- AWS edge security architecture patterns

**Key Concepts:**
- **Edge Security**: Protecting applications at the network perimeter before threats reach backend infrastructure
- **Defense in Depth**: Multi-layered security approach
- **CloudFront Integration**: Content delivery with built-in security features

#### Session 2: AWS WAF Deep Dive (Late Morning)

**AWS WAF Fundamentals:**
- Web Application Firewall architecture and components
- Rule groups and rule priority
- WAF managed rules vs custom rules
- Integration with CloudFront, Application Load Balancer, and API Gateway

**Threat Protection Mechanisms:**
1. **SQL Injection Prevention**
   - Pattern matching for SQL syntax
   - Request body inspection
   - Query string analysis

2. **Cross-Site Scripting (XSS) Protection**
   - Script tag detection
   - JavaScript injection prevention
   - HTML entity encoding

3. **Rate Limiting**
   - Request throttling per IP
   - Bot detection and mitigation
   - Geographic restrictions

#### Session 3: Hands-on Lab - AWS WAF Configuration (Afternoon)

**Lab Objectives:**
Participants configured AWS WAF to protect a sample web application from various attacks.

**Lab Activities:**

**Part 1: Initial Setup**
- Created a CloudFront distribution with origin web server
- Deployed sample vulnerable web application for testing
- Set up CloudWatch logging for security monitoring

**Part 2: SQL Injection Protection**
```
Steps performed:
1. Created WAF Web ACL (Access Control List)
2. Added SQL Injection match condition
3. Configured rule to block suspicious SQL patterns
4. Tested with simulated SQL injection attacks
5. Verified blocking behavior in CloudWatch logs
```

**Key Configuration:**
- Rule Priority: High
- Action: Block
- Scope: Request body and query strings
- Patterns: Common SQL keywords (SELECT, UNION, DROP, etc.)

**Part 3: XSS Protection Implementation**
```
Steps performed:
1. Added XSS match condition to Web ACL
2. Configured script tag detection rules
3. Set up JavaScript pattern matching
4. Tested with XSS payloads
5. Analyzed blocked requests
```

**Part 4: Rate Limiting Rules**
```
Steps performed:
1. Created rate-based rule (1000 requests per 5 minutes)
2. Configured IP-based throttling
3. Simulated high-volume requests
4. Observed automatic blocking behavior
```

#### Session 4: AWS Shield for DDoS Protection (Late Afternoon)

**AWS Shield Overview:**
- **Shield Standard**: Automatic protection at no extra cost
- **Shield Advanced**: Enhanced DDoS protection with 24/7 support

**DDoS Attack Types Covered:**
1. **Network Layer Attacks (Layer 3/4)**
   - SYN floods
   - UDP reflection attacks
   - TCP connection exhaustion

2. **Application Layer Attacks (Layer 7)**
   - HTTP floods
   - Slowloris attacks
   - Application-specific exploits

**Shield Implementation:**
- Enabled AWS Shield Advanced for critical resources
- Configured DDoS Response Team (DRT) access
- Set up CloudWatch alarms for attack detection
- Reviewed cost protection policies

**Hands-on Activities:**
- Analyzed historical DDoS attack patterns
- Configured automatic attack mitigation
- Set up real-time attack notifications
- Reviewed DDoS attack reports and metrics

### Technical Deep Dives

#### AWS WAF Rule Design Best Practices

**1. Layered Protection Strategy**
```
Layer 1: Managed Rule Groups (AWS Managed Rules)
  - Core Rule Set (CRS)
  - Known Bad Inputs
  - Admin Protection

Layer 2: Rate-based Rules
  - Geographic rate limiting
  - IP reputation lists
  - Custom rate thresholds

Layer 3: Custom Business Logic Rules
  - Application-specific patterns
  - Authentication bypass prevention
  - Sensitive data exposure protection
```

**2. Rule Evaluation Order**
- Count rules for monitoring (no blocking)
- Allow rules for trusted sources
- Block rules for known threats
- Rate-based rules for volume control
- Default action (typically Allow)

#### Integration Architecture

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

**Benefits of Edge Protection:**
- Threats blocked before reaching infrastructure
- Reduced backend load and costs
- Improved application performance
- Global threat intelligence sharing

### Monitoring and Incident Response

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

**Incident Response Workflow:**
1. Alert triggered by CloudWatch alarm
2. Security team reviews blocked requests
3. Analyze attack patterns and sources
4. Adjust WAF rules if needed
5. Document incident for future reference

### Real-World Scenarios Discussed

#### Case Study 1: E-commerce Platform Protection
**Challenge**: Online retailer experiencing credential stuffing attacks
**Solution**: 
- Implemented rate-based rules per user session
- Added CAPTCHA challenges for suspicious IPs
- Configured custom rules for login endpoints
**Result**: 95% reduction in fraudulent login attempts

#### Case Study 2: API Gateway Security
**Challenge**: RESTful API vulnerable to injection attacks
**Solution**:
- Deployed WAF on API Gateway
- Created custom rules for API-specific threats
- Implemented request size limits
**Result**: Zero successful injection attacks post-deployment

#### Case Study 3: DDoS Attack Mitigation
**Challenge**: Media website targeted by 300 Gbps DDoS attack
**Solution**:
- AWS Shield Advanced automatic mitigation
- CloudFront geographic restrictions
- Emergency runbook activation
**Result**: Application remained available with < 1% performance impact

### Key Takeaways

#### Technical Skills Acquired

**AWS WAF Expertise:**
- ✅ Configured Web ACLs with multiple rule types
- ✅ Implemented SQL Injection and XSS protection
- ✅ Set up rate-based rules for bot mitigation
- ✅ Integrated WAF with CloudFront and ALB
- ✅ Analyzed security logs and metrics

**DDoS Protection Knowledge:**
- ✅ Understood different DDoS attack vectors
- ✅ Implemented AWS Shield protection layers
- ✅ Configured automatic attack response
- ✅ Set up monitoring and alerting systems

**Security Architecture:**
- ✅ Designed defense-in-depth strategies
- ✅ Applied edge security best practices
- ✅ Implemented zero-trust principles
- ✅ Optimized cost vs security trade-offs

#### Best Practices Learned

**1. Security by Design**
- Implement security controls from day one
- Regular security testing and updates
- Continuous monitoring and improvement

**2. Automation First**
- Automate threat detection and response
- Use managed rules when possible
- Implement Infrastructure as Code for consistency

**3. Cost Optimization**
- Start with Shield Standard (free tier)
- Use managed rules before custom rules
- Monitor and optimize rule efficiency

**4. Compliance and Governance**
- Document all security configurations
- Regular audit and compliance reviews
- Incident response playbooks

### Practical Applications

**Immediate Implementation Plans:**
1. **Week 1**: Deploy AWS WAF on development environment
2. **Week 2**: Configure core rule sets and test thoroughly
3. **Week 3**: Enable production deployment with monitoring
4. **Week 4**: Review metrics and optimize rules

**Skills to Practice:**
- Regular WAF rule testing and updates
- Security log analysis and pattern recognition
- Incident response procedures
- Cost monitoring and optimization

### Personal Reflection

This workshop was exceptionally valuable, providing deep technical knowledge about AWS edge security services. The hands-on labs with real attack scenarios made the learning highly practical and engaging.

**Most Valuable Aspects:**
- **Expert Instruction**: Learning from AWS regional specialists (Julian Ju and Kevin Lim) provided insights not available in documentation
- **Hands-on Practice**: Configuring WAF rules and testing with real attacks solidified theoretical knowledge
- **Real-world Cases**: Case studies demonstrated practical application in production environments
- **Architecture Patterns**: Understanding how to integrate multiple security services effectively

**Challenges Faced:**
- Rule priority and evaluation order initially confusing
- Balancing security strictness with false positive prevention
- Understanding cost implications of different configurations

**Key Learnings:**
- Edge security is critical for modern cloud applications
- AWS provides powerful tools, but proper configuration is essential
- Security is an ongoing process, not a one-time setup
- Integration of multiple services (WAF + Shield + CloudFront) provides comprehensive protection

**Future Applications:**
This knowledge is directly applicable to:
- Securing microservices architectures
- Protecting API endpoints
- Implementing compliance requirements (PCI-DSS, SOC 2)
- Designing resilient, security-first cloud applications

### Resources and References

**AWS Documentation:**
- AWS WAF Developer Guide
- AWS Shield Advanced Best Practices
- CloudFront Security Documentation
- Well-Architected Framework - Security Pillar

**Tools and Services Used:**
- AWS WAF (Web Application Firewall)
- AWS Shield (Standard and Advanced)
- Amazon CloudFront
- Application Load Balancer
- AWS CloudWatch
- AWS Config for compliance

**Additional Learning Resources:**
- AWS Security Hub for centralized security management
- AWS Firewall Manager for multi-account governance
- OWASP Top 10 vulnerability guides
- AWS Security Blog for latest threats and solutions

---

> **Summary**: This workshop provided comprehensive, hands-on training in AWS edge security services, specifically AWS WAF and AWS Shield. The combination of expert instruction from AWS specialists, practical labs with real attack scenarios, and real-world case studies made this an invaluable learning experience. The skills acquired are immediately applicable to securing production cloud applications and designing resilient, security-first architectures.
