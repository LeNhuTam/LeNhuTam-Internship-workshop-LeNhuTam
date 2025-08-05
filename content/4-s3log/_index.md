---
title : "Configure API Gateway"
date: 2024-01-01
weight : 4 
chapter : false
pre : " <b> 4. </b> "
---
Configure API Gateway.
- Create REST API connect Lambda.
Create HTTP API Gateway to call Lambda via URL.
Link API Gateway with function
lambda-performance-test
Deploy stage prod.
- Deploy API and get Invoke URL
Get endpoint URL:**https://661l0vt812.execute-api.ap-southeast-1.amazonaws.com/default/lambda-performance-test**.
Test curl to confirm Lambda works:Open cmd and copy this endpoint URL into: **curl “https://661l0vt812.execute-api.ap-southeast-1.amazonaws.com/default/lambda-performance-test”**.
Result:

![Connect](/images/4.s3/41-Configure-API-Gateway.png)
