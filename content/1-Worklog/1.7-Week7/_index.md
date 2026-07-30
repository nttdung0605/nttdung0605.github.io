---
title: "Week 7 Worklog"
date: 2026-06-06
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---


### Week 7 Objectives:

* Build the processing brain of the API.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - Create the SubmitScoreFunction, utilizing the AWS SDK to call the PutItemCommand. | 13/07/2026 | 14/07/2026      | <https://cloudjourney.awsstudygroup.com/> <br> https://www.youtube.com/@AWSStudyGroup |
| 3   | - Create the SubmitScoreFunction using Node.js 20.x, utilizing the AWS SDK to call the PutItemCommand. | 13/07/2026 | 14/07/2026      | <https://cloudjourney.awsstudygroup.com/> <br> https://www.youtube.com/@AWSStudyGroup |
| 4   | - Create the GetLeaderboardFunction, using the QueryCommand to retrieve descending scores.       | 15/07/2026 | 16/07/2026       | <https://cloudjourney.awsstudygroup.com/> <br> https://www.youtube.com/@AWSStudyGroup |
| 5   | - Create the GetLeaderboardFunction, using the QueryCommand to retrieve descending scores.       | 15/07/2026 | 16/07/2026       | <https://cloudjourney.awsstudygroup.com/> <br> https://www.youtube.com/@AWSStudyGroup |
| 6   | - Attach the IAM Role created to both Lambda functions. | 17/07/2026 | 17/07/2026        | <https://cloudjourney.awsstudygroup.com/> <br> https://www.youtube.com/@AWSStudyGroup |


### Week 7 Achievements:

* Created the SubmitScoreFunction and implemented logic to store scores by calling the DynamoDB PutItem API.

* Created the GetLeaderboardFunction and used DynamoDB Query operations to retrieve leaderboard data in descending order.

* Gained practical experience in building Lambda functions that interact directly with DynamoDB.

* Learned how to connect backend logic with data storage services to support application functionality.

* Attached the IAM role to both Lambda functions, enabling secure and authorized access to required AWS resources.