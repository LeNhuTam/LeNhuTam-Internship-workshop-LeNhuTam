---
title : "Preparation "
date: 2024-01-01
weight : 2
chapter : false
pre : " <b> 2. </b> "
---

{{% notice info %}}
You need to create an activated AWS account to perform this lab.
{{% /notice %}}

- AWS account activated.
- Install AWS CLI.
    https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html
Or run command in cmd:
    msiexec.exe /i https://awscli.amazonaws.com/AWSCLIV2.msi
Download the installer .msi file for Windows.
  Run the installation.
  After installation, close cmd, reopen cmd.
  Check if AWS CLI has been successfully installed by entering cmd: aws –version
- Created IAM role with permissions for Lambda, API Gateway, CloudWatch.
