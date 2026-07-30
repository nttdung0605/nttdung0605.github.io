---
title : "Configure Strict Permissions"
date : 2024-01-01
weight : 4
chapter : false
pre : " <b> 5.4. </b> "
---

#### Create a JSON Policy

* Search IAM on search bar then open.

* Access IAM and create a JSON Policy that grants only the minimum required permissions: dynamodb:PutItem, dynamodb:Query, and logs:CreateLogStream.  
![Create DynamoDB Table](/images/5-Workshop/5.4/5-4-1.png)
![Create DynamoDB Table](/images/5-Workshop/5.4/5-4-2.png)

* Set Policy name and create.
![Create DynamoDB Table](/images/5-Workshop/5.4/5-4-3.png)
![Create DynamoDB Table](/images/5-Workshop/5.4/5-4-4.png)

#### Create a new IAM Role
* Create a new IAM Role specifically for AWS Lambda and attach the newly created Policy. This ensures secure interaction with the database without hard-coding access keys.  
* Return to IAM and choose Roles, then choose Create role.
![Create DynamoDB Table](/images/5-Workshop/5.4/5-4-5.png)
* Select AWS Service and choose Lambda.
![Create DynamoDB Table](/images/5-Workshop/5.4/5-4-6.png)
* Add permission we just create above and set Role name and create.
![Create DynamoDB Table](/images/5-Workshop/5.4/5-4-7.png)
![Create DynamoDB Table](/images/5-Workshop/5.4/5-4-8.png)
![Create DynamoDB Table](/images/5-Workshop/5.4/5-4-9.png)
* Add permission AWSLambdaBasicExecutionRole for avoiding errors about CloudWatch Logs.
![Create DynamoDB Table](/images/5-Workshop/5.4/5-4-10.png)


