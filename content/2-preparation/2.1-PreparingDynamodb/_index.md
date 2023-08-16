---
title : "Create Dynamodb"
date : "`r Sys.Date()`"
weight : 1
chapter : false
pre : " <b> 2.1 </b> "
---

In this step we will learn how to create a Dynamodb databases  
The following step will help you create a Dynamodb databases with the right configuration :

<!-- To learn how to create EC2 instances and VPCs with public/private subnets, you can refer to the lab:
  - [About Amazon EC2](https://000004.awsstudygroup.com/en/)
  - [Works with Amazon VPC](https://000003.awsstudygroup.com/en/)
![dynamodb](/images/2.prerequisite/dynamodb-5-a.png) -->

#### Creating  a Dynamodb databases **EmployeesDataBases**
first go to your [AWS console](https://console.aws.amazon.com):
 + click on the search bar and type **dynamoDB**
 + click on **dynamoDB**
![dynamodb-1](/images/2.prerequisite/dynamodb-1-a.png)

on Dynamodb click on **create table**
![dynamodb-2](/images/2.prerequisite/dynamodb-2-a.png)

on the Dynamodb creation form : 
  + fill in the table name as **EmployeesDataBases**
  + Partition key as **PhoneNumEmp**
  + and leave the sort key  empty
![dynamodb-3](/images/2.prerequisite/dynamodb-3-a.png)
  + on the table setting click **Customize Setting**
  + on the table class click **Dynamodb standard**
  + on the read/write capacity click on **On-demand**
{{% notice warning %}}
we need to click on demand because we do not know the amount of time we write to the databases, but this is not recommend because it will cause us to lose a money if there is many people calling the application  
{{% /notice %}}
![dynamodb-4](/images/2.prerequisite/dynamodb-4-a.png)
  + on the last step click on create table 
![dynamodb-5](/images/2.prerequisite/dynamodb-5-a.png)
check if the table have been created this usually take 1 minute : 
![dynamodb-6](/images/2.prerequisite/dynamodb-6-a.png)
if the table status = active congratulation you have successfully created the dynamodb databases for employees  

  <!-- - [Create VPC](2.1.1-createvpc/)
  - [Create Public Subnet](2.1.2-createpublicsubnet/)
  - [Create Private Subnet](2.1.3-createprivatesubnet/)
  - [Create security group](2.1.4-createsecgroup/)
  - [Create public Linux server](2.1.5-createec2linux/)
  - [Create private Windows server](2.1.6-createec2windows/) -->


