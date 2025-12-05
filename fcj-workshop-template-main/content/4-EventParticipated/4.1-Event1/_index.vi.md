---
title: "Event 1"
date: "2025-10-03"
weight: 1
chapter: false
pre: " <b> 4.1. </b> "
---


# Báo cáo tham dự: "AI-Driven Development Life Cycle: Reimagining Software Engineering"

### Thông tin sự kiện

- **Ngày**: Thứ Sáu, 3 tháng 10, 2025
- **Thời gian**: 2:00 PM - 4:30 PM
- **Địa điểm**: AWS Event Hall, Tầng 26 Bitexco Tower, HCMC
- **Tổ chức**: AWS GenAI Builder Club
- **Điều phối viên**: Diem My, Dai Truong, Dinh Nguyen

### Mục đích của sự kiện

- Khám phá cách generative AI chuyển đổi vòng đời phát triển phần mềm
- Trình bày quy trình phát triển AI-powered từ kiến trúc đến bảo trì
- Giới thiệu Amazon Q Developer và Kiro cho phát triển có hỗ trợ AI
- Trình bày cách tự động hóa AI tăng năng suất và cho phép tập trung vào các tác vụ sáng tạo
- Cung cấp kinh nghiệm thực hành với các công cụ và phương pháp AI-driven development

### Diễn giả & Lịch trình

**2:00 PM - 2:15 PM: Chào mừng**
**2:15 PM - 3:30 PM: Tổng quan AI-Driven Development Life Cycle & Trình diễn Amazon Q Developer**
- **Toàn Huỳnh** – Giảng viên, Chuyên gia AI-Driven Development

**3:30 PM - 3:45 PM: Giải lao**
**3:45 PM - 4:30 PM: Trình diễn Kiro**
- **My Nguyễn** – Giảng viên, Chuyên gia Công cụ AI Development

### Nội Dung Nổi Bật

#### AI-DLC Standard Development Workflow

Workshop giới thiệu **quy trình phát triển 4 giai đoạn** toàn diện:

- **REQUIREMENT**: Product Owner xác định nhu cầu business và user stories
- **DESIGN**: Software Architect tạo system design và architecture  
- **IMPLEMENTATION**: Software Engineers phát triển và code giải pháp
- **DEPLOYMENT**: DevOps team xử lý deployment và operations

Đây là **spec-driven development** approach trong đó mỗi giai đoạn được định nghĩa rõ ràng và có sự hỗ trợ của AI.

#### AI-DLC Steps Framework

Phương pháp theo cách tiếp cận có cấu trúc với nhiều thành phần:

- **Requirements**: Thu thập yêu cầu business và kỹ thuật ban đầu
- **Vibe Coding**: AI-assisted rapid prototyping và code generation
- **Code**: Phát triển production-ready code với AI support

**Ba Giai Đoạn Chính:**
- **Inception**: Lập kế hoạch dự án, user stories và thiết lập ban đầu
- **Construction**: Domain design, logical design và implementation
- **Operation**: Deployment, testing và maintenance

#### AI-Driven Development Lifecycle (9 Bước)

Workshop trình bày chi tiết **quy trình 9 bước**:

1. **Build Context on Existing Codes** - Phân tích codebase hiện tại
2. **Elaborate Intent with User Stories** - Định nghĩa yêu cầu rõ ràng  
3. **Plan with Units of Work** - Chia nhỏ thành các task quản lý được
4. **Domain Model (Component Model)** - Thiết kế system architecture
5. **Generate code & Test** - AI-assisted code generation
6. **Add architectural components** - Tích hợp system components
7. **Deploy with IaaC & tests** - Infrastructure as Code deployment
8. **Deploy in production with** - Production deployment strategies
9. **Manage incidents** - Ongoing maintenance và issue resolution

#### Project Structure và Organization

Workshop trình bày **repository organization** phù hợp:

- **Root Directory**: Chứa nhiều independent Flask applications
- **`.kiro/` folder**: Chứa specifications, steering rules và settings
- **`requirements.txt`**: Shared dependencies cho tất cả applications

**Application Structure** theo consistent patterns:
- Flask environment configuration
- Application file với routes và logic  
- Database models (nếu applicable)
- Static assets (CSS, JS, Images)
- HTML templates

#### Prompt Engineering cho Development

Workshop nhấn mạnh tầm quan trọng của **effective prompt templates**:

- **Role Definition**: "You are an expert software architect..."
- **Task Specification**: Hướng dẫn rõ ràng, actionable cho AI
- **Context Provision**: Thông tin background liên quan
- **Output Format**: Structured markdown với checkboxes để tracking
- **Iterative Refinement**: Quy trình cải thiện và validate AI responses

### Những Gì Học Được

#### Triết Lý AI-Assisted Development

- **Human-AI Collaboration**: Cân bằng giữa AI capabilities và human oversight
- **Iterative Validation**: Luôn validate và review AI-generated code trước khi implementation
- **Context-Aware Prompting**: Cung cấp đủ context để AI generate các giải pháp liên quan
- **Structured Approach**: Theo systematic methodology thay vì ad-hoc AI usage

#### Technical Implementation

- **Modular Architecture**: Mỗi application component nên independently deployable
- **Specification-Driven**: Sử dụng clear specifications và steering rules cho consistency
- **Template-Based Development**: Leverage proven patterns và templates cho faster development
- **Infrastructure as Code**: Automate deployment và infrastructure management

#### Project Management với AI

- **Unit-Based Planning**: Chia complex projects thành manageable, AI-assistable units
- **User Story Elaboration**: Sử dụng AI để expand và clarify business requirements
- **Domain Modeling**: Áp dụng AI để tạo comprehensive component models
- **Continuous Integration**: Implement automated testing và deployment pipelines

### Ứng Dụng Vào Công Việc

- **Implement AI-DLC Framework**: Áp dụng quy trình 9 bước cho current development projects
- **Create Prompt Templates**: Phát triển standardized prompts cho common development tasks
- **Establish Project Structure**: Adopt modular Flask application architecture được trình bày
- **Integrate AI Tools**: Sử dụng AI cho code generation, testing và documentation
- **Practice Spec-Driven Development**: Bắt đầu với clear specifications trước implementation
- **Build Context Libraries**: Maintain reusable components và patterns cho AI assistance

### Trải nghiệm trong event

Tham gia workshop **"AI-Driven Development Lifecycle (AI-DLC)"** là một trải nghiệm rất thú vị, thay đổi hoàn toàn quan điểm của tôi về phát triển phần mềm trong kỷ nguyên AI. Một số trải nghiệm nổi bật:

#### Học structured AI development methodology
- **Quy trình AI-DLC 9 bước** cung cấp framework rõ ràng để tích hợp AI trong toàn bộ software development lifecycle.
- Hiểu về **3-phase approach** (Inception, Construction, Operation) giúp tôi thấy cách AI có thể hỗ trợ ở mỗi giai đoạn.
- **Spec-driven development model** chứng minh tầm quan trọng của clear requirements trước AI implementation.

#### Hands-on AI-assisted development
- Học practical **prompt engineering techniques** từ **Toan Huynh** cho software development tasks.
- Trải nghiệm cách structure **project repositories** cho AI-friendly development theo hướng dẫn của Amazon Q Developer.
- Hiểu tầm quan trọng của **context provision** khi làm việc với AI coding assistants.
- Thực hành tạo **modular Flask applications** với proper separation of concerns.
- Demo ấn tượng về **Kiro tool** từ **My Nguyen** cho real-time AI development assistance.

#### Technical architecture insights
- **Standard development workflow** (Requirement → Design → Implementation → Deployment) cung cấp solid foundation cho AI integration.
- Học về **role-based development** nơi Product Owners, Software Architects và Engineers collaborate với AI tools.
- Hiểu **domain modeling** và **component architecture** trong AI-assisted environment.

#### Practical implementation strategies
- Thấy real examples của **AI-generated code** và học validation techniques.
- Hiểu cách chia complex projects thành **manageable AI-assistable units**.
- Học về **Infrastructure as Code (IaaC)** deployment strategies với AI support.
- Có insights về **incident management** trong AI-assisted development environments.

#### Collaboration và workflow optimization
- Workshop nhấn mạnh **human-AI collaboration** thay vì AI replacement của developers.
- Học tầm quan trọng của **iterative validation** và human oversight trong AI-generated solutions.
- Hiểu cách AI có thể enhance **team productivity** mà vẫn maintain code quality và security.

#### Bài học rút ra
- AI tools cần **structured approaches** và **clear methodologies** để effective trong professional development.
- **Prompt engineering** skills từ **Toan Huynh** về Amazon Q Developer là crucial cho modern developers.
- **Context-aware development** approach significantly improves AI assistance quality theo demo của **Kiro tool**.
- **Template-based development** patterns có thể accelerate AI-assisted project delivery như được thể hiện trong workshop.


> Tổng thể, workshop này không chỉ cung cấp practical AI development skills mà còn thiết lập systematic approach để tích hợp AI tools vào professional software development workflows. Structured methodology đảm bảo rằng AI enhances thay vì complicates development process.
