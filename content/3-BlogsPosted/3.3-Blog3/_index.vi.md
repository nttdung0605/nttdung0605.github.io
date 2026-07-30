---
title: "Blog 3"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 3.3. </b> "
---


# Building a Scalable User Search Layer on Top of Amazon Cognito

Ý tưởng chính của bài viết là giải thích cách xây dựng một lớp tìm kiếm người dùng có khả năng mở rộng trên nền tảng Amazon Cognito. Bài viết tập trung vào việc giải quyết thách thức tìm kiếm người dùng hiệu quả khi ứng dụng phát triển và các khả năng mặc định của Cognito không còn đủ cho các yêu cầu tra cứu nâng cao.

## Ý chính

Amazon Cognito là một dịch vụ xác thực mạnh mẽ, nhưng nó không cung cấp sẵn trải nghiệm tìm kiếm người dùng linh hoạt và mở rộng như nhiều ứng dụng cần. Bài viết cho thấy cách tiếp cận tốt hơn là xây dựng một lớp tìm kiếm bổ sung chạy song song với Cognito để ứng dụng có thể tra cứu người dùng hiệu quả hơn trong khi vẫn giữ hệ thống xác thực ổn định.

## Các vấn đề được nhấn mạnh

- Amazon Cognito có thể xử lý xác thực tốt, nhưng việc tìm kiếm người dùng ở quy mô lớn có thể gặp khó khăn.
- Các yêu cầu tra cứu đơn giản có thể đủ ở giai đoạn đầu, nhưng ứng dụng phát triển thường cần tìm kiếm nhanh và linh hoạt hơn.
- Chỉ dựa vào các tính năng gốc của Cognito có thể không đủ cho các kịch bản tìm kiếm nâng cao.
- Ứng dụng thường cần một cách để tìm kiếm người dùng hiệu quả mà không làm ảnh hưởng đến bảo mật hoặc hiệu năng.

## Cách tiếp cận giải pháp

Giải pháp đề xuất là xây dựng một lớp tìm kiếm chuyên biệt trên nền Cognito. Lớp này có thể sử dụng thêm các dịch vụ và mẫu kiến trúc để hỗ trợ các thao tác tìm kiếm mở rộng trong khi vẫn giữ hệ thống xác thực nguyên bản. Mục tiêu là cải thiện khả năng khám phá người dùng và trải nghiệm sử dụng mà không thay thế các chức năng xác thực cốt lõi của Cognito.

![overview](/images/3-Blogs/blog3.png)

## Điều em học được

Từ bài viết này, em có thể học được:

- hiểu được giới hạn của Amazon Cognito trong các tình huống tìm kiếm người dùng
- thiết kế các lớp kiến trúc bổ sung để tăng khả năng mở rộng và trải nghiệm người dùng
- hiểu sâu hơn về xác thực, mô hình tìm kiếm và thiết kế ứng dụng trên cloud
- suy nghĩ về cách kết hợp nhiều dịch vụ AWS để giải quyết nhu cầu thực tế của ứng dụng

Chủ đề này hữu ích vì nó cho thấy các ứng dụng cloud thường cần hơn một dịch vụ phối hợp với nhau để đáp ứng nhu cầu người dùng và doanh nghiệp đang tăng trưởng.

[Đọc bài gốc của AWS](https://aws.amazon.com/blogs/architecture/building-a-scalable-user-search-layer-on-top-of-amazon-cognito/)