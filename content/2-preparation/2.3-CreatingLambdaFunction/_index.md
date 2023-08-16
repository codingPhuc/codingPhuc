---
title : "Create Lambda Function"
date : "`r Sys.Date()`"
weight : 3
chapter : false
pre : " <b> 2.3 </b> "
---

In this step we will learn how to create a Lambda function to work with our DynamoDb and be the logic that operate our lex bot

The architecture overview after you complete this step will be as follows:

1. Go to [Lambda Service Interface](https://console.aws.amazon.com/lambda/)
2. click on **create a function** 
![lambda-1](/images/2.prerequisite/Lambda-1-a.png)
3. in the create function page 
  + set the Function name to **BotFunction**
  + set the Runtime to **Python 3.11**
  + choose the Architecture  to be **x86_64**
  + change the default execution role to **Used an existing role**
  + in the existing role choose the **BotRoles** that we have created 
  + then click **Create Function**
![lambda-2](/images/2.prerequisite/Lambda-2-a.png)
4. in the BotFunction click on **configuration** 
![lambda-3](/images/2.prerequisite/Lambda-3-a.png)
5. on the configuration tab : 
  + click on **Environment variables**
  + then click on **Edit**
![lambda-4](/images/2.prerequisite/Lambda-4-a.png)
6. on the edit tab click on **Add Environment variables**
![lambda-5](/images/2.prerequisite/Lambda-5-a.png)
7. edit the key and value to connect the databases with the Lambda function : 
  + for the environment add key **TABLE_NAME**
  + for the value add **EmployeesDataBases**
  + then click **save**
![lambda-7](/images/2.prerequisite/Lambda-6-a.png)
8. get the code for Lambda Function : 
  + go to this github link [GITHUB](https://github.com/codingPhuc/LambdaBotCode/blob/main/Lambdacode.py)
  + then click ctrl + A to copy all the code 
![lambda-7](/images/2.prerequisite/Lambda-7.PNG) 
  + Paste the code into the code tab in **BotFunction**
  + then click **Deploy**
![lambda-7](/images/2.prerequisite/Lambda-8-a.png) 

Now we are done with the preparation for lex bot databases and logic now we will move on to configuring the lex bot 

