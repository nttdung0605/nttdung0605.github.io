---
title : "Giới thiệu"
date : 2026-06-06 
weight : 1
chapter : false
pre : " <b> 5.1. </b> "
---

#### Công nghệ cốt lõi:
* Hệ thống sử dụng ba dịch vụ quản lý chính: Amazon API Gateway, AWS Lambda và Amazon DynamoDB.
Trong workshop này, bạn sẽ sử dụng hai VPC.

#### Vấn đề cần giải quyết
* Tính năng Daily Challenge thường gặp tình trạng “burst traffic” (tăng đột biến lưu lượng truy cập trong những giờ cụ thể). Việc duy trì một server 24/7 để xử lý lượng truy cập này là không hiệu quả về tài nguyên và tốn kém.

#### Mục tiêu
Mục tiêu là xây dựng một RESTful API hoàn chỉnh có khả năng tự mở rộng để xử lý các đỉnh lưu lượng đột ngột mà không cần cấu hình hoặc quản lý server. Hệ thống được thiết kế để tối đa hóa tiết kiệm chi phí, hướng tới ngân sách $0 bằng cách tận dụng AWS Free Tier, đồng thời đảm bảo thời gian phản hồi API dưới 500ms.
