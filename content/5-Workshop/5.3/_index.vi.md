---
title : "Khởi tạo cơ sở dữ liệu"
date : 2026-06-06 
weight : 3
chapter : false
pre : " <b> 5.3. </b> "
---

### Tạo bảng DynamoDB
* Truy cập DynamoDB và tạo một bảng mới tên là DailyChallengeScores.

* Cấu hình Partition key là challengeId (String) và Sort key là score (Number).

* Chọn chế độ dung lượng On-demand (cài đặt mặc định) để tối ưu chi phí, chỉ thanh toán cho số lần đọc/ghi thực tế.

![Picture](/images/5-Workshop/5.3/5-3-1.png)

![Create DynamoDB Table Success](/images/5-Workshop/5.3/5-3-2.png)
