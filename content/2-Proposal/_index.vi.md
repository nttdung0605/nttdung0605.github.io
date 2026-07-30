---
title: "Đề xuất dự án"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 2. </b> "
---

Trang này trình bày đề xuất cho dự án Daily Challenge Score API, một hệ thống serverless giúp lưu trữ và hiển thị điểm số cho các thử thách hàng ngày trong chương trình First Cloud AI Journey.

## 1. Tóm tắt điều hành
Dự án nhằm xây dựng một API serverless giúp người dùng có thể gửi điểm số và xem bảng xếp hạng theo thời gian thực. Hệ thống được thiết kế đơn giản, dễ triển khai và có thể mở rộng trong tương lai, đồng thời giúp hiểu rõ hơn về cách các dịch vụ AWS hoạt động cùng nhau trong một kiến trúc serverless.

## 2. Tuyên bố vấn đề
Trong quá trình tham gia chương trình, việc theo dõi kết quả thử thách hàng ngày trở nên khó khăn nếu chỉ dựa trên cách ghi chép thủ công. Cần có một hệ thống cho phép lưu trữ điểm số một cách có tổ chức, đồng thời hỗ trợ truy vấn nhanh và hiển thị bảng xếp hạng rõ ràng. Một giải pháp serverless giúp giảm chi phí vận hành và giảm bớt công việc quản trị hạ tầng.

## 3. Kiến trúc giải pháp
Dự án sử dụng kiến trúc serverless với API Gateway làm cổng truy cập, Lambda xử lý logic nghiệp vụ, DynamoDB lưu trữ dữ liệu và CloudWatch để giám sát. Người dùng có thể gửi dữ liệu qua API POST và lấy bảng xếp hạng qua API GET. Kiến trúc này giúp tập trung vào logic ứng dụng thay vì quản lý server.

![Daily Challenge Score API architecture](public/images/2-Proposal/Architecture.png)

### Các dịch vụ AWS được sử dụng
- Amazon API Gateway: tạo API REST để expose chức năng cho client.
- AWS Lambda: xử lý lưu điểm và truy vấn bảng xếp hạng.
- Amazon DynamoDB: lưu trữ dữ liệu điểm số theo challengeId và score.
- IAM: cung cấp quyền truy cập tối thiểu cho Lambda.
- Amazon CloudWatch: giám sát logs và vận hành.

## 4. Triển khai kỹ thuật
Dự án được triển khai theo từng giai đoạn rõ ràng:
1. Thiết kế dữ liệu và cấu trúc bảng DynamoDB.
2. Xây dựng Lambda để nhận dữ liệu và ghi vào DynamoDB.
3. Xây dựng Lambda để truy vấn leaderboard theo thứ tự giảm dần.
4. Kết nối API Gateway, cấu hình CORS và triển khai API.
5. Kiểm thử bằng Postman và dọn dẹp tài nguyên sau khi hoàn thành.

## 5. Lộ trình và mốc triển khai
- Tuần 1–2: làm quen với AWS và các dịch vụ cơ bản.
- Tuần 3–4: hiểu về database, monitoring và serverless cơ bản.
- Tuần 5–6: xây dựng API Gateway và cấu hình dữ liệu.
- Tuần 7–8: phát triển Lambda, kết nối DynamoDB và triển khai API.
- Tuần 9: hoàn thiện tài liệu, kiểm thử và cleanup tài nguyên.

## 6. Ước tính ngân sách
Dự án được triển khai theo mô hình pay-as-you-go và được dọn dẹp sau khi hoàn thành, giúp giảm chi phí vận hành đáng kể. Với các tài nguyên dùng tạm thời, tổng chi phí phát sinh gần bằng 0 trong hầu hết trường hợp khi không còn chạy dịch vụ.

## 7. Rủi ro và phương án giảm thiểu
- Rủi ro về cấu hình quyền truy cập: giảm thiểu bằng IAM policy theo nguyên tắc least privilege.
- Rủi ro về lỗi logic khi xử lý dữ liệu: giảm thiểu bằng kiểm thử và theo dõi logs trên CloudWatch.
- Rủi ro về phát sinh chi phí: giảm thiểu bằng việc dọn dẹp tài nguyên sau khi hoàn thành.

## 8. Kết quả kỳ vọng
Dự án giúp củng cố hiểu biết về serverless architecture, API Gateway, Lambda và DynamoDB. Ngoài ra, nó cũng tạo nền tảng cho việc phát triển các ứng dụng AWS thực tế trong tương lai.