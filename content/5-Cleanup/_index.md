---
title : "Clean up"
date :  "`r Sys.Date()`" 
weight : 5 
chapter : false
pre : " <b> 5. </b> "
---

In this chapter we will clean Up all the resource that we have been using 

### clean up the Dynamodb databases 
1. go to Dynamodb console [Dynamodb](https://ap-southeast-1.console.aws.amazon.com/dynamodbv2/home?region=ap-southeast-1#tables) 
2. click  on **EmployeesDatabases**
3. click on **delete** 
![dynamodb-1](/images/6.clean/clean-1-a.png)
4. a delete confirmation form will show up : 
+ fill in confirm 
+ then click **delete**
![dynamodb-1](/images/6.clean/clean-2-a.png)
### clean up the Lambda function 
1. Go to [Lambda Service Interface](https://console.aws.amazon.com/lambda/)
2. click on **BotFunction** 
3. click on **delete**
![dynamodb-1](/images/6.clean/clean-3-a.png)
4. a delete confirmation form will show up : 
+ fill in delete
+ then click **delete**
![dynamodb-1](/images/6.clean/clean-4-a.png)
### clean up the lex bot 
1. go to lex bot console [lex bot](https://ap-southeast-1.console.aws.amazon.com/lexv2/home?region=ap-southeast-1#bots)
2. click **delete** delete the lex bot 
![dynamodb-1](/images/6.clean/clean-5-a.png)