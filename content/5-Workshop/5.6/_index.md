---
title : "Set Up Amazon API Gateway"
date : 2026-06-06
weight : 6
chapter : false
pre : " <b> 5.6. </b> "
---

#### Create a new REST API
* Search api on search bar and choose API Gateway.
* Choose Create API and create REST API
![Picture](/images/5-Workshop/5.6/5-6-1.png) 
* Add API name, choose Reginal and Create.
![Picture](/images/5-Workshop/5.6/5-6-2.png) 
* After create API, on the left bar choose create resource.
![Picture](/images/5-Workshop/5.6/5-6-3.png) 
* Add resource name and create.
![Picture](/images/5-Workshop/5.6/5-6-4.png) 

#### Configure POST and GET method
* Choose resource we just create and create method
![Picture](/images/5-Workshop/5.6/5-6-5.png) 
* Create POST method
![Picture](/images/5-Workshop/5.6/5-6-6.png) 
* Do the same with GET method using Lambda GetLeaderboardFunction.

#### Enable CORS
* Return to resource and enable CORS.
![Picture](/images/5-Workshop/5.6/5-6-7.png) 
![Picture](/images/5-Workshop/5.6/5-6-8.png) 

#### Deploy the API to a stage
* Return to resource and choose Deploy API.
![Picture](/images/5-Workshop/5.6/5-6-9.png) 
* After deploy, get Invoke Url for later use.
![Picture](/images/5-Workshop/5.6/5-6-10.png) 