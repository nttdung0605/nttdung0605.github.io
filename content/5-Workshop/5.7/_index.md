---
title : "System Testing"
date : 2026-06-06
weight : 7
chapter : false
pre : " <b> 5.7. </b> "
---

### Test with Lambda
* Go to Lambda and choose SubmitScoreFunction.
* Go to test tab and create test then run test.
![Picture](/images/5-Workshop/5.7/5-7-1.png) 
![Picture](/images/5-Workshop/5.7/5-7-2.png) 
* Go check DynamoDB table. Choose explore items table.
![Picture](/images/5-Workshop/5.7/5-7-3.png) 
* Go test with GetLeaderboardFunction.
![Picture](/images/5-Workshop/5.7/5-7-4.png) 


### Test with PostMan
* Use Postman to send an HTTP POST request to the API URL with a JSON body to verify that an HTTP 200 response is returned. 
![Picture](/images/5-Workshop/5.7/5-7-5.png)
* Send an HTTP GET request to verify that the API accurately returns the array of scores from DynamoDB.  
![Picture](/images/5-Workshop/5.7/5-7-6.png)
* Monitor the execution history and catch any potential errors using Amazon CloudWatch Logs. 
![Picture](/images/5-Workshop/5.7/5-7-7.png) 