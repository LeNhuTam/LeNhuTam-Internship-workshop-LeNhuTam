---
title : "Cấu hình giám sát CloudWatch"
date: 2024-01-01
weight : 5 
chapter : false
pre : " <b> 5. </b> "
---

Mở cmd
Chạy lệnh configure

![Connect](/images/5.fwd/51-auto.png)

Sau khi chạy configure chúng ta chạy.
aws application-autoscaling register-scalable-target --service-namespace lambda --resource-id function:lambda-performance-test:prod --scalable-dimension lambda:function:ProvisionedConcurrency --min-capacity 1 --max-capacity 5.

![Connect](/images/5.fwd/52-auto.png)

Vậy là bạn vừa đăng ký Mục tiêu có thể mở rộng cho tính năng đồng thời được cung cấp
Bật tính năng đồng thời được cung cấp.

![Connect](/images/5.fwd/53-auto.png)

Kết quả test:

![Connect](/images/5.fwd/54-auto.png)

**Cấu hình như trong hình**.

![Connect](/images/5.fwd/55-auto.png)

Tương tự 512 và 1024 thì thay vào Memory là được
Chạy thử 5 lần  cho kết quả như sau :


**Nhận xét:**.
Lambda function của bạn rất nhẹ (hầu như chỉ trả về JSON).
Tăng Memory từ 128 → 512 → 1024 không tạo khác biệt đáng kể về thời gian chạy.
128MB là tối ưu về chi phí, vì:
Memory nhỏ nhất = giá rẻ nhất.
Thời gian chạy gần như bằng nhau.


**Tạo bảng điều khiển giám sát**.

![Connect](/images/5.fwd/56-auto.png)

**Bảng điều khiển giám sát**

![Connect](/images/5.fwd/57-auto.png)

**Đã tạo thành công Chính sách mở rộng để tự động điều chỉnh Đồng thời được cung cấp**

![Connect](/images/5.fwd/58-auto.png)

![Connect](/images/5.fwd/59-auto.png)

![Connect](/images/5.fwd/590-auto.png)

![Connect](/images/5.fwd/591-auto.png)
