---
title : "Creating lex bot"
date : "`r Sys.Date()`"
weight : 2
chapter : false
pre : " <b> 3.2. </b> "
---
In this chapter we will be configuring the lex bot to work with our lambda function and add data to our dynamodb databases 

#### Configure lex bot 
1. go to intent tab on lex bot and Click on **NewIntent** that was created when you create the bot 
![lex7](/images/3.connect/lex-12-a.png)  
{{% notice note %}}
If you don't have a intent name NewIntent you  can create one by click on create Intent 
{{% /notice %}} 
2. name the intent as **BotIntent** 
![lex7](/images/3.connect/lex-13-a.png)
3. In the **Sample utterances** :
   + click on **Plain text** 
   + then add the code bellow 
```
register information
my name is {FirstName}  phone number {PhoneNumEmp} and position {job_position}
```
![lex7](/images/3.connect/lex-14-a.png)
4. In **Slots** :
   + click on **Add Slot**
![lex7](/images/3.connect/lex-15-a.png)
   +  Add the name : **PhoneNumEmp**
   +  Add the slot types : **AMAZON.PhoneNumber**
   +  Add the Prompts : **what your phone number ?**
![lex7](/images/3.connect/lex-16-a.png)
   +  do the same for the employees name 
   +  Add the name : **FirstName**
   +  Add the slot types : **AMAZON.FirstName**
   +  Add the Prompts : **tell me your name ?**
![lex7](/images/3.connect/lex-17-a.png)
   +  do the same for the employees job 
   +  Add the name : **FirstName**
   +  Add the slot types : **AMAZON.FirstName**
   +  Add the Prompts : **tell me your name ?**
![lex7](/images/3.connect/lex-18-a.png)
5. in the Confirmation : 
   + click **Active**  
   + fill the Confirmation prompt : **so your name is {FirstName}  , phone number {PhoneNumEmp} and current job postion is {job_position} correct ?**
   + Decline response prompt : **okay we will ask again**
![lex7](/images/3.connect/lex-19-a.png)
   + In Fulfillment click on **Active**
6. finally click on **Use a Lambda function for initialization and validation** then click on **build**
![lex7](/images/3.connect/lex-20-a.png)

7. configure the test : 
   + Click on **test** 
   + Click on the **setting icon** 
   + for the source choose **BotFunction** 
   + then choose **Save** 
![lex7](/images/3.connect/lex-21-a.png)
8. fill in the require information to test out the bot 
![lex7](/images/3.connect/lex-22.PNG)
![lex7](/images/3.connect/lex-23.PNG)
9. then check the databases to see if the Information is register go to [AWS Dynamodbv2](https://console.aws.amazon.com/dynamodbv2/)
10. click on **Explore items** 
![lex7](/images/3.connect/dyanmodb-1-a.png)
11. in **Explore item**  click on **EmployeesDataBases** : 
 ![lex7](/images/3.connect/dyanmodb-2.PNG)
We can see that the information have been log into our databases   
