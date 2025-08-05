---
title : "Clean up resources"
date: 2024-01-01
weight : 6 
chapter : false
pre : " <b> 6. </b> "
---


1. **Delete Lambda Function & Alias**.
• Go to AWS Lambda => Functions => Select function lambda-performance-test.
• Delete alias prod first, then delete the function.

![Connect](/images/6.clean/61-Clean.png)

![Connect](/images/6.clean/62-Clean.png)

![Connect](/images/6.clean/63-Clean.png)

![Connect](/images/6.clean/64-Clean.png)

![Connect](/images/6.clean/65-Clean.png)

2. **Delete API Gateway**.
Run this command in cmd: aws apigateway get -rest-api.

![Connect](/images/6.clean/66-Clean.png)

**Wish everyone a successful practice**.