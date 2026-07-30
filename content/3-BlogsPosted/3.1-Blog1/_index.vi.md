---
title: "Blog 1"
date: 2026-06-06
weight: 1
chapter: false
pre: " <b> 3.1. </b> "
---

# Building Multi-Region Resiliency for AWS CloudFormation Custom Resource Deployment

Ý tưởng chính của bài viết là chỉ ra cách làm cho AWS CloudFormation custom resources trở nên đáng tin cậy hơn khi triển khai trên nhiều Region khác nhau. Bài viết tập trung vào các vấn đề thường gặp như lỗi vận hành, retry, triển khai một phần và trạng thái không nhất quán giữa các Region.

## Ý chính

CloudFormation custom resources rất hữu ích, nhưng trong môi trường đa Region chúng có thể tạo ra nhiều rủi ro. Chúng cho phép đội ngũ mở rộng CloudFormation bằng logic tùy chỉnh, nhưng đồng thời cũng làm tăng các thách thức về độ tin cậy. Khi stack được triển khai qua nhiều Region, một lỗi ở một Region, timeout hoặc phản hồi chậm có thể dẫn đến thao tác chưa hoàn tất hoặc trạng thái không đồng bộ. Bài viết cho thấy vấn đề không chỉ nằm ở tính sẵn sàng mà còn ở việc tránh việc thực thi trùng lặp và đảm bảo khôi phục an toàn sau lỗi.

## Các vấn đề được nhấn mạnh

- CloudFormation không cung cấp cơ chế phối hợp đa Region tích hợp sẵn cho custom resources.
- Cùng một sự kiện có thể được xử lý bởi nhiều Region, dẫn đến tác dụng phụ bị lặp lại.
- Không có cơ chế locking phân tán để đảm bảo chỉ một handler xử lý một request.
- Nếu Region chính gặp lỗi, không có failover tự động trong luồng custom resource.
- Developers cần xử lý idempotency cẩn thận để retry không tạo ra bản sao không mong muốn.

## Cách tiếp cận giải pháp

Giải pháp đề xuất là kiến trúc active-active đa Region. Theo đó, nhiều Region được chuẩn bị để xử lý sự kiện cùng lúc, nhưng chỉ một Region nên xử lý một request cụ thể. Kiến trúc này sử dụng trạng thái phân tán và cơ chế phối hợp để ngăn xử lý trùng lặp. Đồng thời, nó cũng bao gồm retry logic, monitoring và failover để hệ thống có thể tự phục hồi khi một Region gặp sự cố. Điều này làm cho quá trình triển khai đáng tin cậy hơn và phù hợp hơn với workload quan trọng.

![overview](/images/3-Blogs/blog1.png)

## Điều em học được

Từ bài viết này, em có thể học được:

- hiểu cách custom resources hoạt động trong CloudFormation
- thiết kế hệ thống bền vững và an toàn hơn khi xảy ra lỗi
- áp dụng các khái niệm quan trọng như idempotency, retries và monitoring
- hiểu sâu hơn về các dịch vụ AWS như Lambda, DynamoDB, SQS và Step Functions

[Đọc bài gốc của AWS](https://aws.amazon.com/blogs/architecture/building-multi-region-resiliency-for-aws-cloudformation-custom-resource-deployment/)