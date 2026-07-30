---
title : "Cấu hình quyền truy cập chặt chẽ"
date : 2024-01-01 
weight : 4 
chapter : false
pre : " <b> 5.4. </b> "
---

#### Tạo JSON Policy

* Mở IAM bằng cách tìm kiếm trên thanh tìm kiếm.

* Truy cập IAM và tạo một JSON Policy chỉ cấp các quyền tối thiểu cần thiết: dynamodb:PutItem, dynamodb:Query và logs:CreateLogStream.
![Create DynamoDB Table](/images/5-Workshop/5.4/5-4-1.png)
![Create DynamoDB Table](/images/5-Workshop/5.4/5-4-2.png)

* Đặt tên Policy và tạo.
![Create DynamoDB Table](/images/5-Workshop/5.4/5-4-3.png)
![Create DynamoDB Table](/images/5-Workshop/5.4/5-4-4.png)

#### Tạo IAM Role mới
* Tạo một IAM Role mới dành riêng cho AWS Lambda và gắn Policy vừa tạo. Điều này giúp tương tác an toàn với cơ sở dữ liệu mà không cần hard-code access keys.
* Quay lại IAM và chọn Roles, sau đó chọn Create role.
![Create DynamoDB Table](/images/5-Workshop/5.4/5-4-5.png)
* Chọn AWS Service và chọn Lambda.
![Create DynamoDB Table](/images/5-Workshop/5.4/5-4-6.png)
* Thêm permission vừa tạo ở trên và đặt tên Role rồi tạo.
![Create DynamoDB Table](/images/5-Workshop/5.4/5-4-7.png)
![Create DynamoDB Table](/images/5-Workshop/5.4/5-4-8.png)
![Create DynamoDB Table](/images/5-Workshop/5.4/5-4-9.png)
* Thêm permission AWSLambdaBasicExecutionRole để tránh lỗi liên quan đến CloudWatch Logs.
![Create DynamoDB Table](/images/5-Workshop/5.4/5-4-10.png)

