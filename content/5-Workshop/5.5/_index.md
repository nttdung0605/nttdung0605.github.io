---
title : "Write Business Logic"
date : 2024-01-01
weight : 5
chapter : false
pre : " <b> 5.5. </b> "
---

### Create two Lambda functions:
#### Create SubmitScoreFunction
* Search Lambda on search bar and enter. Press Create Function.
* Choose author from sracth.
* Set Funciton name and choose runtime Node.js 24.x
![Create DynamoDB Table](/images/5-Workshop/5.5/5-5-1.png)
* At Additional settings add permissions we create at last step for functiion and save.
![Create DynamoDB Table](/images/5-Workshop/5.5/5-5-2.png)
* Hit Craete function.
* Download leaderboard-api.zip from: https://github.com/nttdung0605/Workshop-funcs
* Choose function andd update code from a .zip file. 
![Create DynamoDB Table](/images/5-Workshop/5.5/5-5-4.png)

#### Create GetLeaderboardFunction
* Download leaderboard-get.zip from: https://github.com/nttdung0605/Workshop-funcs
* Repeat the same like SubmitScoreFunction.

#### Result:
![Create DynamoDB Table](/images/5-Workshop/5.5/5-5-3.png)