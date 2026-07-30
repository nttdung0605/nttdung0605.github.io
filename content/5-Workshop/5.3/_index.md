---
title : "Initialize the Database"
date : 2026-06-06
weight : 3
chapter : false
pre : " <b> 5.3. </b> "
---

### Create DynamoDB Table
* Access DynamoDB and create a new table named DailyChallengeScores.  

* Configure the Partition key as challengeId (String) and the Sort key as score (Number).

* Select the On-demand capacity mode (Default settings) to optimize costs, paying only for actual read/write operations.

![Picture](/images/5-Workshop/5.3/5-3-1.png)

![Create DynamoDB Table Success](/images/5-Workshop/5.3/5-3-2.png)