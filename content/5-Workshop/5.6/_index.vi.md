---
title : "Thiết lập Amazon API Gateway"
date : 2024-01-01
weight : 6
chapter : false
pre : " <b> 5.6. </b> "
---

#### Tạo REST API mới
* Tìm kiếm api trên thanh tìm kiếm và chọn API Gateway.
* Chọn Create API và tạo REST API.
![Create DynamoDB Table](/images/5-Workshop/5.6/5-6-1.png)
* Thêm API name, chọn Reginal và Create.
![Create DynamoDB Table](/images/5-Workshop/5.6/5-6-2.png)
* Sau khi tạo API, ở thanh trái chọn create resource.
![Create DynamoDB Table](/images/5-Workshop/5.6/5-6-3.png)
* Thêm resource name và tạo.
![Create DynamoDB Table](/images/5-Workshop/5.6/5-6-4.png)

#### Cấu hình method POST và GET
* Chọn resource vừa tạo và create method.
![Create DynamoDB Table](/images/5-Workshop/5.6/5-6-5.png)
* Tạo POST method.
![Create DynamoDB Table](/images/5-Workshop/5.6/5-6-6.png)
* Làm tương tự với GET method sử dụng Lambda GetLeaderboardFunction.

#### Bật CORS
* Quay lại resource và bật CORS.
![Create DynamoDB Table](/images/5-Workshop/5.6/5-6-7.png)
![Create DynamoDB Table](/images/5-Workshop/5.6/5-6-8.png)

#### Deploy API lên stage
* Quay lại resource và chọn Deploy API.
![Create DynamoDB Table](/images/5-Workshop/5.6/5-6-9.png)
* Sau khi deploy, lấy Invoke Url để dùng sau.
![Create DynamoDB Table](/images/5-Workshop/5.6/5-6-10.png)
