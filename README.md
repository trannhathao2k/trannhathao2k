## Các đường dẫn tài liệu em đã tìm hiểu
* Kiến trúc Microservice
  1. [Kiến trúc Microservice là gì? Cùng tìm hiểu trong 10 phút](https://phambinh.net/bai-viet/kien-truc-microservice-la-gi-cung-tim-hieu-trong-10-phut/)
  2. [API Gateway là gì? Tại sao một hệ thống microservices lại cần API Gateway?](https://viblo.asia/p/api-gateway-la-gi-tai-sao-mot-he-thong-microservices-lai-can-api-gateway-Do754pDX5M6).

* Java Spring Boot
  1. [Khóa học Java Spring Boot 2021 trong 2 giờ (Youtube)](https://youtu.be/UMePnyjr6FM)
  2. [Giới thiệu về Spring Boot. Spring Boot là gì?](https://topdev.vn/blog/gioi-thieu-ve-spring-boot-spring-boot-la-gi/#:~:text=Spring%20Boot%20l%C3%A0%20m%E1%BB%99t%20d%E1%BB%B1,tri%E1%BB%83n%20business%20cho%20%E1%BB%A9ng%20d%E1%BB%A5ng.)

## Những nội dung đã tìm hiểu
* **Về kiến trúc Microservice:**
  * Những dự án trước đây em thực hiện đều được xây dựng với kiến trúc Monolithic (phần mềm dạng nguyên khối), mọi tính năng đều nằm trong 1 project và cả project chỉ được xây dựng trên một công nghệ nhất định. Qua tìm hiểu về kiến trúc Microservice, em hiểu đây là kiến trúc theo kiểu chia nhỏ các tính năng hoạt động trong một dự án thành nhiều service nhỏ, các service này hoạt động độc lập với nhau, chúng có thể sử dụng công nghệ khác nhau và thậm chí là database riêng biệt, và chúng sẽ trao đổi thông tin thông qua môi trường mạng (có thể bằng endpoint restful API hoặc các message queue (em vẫn đang tìm hiểu thêm về phần này)).
* **Về Database MySQL:**
    * MySQL là một hệ quản trị cơ sở dữ liệu mã nguồn mở hoạt động theo mô hình client-server, MySQL tạo ra bảng để lưu trữ dữ liệu, định nghĩa sự liên quan giữa các bảng đó, client sẽ gửi yêu cầu SQL bằng một lệnh đặt biệt trên MySQL, ứng dụng trên server sẽ phản hồi thông tin và trả về kết quả trên máy client.
* **Về Java Spring Boot:**
  * Spring Boot là một dự án phát triển bởi JAVA trong hệ sinh thái Spring framework. Nó giúp cho các lập trình viên chúng ta đơn giản hóa quá trình lập trình một ứng dụng với Spring, chỉ tập trung vào việc phát triển business cho ứng dụng.
  * Để có thể khởi tạo một dự án Spring Boot, ta cần cài đặt Spring Boot CLI.
  * Các ưu điểm của Spring Boot:
    * Hội tụ đầy đủ các tính năng của Spring framework.
    * Đơn giản hóa cấu hình và xây dựng được các ứng dụng độc lập có khả năng chạy bằng java-jar nhờ các dependency starter. 
    * Dễ dàng deploy vì các ứng dụng server được nhúng trực tiếp vào ứng dụng để tránh những khó khăn khi triển khai lên môi trường production mà không cần thiết phải tải file WAR.
    * Cấu hình ít, tự động được hỗ trợ bất cứ khi nào cho chức năng spring như tăng năng suất, giảm thời gian viết code và không yêu cầu XML config.
    * Cung cấp nhiều plugin, số liệu, cấu hình ứng dụng từ bên ngoài.
