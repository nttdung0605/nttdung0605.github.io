---
title: "Proposal"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 2. </b> "
---


# Serverless Daily Challenge Score API
## A Basic AWS Serverless Backend for Real-Time Scoring and Leaderboards

### 1. Executive Summary
This project proposes a basic serverless backend on AWS for a daily challenge application that stores and retrieves user scores. The solution uses Amazon API Gateway, AWS Lambda, and Amazon DynamoDB to provide a RESTful API for score submission and leaderboard retrieval. It is designed to handle burst traffic efficiently while keeping infrastructure costs low.

### 2. Problem Statement
#### What’s the Problem?
Daily challenge applications often experience sudden spikes in traffic during specific hours and very low traffic at other times. Maintaining a traditional 24/7 server-based architecture would waste resources and increase operating costs. In addition, the development team wants to focus on UI/UX design and user experience rather than spending time managing servers and network infrastructure.

#### The Solution
The proposed solution uses a fully serverless architecture. Client requests are sent via HTTP to Amazon API Gateway, which invokes AWS Lambda functions to process business logic. Lambda then stores or retrieves data in Amazon DynamoDB. The system provides two core endpoints:
- POST /score: Submit a user score
- GET /leaderboard: Retrieve the top 10 highest scores

This architecture is lightweight, cost-effective, and automatically scales based on demand.

### 3. Solution Architecture
The architecture follows an event-driven model:

Client (Mobile/Web) → Amazon API Gateway → AWS Lambda → Amazon DynamoDB

Lambda also sends logs to Amazon CloudWatch for monitoring and troubleshooting.

![Daily Challenge Score API architecture](public/images/2-Proposal/Architecture.png)

#### AWS Services Used
- **Amazon API Gateway**: Exposes secure RESTful API endpoints.
- **AWS Lambda**: Executes business logic in Node.js or Python.
- **Amazon DynamoDB**: Stores score records and supports fast read/write operations.
- **Amazon CloudWatch**: Collects logs and metrics for monitoring.

### 4. Technical Implementation
The implementation is designed as a simple serverless backend with one database table and two API routes.

#### Core Components
- **API Layer**: Amazon API Gateway exposes public endpoints for score submission and leaderboard retrieval.
- **Business Logic**: AWS Lambda performs validation and handles score processing.
- **Data Layer**: Amazon DynamoDB stores user scores in a single table named DailyChallengeScores.
- **Monitoring**: CloudWatch Logs capture errors and latency, while alarms can be configured for API failures.

#### Security and IAM
- Lambda uses an execution role with least-privilege permissions.
- The role is granted only the necessary permissions: dynamodb:PutItem and dynamodb:Query.
- DynamoDB is not exposed publicly and is accessed only through Lambda via AWS IAM.

### 5. Timeline & Milestones
- **Week 1**: Define project requirements, API endpoints, and the overall serverless architecture.
- **Week 2**: Set up the AWS environment, create the Lambda function, and configure API Gateway.
- **Week 3**: Design and create the DynamoDB table, then connect it to the Lambda function.
- **Week 4**: Implement API testing, security configuration, and basic monitoring with CloudWatch.
- **Week 5**: Deploy the solution, validate endpoint behavior, and finalize documentation and reporting.

### 6. Budget Estimation
The system is expected to use AWS Free Tier as the primary cost model:
- **AWS Lambda**: 1 million requests per month free
- **Amazon DynamoDB**: 25 GB storage free
- **API Gateway**: 1 million API calls per month free

Estimated monthly cost: **$0**

### 7. Risk Assessment
#### Risks
- CORS misconfiguration on API Gateway may prevent the frontend from calling the API.
- Missing IAM permissions may block Lambda from writing to DynamoDB and result in AccessDenied errors.

#### Mitigation Strategies
- Configure CORS properly on API Gateway.
- Assign least-privilege IAM permissions to the Lambda execution role.
- Test integration thoroughly before deployment.

### 8. Expected Outcomes
The project will deliver a lightweight, scalable, and low-cost backend for daily challenge applications. It will enable real-time score submission and leaderboard retrieval while allowing the development team to focus on frontend experience and product design.