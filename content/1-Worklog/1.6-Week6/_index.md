---
title: "Week 6 Worklog"
date: 2026-06-06
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---


### Week 6 Objectives:

* Initialize the data infrastructure and configure strict permissions.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - Access DynamoDB and create the DailyChallengeScores table. Configure the Partition key as challengeId and the Sort key as score. Select On-demand mode. | 06/07/2026 | 07/07/2026      | <https://cloudjourney.awsstudygroup.com/> <br> https://www.youtube.com/@AWSStudyGroup |
| 3   | - Access DynamoDB and create the DailyChallengeScores table. Configure the Partition key as challengeId and the Sort key as score. Select On-demand mode. | 06/07/2026 | 07/07/2026      | <https://cloudjourney.awsstudygroup.com/> <br> https://www.youtube.com/@AWSStudyGroup |
| 4   | - Create an IAM Policy that only grants dynamodb:PutItem, dynamodb:Query, and logs:CreateLogStream permissions.        | 08/07/2026 | 09/07/2026       | <https://cloudjourney.awsstudygroup.com/> <br> https://www.youtube.com/@AWSStudyGroup |
| 5   | - Create an IAM Policy that only grants dynamodb:PutItem, dynamodb:Query, and logs:CreateLogStream permissions.        | 08/07/2026 | 09/07/2026       | <https://cloudjourney.awsstudygroup.com/> <br> https://www.youtube.com/@AWSStudyGroup |
| 6   | - Create an IAM Role for Lambda and attach the newly created Policy. | 10/07/2026 | 10/07/2026        | <https://cloudjourney.awsstudygroup.com/> <br> https://www.youtube.com/@AWSStudyGroup |


### Week 6 Achievements:

* Created the DynamoDB table for storing daily challenge scores with appropriate key attributes and on-demand capacity settings.

* Learned how to design a simple data storage structure using DynamoDB with a partition key and sort key.

* Configured a least-privilege IAM policy to allow only the necessary DynamoDB and logging permissions for Lambda.

* Created and attached an IAM role for Lambda to securely access the required resources.

* Strengthened understanding of secure access control and the importance of applying the principle of least privilege in AWS.