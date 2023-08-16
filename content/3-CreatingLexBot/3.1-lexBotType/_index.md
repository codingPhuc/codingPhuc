---
title : "Creating Lex bot and custom type"
date : "`r Sys.Date()`"
weight : 1
chapter : false
pre : " <b> 3.1. </b> "
---

#### Creating the bot 
1. Go to [Lex bot console manager ](https://ap-southeast-1.console.aws.amazon.com/lexv2/home?region=ap-southeast-1#welcome)
  + Click on **Create bot from template**
![Connect](/images/3.connect/lex-1-a.png)

2. in amazon lex click on **bot**
![lex1](/images/3.connect/lex-2-a.png)
3. click on ***create bot*** 
![lex2](/images/3.connect/lex-3-a.png)
4. in configure bot setting : 
  + In Creation method click **Create a blank bot**
  + In bot configuration set bot name as **EmployeesBot**
![lex4](/images/3.connect/lex-4-a.png)
  + In IAM role choose to create a role with basic permission 
  + Click no for Children’s Online Privacy Protection Act (COPPA) 
  + Click next
![lex5](/images/3.connect/lex-5-a.png)
5. Add languages to lex bot 
  + In languages choose **english** 
  + In Voice interaction choose **None this is only a text bases application**

![lex6](/images/3.connect/lex-6-a.png)
#### Creating a custom Slot types 

In Amazon Lex, custom slot types are like labels for specific types of information that your bot needs to understand. They help your bot recognize and grab important details from what users say, like dates, names, or places. This makes your bot smarter at understanding and responding accurately.

1. In the intend section tab click on **Slot types**
![lex7](/images/3.connect/lex-7-a.png)
2. click the **Add slot type**
3. click **Add a blank slot type**
![lex7](/images/3.connect/lex-8-a.png)  
4. In **Add blank slot type** : 
  + Add the slot type name as **Jobs** 
  + click **next**
![lex7](/images/3.connect/lex-9-a.png)  
5. now configure the Jobs slot types : 
  + click  **Restrict to slot values** 
  + add **sotfware engineer** as a value 
  + then click **add** 
![lex7](/images/3.connect/lex-10-a.png)  
  + add the value **data engineer** 
  + add the value **data analysis** 
  + then click **Save Slot Type**
![lex7](/images/3.connect/lex-11-a.png)  

now let move on to create the  lex bot configuration 


