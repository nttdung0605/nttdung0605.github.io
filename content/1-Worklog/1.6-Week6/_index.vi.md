---
title: "Tuần 6 - Nhật ký công việc"
date: 2026-06-06
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu của tuần 6:

* Khởi tạo hạ tầng dữ liệu và cấu hình quyền truy cập chặt chẽ.

### Các công việc thực hiện trong tuần:
| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 2 | - Truy cập DynamoDB và tạo bảng DailyChallengeScores. Cấu hình Partition key là challengeId và Sort key là score. Chọn On-demand mode. | 06/07/2026 | 07/07/2026 | <https://cloudjourney.awsstudygroup.com/> <br> https://www.youtube.com/@AWSStudyGroup |
| 3 | - Truy cập DynamoDB và tạo bảng DailyChallengeScores. Cấu hình Partition key là challengeId và Sort key là score. Chọn On-demand mode. | 06/07/2026 | 07/07/2026 | <https://cloudjourney.awsstudygroup.com/> <br> https://www.youtube.com/@AWSStudyGroup |
| 4 | - Tạo IAM Policy chỉ cấp quyền dynamodb:PutItem, dynamodb:Query và logs:CreateLogStream. | 08/07/2026 | 09/07/2026 | <https://cloudjourney.awsstudygroup.com/> <br> https://www.youtube.com/@AWSStudyGroup |
| 5 | - Tạo IAM Policy chỉ cấp quyền dynamodb:PutItem, dynamodb:Query và logs:CreateLogStream. | 08/07/2026 | 09/07/2026 | <https://cloudjourney.awsstudygroup.com/> <br> https://www.youtube.com/@AWSStudyGroup |
| 6 | - Tạo IAM Role cho Lambda và gắn Policy vừa tạo. | 10/07/2026 | 10/07/2026 | <https://cloudjourney.awsstudygroup.com/> <br> https://www.youtube.com/@AWSStudyGroup |

### Thành quả của tuần 6:

* Tạo bảng DynamoDB để lưu trữ điểm số thử thách hàng ngày với các thuộc tính khóa phù hợp và cài đặt dung lượng on-demand.

* Học cách thiết kế cấu trúc lưu trữ dữ liệu đơn giản bằng DynamoDB với partition key và sort key.

* Cấu hình IAM policy theo nguyên tắc least privilege để chỉ cấp các quyền cần thiết cho DynamoDB và logging cho Lambda.

* Tạo và gắn IAM role cho Lambda để truy cập các tài nguyên cần thiết một cách an toàn.

* Củng cố hiểu biết về kiểm soát truy cập an toàn và tầm quan trọng của nguyên tắc least privilege trên AWS.

