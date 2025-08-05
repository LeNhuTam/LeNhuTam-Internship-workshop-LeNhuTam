---
title : "Set Auto Adjust for Provisioned Concurrency"
date: 2024-01-01
weight : 5 
chapter : false
pre : " <b> 5. </b> "
---

Open cmd.
Run configure command.

![Connect](/images/5.fwd/51-auto.png)

After running configure we run
aws application-autoscaling register-scalable-target --service-namespace lambda --resource-id function:lambda-performance-test:prod --scalable-dimension lambda:function:ProvisionedConcurrency --min-capacity 1 --max-capacity 5

![Connect](/images/5.fwd/52-auto.png)

So you've just registered a Scalable Goal for Provisioned Concurrency
Enable Provisioned Concurrency.

![Connect](/images/5.fwd/53-auto.png)

Test results:

![Connect](/images/5.fwd/54-auto.png)

**Configuration as shown in picture**.

![Connect](/images/5.fwd/55-auto.png)

Similarly, 512 and 1024 are replaced with Memory.
Run the test 5 times for the following results:


**Remarks:**.
Your lambda function is very lightweight (returns almost only JSON).
Increasing Memory from 128 → 512 → 1024 does not make a significant difference in running time.
128MB is cost-effective, because:
Least memory = cheapest price.
Running time is almost the same.


**Create monitoring dashboard**.

![Connect](/images/5.fwd/56-auto.png)

**Monitoring Dashboard**.

![Connect](/images/5.fwd/57-auto.png)

**Successfully created Extension Policy to automatically adjust Provisioned Concurrency**.

![Connect](/images/5.fwd/58-auto.png)

![Connect](/images/5.fwd/59-auto.png)

![Connect](/images/5.fwd/590-auto.png)

![Connect](/images/5.fwd/591-auto.png)
