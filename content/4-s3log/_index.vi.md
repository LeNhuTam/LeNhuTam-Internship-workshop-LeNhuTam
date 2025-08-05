---
title : "Cấu hình API Gateway"
date: 2024-01-01
weight : 4 
chapter : false
pre : " <b> 4. </b> "
---

Cấu hình API Gateway.
- Tạo REST API connect Lambda.
Tạo HTTP API Gateway để gọi Lambda qua URL.
Liên kết API Gateway với hàm lambda-performance-test
Triển khai giai đoạn prod.
- Triển khai API và lấy URL Invoke
Lấy URL điểm cuối:**https://661l0vt812.execute-api.ap-southeast-1.amazonaws.com/default/lambda-performance-test**.
Kiểm tra curl để xác nhận Lambda hoạt động: Mở cmd và sao chép URL điểm cuối này vào:**curl “https://661l0vt812.execute-api.ap-southeast-1.amazonaws.com/default/lambda-performance-test”**.
Kết quả:

![Connect](/images/4.cap/41-Configure-API-Gateway.png)