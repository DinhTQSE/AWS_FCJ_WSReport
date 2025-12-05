---
title: "Event 2"
date: "2025-10-18"
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---

# Báo cáo tham dự: "Workshop Data Science trên AWS"

### Thông tin sự kiện

- **Ngày**: 18 tháng 10, 2025
- **Thời gian**: 9:30 - 11:45 sáng
- **Địa điểm**: Hội trường A - Đại học FPT HCMC
- **Chủ trì**: Đoàn Nguyễn Thành Hòa - Giảng viên CF, Đại học FPT HCMC

### Mục đích của sự kiện

- Cung cấp kiến thức nền tảng về Machine Learning và AI
- Giới thiệu hệ sinh thái AWS AI/ML và các dịch vụ
- Chia sẻ phương pháp thực tế cho các dự án data science
- Hướng dẫn sinh viên xây dựng giải pháp ML sử dụng nền tảng AWS cloud

### Danh sách diễn giả

- **Văn Hoàng Kha** – Cloud Solutions Architect, AWS User Group Leaders
- **Bạch Doãn Vương** – Cloud DevOps Engineer, AWS Community Builder

### Nội dung nổi bật

#### Kiến thức nền tảng về Machine Learning

**Định nghĩa**: Machine Learning (ML) là một lĩnh vực của AI, cho phép máy tính "học" từ dữ liệu để thực hiện tác vụ mà không cần lập trình tường minh.

**Ba loại chính**:
- **Học có giám sát (Supervised Learning)**: Học từ dữ liệu đã được gán nhãn (ví dụ: phân loại email spam)
- **Học không giám sát (Unsupervised Learning)**: Tự tìm ra cấu trúc trong dữ liệu chưa được gán nhãn (ví dụ: phân nhóm khách hàng)
- **Học tăng cường (Reinforcement Learning)**: Học qua thử và sai bằng cách tương tác với môi trường (ví dụ: AI chơi game, xe tự lái)

#### Quy trình của một dự án Machine Learning

Vòng đời chuẩn của bất kỳ dự án Data Science nào bao gồm 4 giai đoạn chính:

1. **Xác định vấn đề**: Chuyển bài toán kinh doanh thành bài toán máy học
2. **Xử lý dữ liệu**: Thu thập, làm sạch, và phân tích dữ liệu (thường chiếm nhiều thời gian nhất)
3. **Xây dựng mô hình**:
   - **Feature Engineering**: Tạo ra các đặc trưng tốt nhất cho mô hình
   - **Training & Tuning**: Huấn luyện và tinh chỉnh mô hình
   - **Evaluation**: Đánh giá độ chính xác của mô hình
4. **Triển khai & Vận hành (MLOps)**: Đưa mô hình vào sử dụng thực tế, liên tục giám sát, và huấn luyện lại khi cần thiết

#### Hệ sinh thái AI/ML của AWS

AWS cung cấp một bộ công cụ toàn diện gồm 3 tầng, phục vụ mọi đối tượng người dùng:

**Tầng 1: AI Services (Dịch vụ AI tạo sẵn - Dùng API)**
Các dịch vụ "thông minh" có thể tích hợp ngay vào ứng dụng mà không cần chuyên môn về ML:

*Xử lý Ngôn ngữ & Âm thanh*:
- **Amazon Comprehend**: "Đọc hiểu" văn bản (phân tích cảm xúc, trích xuất thực thể)
- **Amazon Translate**: "Dịch" văn bản giữa các ngôn ngữ
- **Amazon Textract**: "Đọc" và trích xuất văn bản/dữ liệu từ tài liệu, hình ảnh (OCR thông minh)
- **Amazon Polly**: "Nói" (chuyển văn bản thành giọng nói tự nhiên)
- **Amazon Transcribe**: "Nghe" (chuyển giọng nói thành văn bản)
- **Amazon Lex**: "Bộ não" xây dựng chatbot và voice bot hội thoại (công nghệ của Alexa)

*Thị giác Máy tính*:
- **Amazon Rekognition**: "Nhìn" và phân tích hình ảnh/video (phát hiện đối tượng, nhận dạng khuôn mặt)

*Cá nhân hóa*:
- **Amazon Personalize**: Xây dựng hệ thống gợi ý (recommendation engine) mạnh mẽ (công nghệ của Amazon.com)

**Tầng 2: ML Services (Nền tảng Máy học)**
- **Amazon SageMaker**: Nền tảng tích hợp toàn diện, cung cấp công cụ cho mọi bước trong quy trình máy học, từ chuẩn bị dữ liệu đến huấn luyện, triển khai và giám sát mô hình

**Tầng 3: ML Frameworks & Infrastructure (Hạ tầng & Nền tảng)**
- **Hỗ trợ đầy đủ**: Cung cấp các máy chủ mạnh mẽ (CPU, GPU, chip chuyên dụng AWS) và hỗ trợ mọi framework phổ biến
- **Frameworks chính**: TensorFlow (mạnh mẽ, toàn diện), PyTorch (linh hoạt, trực quan)
- **Linh hoạt tối đa**: Cho phép mang môi trường tùy chỉnh lên AWS thông qua "Bring Your Own Container"

### Những gì học được

#### Tư duy cốt lõi & Lời khuyên thực tế

**Tư duy quan trọng nhất**:
- **Thinking like a Cloud Engineer, Not only AI Engineer**: Để thành công, bạn không chỉ cần xây dựng mô hình chính xác mà còn phải biết cách triển khai, mở rộng, tối ưu chi phí và bảo mật nó trên nền tảng đám mây

#### Nguồn dữ liệu cho cá nhân

**Kho dữ liệu công khai**:
- **Kaggle**, **Hugging Face Hub**, **UCI Repository** là những nơi tốt nhất để bắt đầu

**Tự tạo dữ liệu**:
- Sử dụng kỹ thuật **Web Scraping** (cào dữ liệu web), API, hoặc dùng chính AI để tạo **dữ liệu giả lập (Synthetic Data)**

#### Chiến lược AWS ML

**Phương pháp ba tầng**:
- **Bắt đầu đơn giản**: Sử dụng AI Services cho các quick wins và proof of concepts
- **Mở rộng thông minh**: Chuyển sang SageMaker cho các quy trình ML tùy chỉnh
- **Tối ưu sâu**: Tận dụng tầng infrastructure để đạt hiệu suất và tối ưu chi phí tối đa

#### Best practices triển khai

- **Chất lượng dữ liệu đầu tiên**: Dữ liệu sạch, phù hợp quan trọng hơn thuật toán phức tạp
- **Bắt đầu từ vấn đề kinh doanh**: Không xây dựng ML vì mục đích công nghệ
- **Lặp lại nhanh chóng**: Sử dụng dịch vụ managed của AWS để tập trung vào logic kinh doanh, không phải hạ tầng
- **Giám sát liên tục**: Mô hình ML suy giảm theo thời gian và cần được chú ý liên tục

### Ứng dụng vào công việc

- **Bắt đầu với AI Services**: Sử dụng Amazon Rekognition, Comprehend, hoặc Translate cho các quick wins trong dự án hiện tại
- **Khám phá SageMaker**: Bắt đầu với SageMaker Studio để khám phá dữ liệu và thử nghiệm mô hình
- **Thực hành thu thập dữ liệu**: Sử dụng web scraping và public datasets để xây dựng các dự án ML cá nhân
- **Học MLOps**: Hiểu toàn bộ vòng đời ML từ phát triển đến triển khai production
- **Xây dựng cloud-native**: Thiết kế các giải pháp ML với khả năng mở rộng, tối ưu chi phí và bảo mật
- **Tham gia cộng đồng AWS**: Kết nối với AWS User Groups và Community Builders để chia sẻ kiến thức

### Trải nghiệm trong sự kiện

Tham gia workshop **"Data Science trên AWS"** tại Đại học FPT là một trải nghiệm thú vị, cung cấp những hiểu biết toàn diện về machine learning và các dịch vụ AWS cloud. Một số trải nghiệm nổi bật:

#### Học hỏi từ các chuyên gia AWS
- **Văn Hoàng Kha** và **Bạch Doãn Vượng** đã chia sẻ kiến thức sâu rộng về **hệ sinh thái AWS AI/ML** và các chiến lược triển khai thực tế.
- Thông qua các ví dụ thực tế, tôi hiểu sâu hơn về **kiến trúc AWS ML 3 tầng** và cách các dịch vụ khác nhau bổ trợ cho nhau.

#### Hiểu về nền tảng ML
- Học được **ba loại chính của machine learning**: supervised, unsupervised, và reinforcement learning với các ví dụ rõ ràng.
- Hiểu về **vòng đời hoàn chỉnh của dự án ML** từ định nghĩa vấn đề đến triển khai và vận hành liên tục.
- Khám phá tầm quan trọng của **chất lượng dữ liệu và feature engineering** trong việc xây dựng mô hình ML thành công.

#### Khám phá các dịch vụ AWS AI
- Được tiếp xúc thực tế với **các dịch vụ AI có sẵn** như Amazon Comprehend, Rekognition, và Translate có thể tích hợp ngay lập tức.
- Học về **Amazon SageMaker** như một nền tảng toàn diện cho quy trình ML tùy chỉnh và quản lý mô hình.
- Hiểu về **tầng hạ tầng** hỗ trợ các framework phổ biến như TensorFlow và PyTorch.

#### Phát triển tư duy cloud-native
- Khái niệm **"Think like a Cloud Engineer, Not only AI Engineer"** đặc biệt có giá trị, nhấn mạnh tầm quan trọng của triển khai, mở rộng và tối ưu chi phí.
- Học về **thực hành MLOps** và nhu cầu giám sát liên tục và huấn luyện lại mô hình.
- Hiểu về sự cân bằng giữa **khả năng kỹ thuật và yêu cầu kinh doanh**.

#### Hướng dẫn thực tế cho việc thu thập dữ liệu
- Khám phá các **bộ dữ liệu công khai** có giá trị trên Kaggle, Hugging Face Hub, và UCI Repository để học tập và thử nghiệm.
- Học về **kỹ thuật web scraping** và sử dụng AI để tạo dữ liệu synthetic cho mục đích huấn luyện.
- Hiểu tầm quan trọng của **chuẩn bị và làm sạch dữ liệu** như phần tốn thời gian nhất của các dự án ML.

#### Xây dựng mạng lưới và cộng đồng
- Kết nối với **các AWS community builders** và học về sự hỗ trợ liên tục thông qua các user groups.
- Trao đổi ý tưởng với các sinh viên và chuyên gia khác quan tâm đến data science và cloud computing.
- Có cái nhìn sâu sắc về **con đường sự nghiệp** trong lĩnh vực cloud engineering và data science.


> Tổng thể, workshop này không chỉ cung cấp kiến thức kỹ thuật về các dịch vụ AWS ML mà còn giúp tôi hiểu được hành trình hoàn chỉnh từ các vấn đề kinh doanh đến các giải pháp ML được triển khai, nhấn mạnh tầm quan trọng của tư duy cloud-native trong các dự án data science hiện đại.
