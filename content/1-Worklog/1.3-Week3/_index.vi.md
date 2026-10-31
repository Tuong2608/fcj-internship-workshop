---
title: "Worklog Tuần 3"
date: 2026-10-23
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

## Daily Worklog — Thứ Sáu, 23/10/2026

**Nội dung:** Ôn tập Amazon VPC, Amazon EC2 và học mới về IAM Roles for EC2, AWS Cloud9.

### Công việc đã thực hiện

- Lên văn phòng thực tập, ôn tập củng cố lại hai chuyên đề mạng và máy chủ ảo đã tiếp cận, đồng thời học tiếp hai bài mới trong lộ trình First Cloud Journey:
  - **Amazon VPC (Ôn tập & Đào sâu):** Ôn lại cách thiết kế VPC với Public/Private Subnet, Route Table, Internet Gateway, NAT Gateway; tìm hiểu sâu hơn về Security Group, Network ACL, VPC Resource Map, Reachability Analyzer, Systems Manager Session Manager, VPC Flow Logs và mô hình kết nối Site-to-Site VPN.
  - **Amazon EC2 (Ôn tập & Thực hành):** Ôn lại quy trình khởi tạo và kết nối máy chủ Windows Server và Amazon Linux 2023 (qua RDP và SSH), triển khai ứng dụng web (LAMP, XAMPP, Node.js), tạo EBS Snapshot, Custom AMI, khôi phục quyền truy cập khi mất Key Pair và áp dụng IAM Policy để kiểm soát chi phí/tài nguyên EC2.
  - **IAM Roles for EC2:** Tìm hiểu cơ chế Instance Profile và cách cấp quyền cho ứng dụng chạy trên EC2 truy cập an toàn tới các dịch vụ AWS khác (như Amazon S3) thông qua IAM Role thay vì nhúng cứng Access Key / Secret Key của IAM User trong mã nguồn.
  - **AWS Cloud9:** Tìm hiểu môi trường tích hợp phát triển trên trình duyệt (Cloud IDE), cách khởi tạo Cloud9 environment gắn với EC2 và sử dụng terminal tích hợp sẵn AWS CLI để thao tác với tài nguyên AWS.

### Kết quả và bài học

- Nắm vững hơn luồng định tuyến giữa Public Subnet và Private Subnet, cũng như các công cụ kiểm tra kết nối và bảo mật mạng trong VPC.
- Củng cố kỹ năng vận hành EC2, sao lưu bằng EBS Snapshot / Custom AMI và giới hạn quyền triển khai EC2 theo Region, Instance Family/Type để tối ưu chi phí.
- Hiểu rõ nguyên tắc bảo mật quan trọng trên AWS: sử dụng IAM Role (cấp phát thông tin xác thực tạm thời) cho EC2 thay vì lưu trữ cố định khóa truy cập.
- Làm quen với việc phát triển và quản trị tài nguyên thông qua môi trường đám mây AWS Cloud9.

### Tài liệu tham khảo

1. [Networking Essentials with Amazon Virtual Private Cloud (VPC)](https://000003.awsfcaj.com/)
2. [Compute Essentials with Amazon Elastic Compute Cloud (EC2)](https://000004.awsfcaj.com/)
3. [Instance Profiling with IAM Roles for EC2](https://000048.awsfcaj.com/)
4. [Cloud Development with AWS Cloud9](https://000049.awsfcaj.com/)

---

## Weekly Worklog — 19–23/10/2026

### Mục tiêu trong tuần

- Ôn tập và nắm chắc kiến thức thực hành về hạ tầng mạng Amazon VPC và máy chủ ảo Amazon EC2.
- Hiểu và áp dụng cơ chế cấp quyền cho ứng dụng trên EC2 thông qua IAM Role.
- Làm quen với công cụ phát triển trên đám mây AWS Cloud9.

### Công việc đã thực hiện

| Ngày | Nội dung | Tài liệu |
|---|---|---|
| 23/10/2026 | Lên văn phòng ôn tập và thực hành chuyên sâu về Amazon VPC, NAT Gateway, kiểm soát lưu lượng và các công cụ chẩn đoán kết nối. | [Amazon VPC](https://000003.awsfcaj.com/) |
| 23/10/2026 | Ôn tập triển khai máy chủ Amazon EC2 (Linux/Windows), quản lý EBS Snapshot, Custom AMI và chính sách IAM quản trị chi phí. | [Amazon EC2](https://000004.awsfcaj.com/) |
| 23/10/2026 | Học và thực hành cấp quyền cho ứng dụng trên EC2 truy cập dịch vụ AWS thông qua IAM Role (Instance Profile). | [IAM Roles for EC2](https://000048.awsfcaj.com/) |
| 23/10/2026 | Tìm hiểu và thực hành sử dụng môi trường Cloud IDE với AWS Cloud9 và AWS CLI tích hợp. | [AWS Cloud9](https://000049.awsfcaj.com/) |

### Kết quả đạt được

- Củng cố vững chắc kiến thức nền tảng về mạng (VPC) và tính toán (EC2) thông qua buổi học và ôn tập tại văn phòng.
- Hiểu rõ lý do và cách thức sử dụng IAM Role cho EC2 để đảm bảo an toàn bảo mật khi ứng dụng cần gọi tới các dịch vụ AWS khác.
- Biết cách khởi tạo và sử dụng AWS Cloud9 để phục vụ việc lập trình và chạy lệnh quản trị trên trình duyệt.
- Chuẩn bị tốt kiến thức nền tảng để tiếp cận các dịch vụ cơ sở dữ liệu, container và tự động mở rộng quy mô ở tuần kế tiếp.

### Nội dung cần củng cố

- Thực hành thêm việc kiểm tra đường đi của gói tin và kết nối an toàn vào Private Subnet bằng VPC Reachability Analyzer và Session Manager.
- Rèn luyện thói quen phân quyền tối thiểu (Least Privilege) khi gắn IAM Role cho máy chủ EC2.
- Kiểm tra và dọn dẹp triệt để các tài nguyên phát sinh phí theo giờ (như NAT Gateway, Elastic IP, EC2, Cloud9) sau khi hoàn tất bài thực hành.
