---
title : "Twillio"
date : "`r Sys.Date()`"
weight : 4
chapter : false
pre : " <b> 4. </b> "
---








In this chapter we will configure twilio to work with our Amazon lex bot







![twilio](/images/arc-001.png)
#### creating a twillio account 
Open twilio with the following link  [TWILLIO](https://www.twilio.com/en-us)
1. click on login then follow the instruction to login into your account 
![twilio](/images/4.s3/twillio-1-a.png)
2. choose the most importance part in the TWILLIO configuration : 
 + choose **SMS** as used 
 + in the **How do you want to build with twillio** choose **with minimum code**
 + then click **get started** 
![twilio](/images/4.s3/twillio-2-a.png)
3. in twillio home screen choose get phone number 
![twilio](/images/4.s3/twillio-3-a.png)
4. click  on your twillio account 
 ![twilio](/images/4.s3/twillio-7-a.png)  
5. get the Account SID and Auth Token to used with lex bot
![twilio](/images/4.s3/twillio-8-a.png)
#### building lex bot to work with twillio
1. on bot version click create version 
![twilio](/images/4.s3/twillio-9-a.png)

2. click on **Create version**
![twilio](/images/4.s3/twillio-10-a.PNG)

3. on channel integration  click **Add channel**
![twilio](/images/4.s3/twillio-14-a.png) 

4. on the channel integration creation form : 
+ click on twillio 
![twilio](/images/4.s3/twillio-15-a.png) 
+ name the bot **twillio bot** 
+ choose **TestBotAlias** 
+ choose language as **English** 
+ then add the account id  and authentication key in your twillio account 
![twilio](/images/4.s3/twillio-16-a.png)
5 when created successfully copy the url of the channel 
![twilio](/images/4.s3/twillio-17.PNG)
#### calling whatapp using twillio
1. testing the whatapp messaging 
 + In  twillio click on **Messaging** 
 + click on **Send a  WhatApp Message** 
![twilio](/images/4.s3/twillio-4-a.png) 
2. In whatapp try to send a message to whatapp twillio will give you the phone number and join  code copy them: 
![twilio](/images/4.s3/twillio-5-a.png)
3. find the twillio number on whatapp then enter paste the code to used twillio 
![twilio](/images/4.s3/twillio-6-a.png)  
4. In the whatapp sand bot setting copy the lex bot url into the post 
5. then hit save 
![twilio](/images/4.s3/twillio-18-a.png)
6. now you can talk to your lex bot thought whatapp using twillio 
![twilio](/images/4.s3/twillio-19.PNG)

