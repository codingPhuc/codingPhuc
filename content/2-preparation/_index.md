---
title : "preparation"
date : "`r Sys.Date()`"
weight : 2
chapter : false
pre : " <b> 2. </b> "
---

{{% notice info %}}
you need to create dynamodb and lambda function to proceed with this lab 
{{% /notice %}}

To learn how to create dynamodb and lambda function ,  you can refer to these lab:
  - [About dynamodb](https://amazon-dynamodb-labs.com/)
  - [work with Lambda](https://aws.amazon.com/lambda/resources/workshops-and-tutorials/)

In order for Lambda function to work with dynamodb we need to create our own IAM role to gain permission 

### Content
  - [Create Dynamodb](2.1-PreparingDynamodb/)
  - [Create IAM Role](2.2-CreatingIAMRoles/)
  - [Create Lambda function](2.3-CreatingLambdaFunction/)