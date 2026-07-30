---
title : "Viết logic nghiệp vụ"
date : 2024-01-01
weight : 5
chapter : false
pre : " <b> 5.5. </b> "
---

### Tạo hai Lambda functions:
#### Tạo SubmitScoreFunction
* Tìm Lambda trên thanh tìm kiếm và truy cập. Nhấn Create Function.
* Chọn author from scratch.
* Đặt tên Function và chọn runtime Node.js 24.x.
![Create DynamoDB Table](/images/5-Workshop/5.5/5-5-1.png)
* Ở phần Additional settings, thêm permission vừa tạo ở bước trước cho function và lưu.
![Create DynamoDB Table](/images/5-Workshop/5.5/5-5-2.png)
* Nhấn Create function.
* Tải xuống file leaderboard-api.zip từ: https://github.com/nttdung0605/Workshop-funcs
* Chọn function và cập nhật code từ file .zip.
![Create DynamoDB Table](/images/5-Workshop/5.5/5-5-4.png)

#### Tạo GetLeaderboardFunction
* Tải xuống file leaderboard-get.zip từ: https://github.com/nttdung0605/Workshop-funcs
* Lặp lại tương tự như SubmitScoreFunction.

#### Kết quả:
![Create DynamoDB Table](/images/5-Workshop/5.5/5-5-3.png)
