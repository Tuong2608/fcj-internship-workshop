---
title: "Worklog Tuần 4"
date: 2026-10-30
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

## Daily Worklog — Thứ Sáu, 30/10/2026

**Nội dung:** Học và thực hành về Amazon RDS, Amazon Lightsail, Amazon Lightsail Containers và EC2 Auto Scaling.

### Công việc đã thực hiện

- Lên văn phòng thực tập và học, thực hành bốn bài hướng dẫn tiếp theo trong lộ trình First Cloud Journey về cơ sở dữ liệu quan hệ, điện toán đơn giản hóa, triển khai container và tự động mở rộng quy mô:
  - **Amazon RDS:** Tìm hiểu dịch vụ cơ sở dữ liệu quan hệ có quản lý trên AWS; thực hành thiết lập VPC, DB Subnet Group, Security Group, khởi tạo RDS instance, kết nối ứng dụng trên EC2 tới cơ sở dữ liệu RDS và thực hiện sao lưu tự động (Automated Backup) cũng như tạo bản sao lưu thủ công (Manual Snapshot).
  - **Amazon Lightsail:** Tìm hiểu cách triển khai nhanh máy chủ ảo và cơ sở dữ liệu bằng Lightsail OS / Application Blueprints (WordPress, PrestaShop, Akaunting); cấu hình địa chỉ IP tĩnh (Static IP), tường lửa, tạo Snapshot dự phòng, nâng cấp cấu hình instance và thiết lập cảnh báo (Alarms).
  - **Amazon Lightsail Containers:** Tìm hiểu dịch vụ triển khai container đơn giản hóa trên Lightsail; nắm quy trình cấu hình mức tài nguyên (Power & Scale), đẩy và chạy Docker container image cũng như cung cấp truy cập qua HTTPS endpoint tích hợp sẵn.
  - **EC2 Auto Scaling:** Tìm hiểu kiến trúc ứng dụng web có tính sẵn sàng cao kết hợp giữa VPC, RDS, Custom AMI, Launch Template, bộ cân bằng tải Application Load Balancer (ALB) cùng Target Group và EC2 Auto Scaling Group (ASG); tìm hiểu 4 phương thức mở rộng quy mô: Manual Scaling, Scheduled Scaling, Dynamic Scaling (theo CloudWatch metrics) và Predictive Scaling.

### Kết quả và bài học

- Hiểu cách tách biệt tầng cơ sở dữ liệu (Amazon RDS) khỏi tầng ứng dụng (EC2) và kiểm soát truy cập chặt chẽ giữa hai tầng bằng Security Group và DB Subnet Group.
- Nắm được ưu điểm của Amazon Lightsail và Lightsail Containers trong việc triển khai nhanh các ứng dụng web vừa và nhỏ hoặc container với mức chi phí cố định, dễ dự toán.
- Hiểu cơ chế phối hợp giữa Application Load Balancer và EC2 Auto Scaling trên nhiều Availability Zone giúp hệ thống tự động thích ứng với tải truy cập và tăng khả năng chịu lỗi.

### Tài liệu tham khảo

1. [Database Essentials with Amazon Relational Database Service (RDS)](https://000005.awsfcaj.com/)
2. [Simplified Computing with Amazon Lightsail](https://000045.awsfcaj.com/)
3. [Container Deployment with Amazon Lightsail Containers](https://000046.awsfcaj.com/)
4. [Scaling Applications with EC2 Auto Scaling](https://000006.awsfcaj.com/)

---

## Weekly Worklog — 26–30/10/2026

### Mục tiêu trong tuần

- Nắm vững cách khởi tạo, bảo mật, kết nối và sao lưu cơ sở dữ liệu quan hệ với Amazon RDS.
- Làm quen với giải pháp triển khai máy chủ và container tinh gọn bằng Amazon Lightsail và Lightsail Containers.
- Hiểu cách thiết kế và triển khai hệ thống web có khả năng tự động co giãn (Auto Scaling) và cân bằng tải (Load Balancing) trên AWS.

### Công việc đã thực hiện

| Ngày | Nội dung | Tài liệu |
|---|---|---|
| 30/10/2026 | Học và thực hành khởi tạo cơ sở dữ liệu Amazon RDS, cấu hình DB Subnet Group, Security Group, kết nối từ ứng dụng trên EC2 và sao lưu dữ liệu. | [Amazon RDS](https://000005.awsfcaj.com/) |
| 30/10/2026 | Học và thực hành triển khai ứng dụng trên Amazon Lightsail, gán Static IP, tạo Snapshot, nâng cấp máy chủ và cài đặt cảnh báo. | [Amazon Lightsail](https://000045.awsfcaj.com/) |
| 30/10/2026 | Tìm hiểu và thực hành triển khai ứng dụng đóng gói bằng container thông qua dịch vụ Amazon Lightsail Containers. | [Lightsail Containers](https://000046.awsfcaj.com/) |
| 30/10/2026 | Học và thực hành thiết lập Launch Template, Application Load Balancer và EC2 Auto Scaling Group với các chiến lược mở rộng quy mô khác nhau. | [EC2 Auto Scaling](https://000006.awsfcaj.com/) |

### Kết quả đạt được

- Mở rộng kiến thức từ việc chạy một máy chủ đơn lẻ sang kiến trúc nhiều tầng (Multi-tier architecture) kết hợp giữa ALB, EC2 Auto Scaling và Amazon RDS.
- Biết cách sử dụng Amazon Lightsail để triển khai nhanh cả ứng dụng cài đặt sẵn trên OS/Blueprint lẫn ứng dụng chạy trên nền tảng Container.
- Phân biệt rõ các kịch bản áp dụng của Manual Scaling, Scheduled Scaling, Dynamic Scaling và Predictive Scaling trong thực tế vận hành.
- Rèn luyện quy trình dọn dẹp tài nguyên theo đúng thứ tự phụ thuộc (xóa Auto Scaling Group, Load Balancer, Target Group, RDS, Lightsail) để tránh phát sinh chi phí ngoài ý muốn.

### Nội dung cần củng cố

- Tìm hiểu sâu hơn về tính năng Multi-AZ và Read Replica của Amazon RDS để tăng tính sẵn sàng và hiệu năng đọc dữ liệu.
- Ôn lại cách thiết lập ngưỡng cảnh báo CloudWatch Alarm và thời gian chờ (Cooldown period) khi cấu hình Dynamic Scaling cho EC2 Auto Scaling.
- So sánh bài toán sử dụng Lightsail Containers với các dịch vụ điều phối container chuyên sâu hơn như Amazon ECS và AWS Fargate.
