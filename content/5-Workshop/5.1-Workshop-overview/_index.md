---
title : "Introduction"
date : 2026-06-06 
weight : 1 
chapter : false
pre : " <b> 5.1. </b> "
---

#### Core Technologies: 
* The system utilizes three core managed services: Amazon API Gateway, AWS Lambda, and Amazon DynamoDB.
In this workshop, you will use two VPCs. 

#### Problem Statement
* Daily challenge features typically experience "burst traffic" (sudden spikes in user access during specific hours). Maintaining a traditional 24/7 server to handle this is resource-inefficient and costly.

#### Objective
The goal is to build a complete RESTful API capable of auto-scaling to handle sudden traffic spikes without the need to configure or manage servers. The system is designed to maximize cost savings, aiming for a budget of $0 by utilizing the AWS Free Tier , while ensuring API response times remain under 500ms.