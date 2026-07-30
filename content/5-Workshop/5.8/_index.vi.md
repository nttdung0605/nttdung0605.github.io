---
title : "Dọn dẹp tài nguyên"
date : 2024-01-01
weight : 8
chapter : false
pre : " <b> 5.8. </b> "
---

Sau khi hoàn thành workshop, để tránh phát sinh chi phí bất ngờ, hãy xóa REST API trong API Gateway, hai Lambda function, bảng DynamoDB, cùng IAM Role và Policy để giữ môi trường sạch sẽ.

#### Xóa API Gateway
* Mở API Gateway, chọn API và xóa.
![Create DynamoDB Table](/images/5-Workshop/5.8/5-8-1.png)

#### Xóa Lambda Functions
* Mở Lambda, chọn functions và xóa.
![Create DynamoDB Table](/images/5-Workshop/5.8/5-8-2.png)

#### Xóa DynamoDB Table
* Mở DynamoDB, chọn table và xóa.
![Create DynamoDB Table](/images/5-Workshop/5.8/5-8-3.png)

#### Xóa IAM Role và IAM Policy
* Mở IAM, chọn role và xóa.
![Create DynamoDB Table](/images/5-Workshop/5.8/5-8-4.png)
* Sang tab Policy và xóa.
![Create DynamoDB Table](/images/5-Workshop/5.8/5-8-5.png)
