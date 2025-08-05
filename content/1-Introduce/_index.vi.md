---
title : "Giới thiệu"
date: 2024-01-01
weight : 1 
chapter : false
pre : " <b> 1. </b> "
---
**AWS Lambda** là một dịch vụ điện toán không máy chủ (serverless) do Amazon Web Services cung cấp, cho phép bạn chạy mã mà không cần quản lý máy chủ. Bạn chỉ cần viết mã và triển khai, còn việc xử lý hạ tầng, mở rộng, bảo trì đều do AWS tự động đảm nhiệm.

 Đặc điểm chính:
- Không cần quản lý server: Không cần cấu hình, vận hành hay cập nhật hệ điều hành.
- Tự động mở rộng: Lambda tự động scale theo số lượng yêu cầu thực tế.
- Trả phí theo mức sử dụng: Bạn chỉ trả tiền cho thời gian thực thi và số lần gọi hàm, không tốn phí khi không dùng.
- Hỗ trợ nhiều ngôn ngữ: Node.js, Python, Java, Go, .NET, Ruby và hơn thế nữa.
- Tích hợp sâu với các dịch vụ AWS: Có thể kích hoạt từ S3, API Gateway, DynamoDB, CloudWatch, EventBridge, v.v.

 Ứng dụng phổ biến:
- Xử lý ảnh, video, file ngay khi tải lên S3.
- Tự động phản hồi các sự kiện API hoặc webhook.
- Tự động backup, đồng bộ dữ liệu.
- Xây dựng microservices hoặc backend đơn giản.