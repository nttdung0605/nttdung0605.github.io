---
title : "Kiểm thử hệ thống"
date : 2024-01-01
weight : 7
chapter : false
pre : " <b> 5.7. </b> "
---

### Kiểm thử với Lambda
* Truy cập Lambda và chọn SubmitScoreFunction.
* Vào tab Test, tạo test rồi chạy.
![Create DynamoDB Table](/images/5-Workshop/5.7/5-7-1.png)
![Create DynamoDB Table](/images/5-Workshop/5.7/5-7-2.png)
* Kiểm tra bảng DynamoDB. Chọn Explore items table.
![Create DynamoDB Table](/images/5-Workshop/5.7/5-7-3.png)
* Kiểm thử với GetLeaderboardFunction.
![Create DynamoDB Table](/images/5-Workshop/5.7/5-7-4.png)

### Kiểm thử với PostMan
* Sử dụng Postman để gửi HTTP POST request tới API URL với JSON body để xác nhận phản hồi HTTP 200.
![Create DynamoDB Table](/images/5-Workshop/5.7/5-7-5.png)
* Gửi HTTP GET request để kiểm tra API trả về đúng mảng điểm số từ DynamoDB.
![Create DynamoDB Table](/images/5-Workshop/5.7/5-7-6.png)
* Theo dõi execution history và bắt lỗi tiềm ẩn bằng Amazon CloudWatch Logs.
![Create DynamoDB Table](/images/5-Workshop/5.7/5-7-7.png)
