---
title: "Tuần 8 - Nhật ký công việc"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.8. </b> "
---


### Mục tiêu của tuần 8:

* Đưa API lên chạy và mô phỏng lưu lượng truy cập.

### Các công việc thực hiện trong tuần:
| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 2 | - Tạo REST API tên ChallengeLeaderboardAPI và tạo resource /scores. | 20/07/2026 | 21/07/2026 | <https://cloudjourney.awsstudygroup.com/> <br> https://www.youtube.com/@AWSStudyGroup |
| 3 | - Tạo REST API tên ChallengeLeaderboardAPI và tạo resource /scores. | 20/07/2026 | 21/07/2026 | <https://cloudjourney.awsstudygroup.com/> <br> https://www.youtube.com/@AWSStudyGroup |
| 4 | - Cấu hình method POST trỏ tới SubmitScoreFunction và method GET trỏ tới GetLeaderboardFunction. | 22/07/2026 | 22/07/2026 | <https://cloudjourney.awsstudygroup.com/> <br> https://www.youtube.com/@AWSStudyGroup |
| 5 | - Cấu hình CORS và deploy API lên dev stage để lấy URL. | 23/07/2026 | 23/07/2026 | <https://cloudjourney.awsstudygroup.com/> <br> https://www.youtube.com/@AWSStudyGroup |
| 6 | - Dùng Postman để gửi request POST/GET nhằm kiểm thử thực tế. | 24/07/2026 | 24/07/2026 | <https://cloudjourney.awsstudygroup.com/> <br> https://www.youtube.com/@AWSStudyGroup |

### Thành quả của tuần 8:

* Tạo REST API tên ChallengeLeaderboardAPI và thiết lập resource /scores để xử lý các request leaderboard.

* Cấu hình API Gateway để POST request chuyển tới Lambda submit và GET request chuyển tới Lambda leaderboard.

* Bật CORS và deploy API lên dev stage, làm cho API có thể truy cập qua endpoint live.

* Kiểm thử API bằng Postman bằng cách gửi request POST và GET thực tế, xác nhận chức năng end-to-end.

* Có kinh nghiệm thực tế trong việc expose services backend serverless qua API công khai.

