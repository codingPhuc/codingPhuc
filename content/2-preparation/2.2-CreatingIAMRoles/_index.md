---
title : "Create IAM Role"
date : "`r Sys.Date()`"
weight : 2
chapter : false
pre : " <b> 2.2 </b> "
---

### Create IAM Role

In this step, we will proceed to create IAM Role. In this IAM Role, the policy **AmazonDynamoDBFullAccess** and **CloudWatchFullAccess** will be assigned, this is the policy that allows the Lambda function to interact with  DynamoDB databases.

1. Go to [IAM service administration interface](https://console.aws.amazon.com/iamv2/)
2. In the left navigation bar, click **Roles**.

![role](/images/2.prerequisite/IAM-1-a.PNG)

3. Click **Create role**.

![role1](/images/2.prerequisite/IAM-2-a.png)

4. on **Select trusted entity** 
  + Click **AWS service**.
  + Click **Lambda**
  + Click **Next**

![role1](/images/2.prerequisite/IAM-3-a.png)

1. In the Search box, enter **AmazonDynamoDBFullAccess** and press Enter to search for this policy.
  + Click the policy **AmazonDynamoDBFullAccess**.
![createpolicy1](/images/2.prerequisite/IAM-4-a.png)
2. In the Search box, enter **CloudWatchFullAccess** and press Enter to search for this policy.
  + Click the policy **CloudWatchFullAccess**
  + then click **Next**
![createpolicy](/images/2.prerequisite/IAM-5-a.png)

1. Click **Next: Review**.
2. Name the Role **BotRoles** in Role Name
![createpolicy](/images/2.prerequisite/IAM-6-a.png)
check again if the roles are correct  
Click **Create Role** 
![createpolicy](/images/2.prerequisite/IAM-7-a.png)

Next, we will configure the role to Lambda so it can be able to call the databases.