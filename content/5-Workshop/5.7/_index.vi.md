---
title : "Kiểm thử hệ thống"
date : 2026-06-06
weight : 7
chapter : false
pre : " <b> 5.7. </b> "
---

### Kiểm thử với Lambda
* Truy cập Lambda và chọn SubmitScoreFunction.
* Vào tab Test, tạo test rồi chạy.
![Picture](/images/5-Workshop/5.7/5-7-1.png)
![Picture](/images/5-Workshop/5.7/5-7-2.png)
* Kiểm tra bảng DynamoDB. Chọn Explore items table.
![Picture](/images/5-Workshop/5.7/5-7-3.png)
* Kiểm thử với GetLeaderboardFunction.
![Picture](/images/5-Workshop/5.7/5-7-4.png)

### Kiểm thử với PostMan
* Sử dụng Postman để gửi HTTP POST request tới API URL với JSON body để xác nhận phản hồi HTTP 200.
![Picture](/images/5-Workshop/5.7/5-7-5.png)
* Gửi HTTP GET request để kiểm tra API trả về đúng mảng điểm số từ DynamoDB.
![Picture](/images/5-Workshop/5.7/5-7-6.png)
* Theo dõi execution history và bắt lỗi tiềm ẩn bằng Amazon CloudWatch Logs.
![Picture](/images/5-Workshop/5.7/5-7-7.png)
