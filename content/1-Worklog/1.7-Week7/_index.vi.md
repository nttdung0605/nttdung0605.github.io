---
title: "Tuần 7 - Nhật ký công việc"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu của tuần 7:

* Xây dựng "bộ não" xử lý của API.

### Các công việc thực hiện trong tuần:
| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 2 | - Tạo SubmitScoreFunction, sử dụng AWS SDK để gọi PutItemCommand. | 13/07/2026 | 14/07/2026 | <https://cloudjourney.awsstudygroup.com/> <br> https://www.youtube.com/@AWSStudyGroup |
| 3 | - Tạo SubmitScoreFunction bằng Node.js 20.x, sử dụng AWS SDK để gọi PutItemCommand. | 13/07/2026 | 14/07/2026 | <https://cloudjourney.awsstudygroup.com/> <br> https://www.youtube.com/@AWSStudyGroup |
| 4 | - Tạo GetLeaderboardFunction, dùng QueryCommand để lấy dữ liệu điểm số theo thứ tự giảm dần. | 15/07/2026 | 16/07/2026 | <https://cloudjourney.awsstudygroup.com/> <br> https://www.youtube.com/@AWSStudyGroup |
| 5 | - Tạo GetLeaderboardFunction, dùng QueryCommand để lấy dữ liệu điểm số theo thứ tự giảm dần. | 15/07/2026 | 16/07/2026 | <https://cloudjourney.awsstudygroup.com/> <br> https://www.youtube.com/@AWSStudyGroup |
| 6 | - Gắn IAM Role đã tạo cho cả hai Lambda function. | 17/07/2026 | 17/07/2026 | <https://cloudjourney.awsstudygroup.com/> <br> https://www.youtube.com/@AWSStudyGroup |

### Thành quả của tuần 7:

* Tạo SubmitScoreFunction và triển khai logic để lưu điểm bằng cách gọi API DynamoDB PutItem.

* Tạo GetLeaderboardFunction và sử dụng các thao tác DynamoDB Query để lấy dữ liệu leaderboard theo thứ tự giảm dần.

* Có kinh nghiệm thực tế trong việc xây dựng Lambda function tương tác trực tiếp với DynamoDB.

* Học cách kết nối logic backend với dịch vụ lưu trữ dữ liệu để hỗ trợ chức năng ứng dụng.

* Gắn IAM role cho cả hai Lambda function, cho phép truy cập AWS một cách an toàn và có quyền hạn phù hợp.

