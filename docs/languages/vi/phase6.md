# Giai đoạn 6 – Dự án cuối kỳ (Liên tục)

### Dự án 1: CRUD hoàn chỉnh với Xác thực
- **Mục tiêu**: Xây dựng một RESTful API mạnh mẽ với xác thực an toàn và kiểm thử.  
- **Công nghệ**: Spring Boot, Spring Data JPA (PostgreSQL), Spring Security (JWT), JUnit 5, Testcontainers.  
- **Tính năng**: CRUD cho các thực thể (ví dụ: tác vụ, người dùng), xác thực với vai trò (ADMIN, USER), tài liệu với Swagger.  
- **Tùy chọn**: Thêm giao diện Thymeleaf để xem/quản lý tác vụ.  
- **Ví dụ**: API để quản lý dự án (thực thể: `Project`, `Task`, `User`) với các endpoint được bảo vệ.  

### Dự án 2: Tải lên tệp
- **Mục tiêu**: Thêm chức năng tải lên tệp vào API từ Dự án 1.  
- **Công nghệ**: Spring Boot (`MultipartFile`), Amazon S3 hoặc lưu trữ cục bộ, xác thực tệp.  
- **Tính năng**: Tải lên hình ảnh/tài liệu liên quan đến tác vụ, xác thực loại/kích thước.  
- **Ví dụ**: Cho phép tải lên tệp đính kèm (ví dụ: PDF, PNG) cho tác vụ trong API.  

### Dự án 3: Triển khai trên đám mây
- **Mục tiêu**: Triển khai API lên nền tảng đám mây với CI/CD.  
- **Công nghệ**: Railway, Heroku, hoặc AWS (Elastic Beanstalk), GitHub Actions, Docker.  
- **Tính năng**: Đóng gói thành JAR/Docker, cấu hình biến môi trường, tự động hóa triển khai.  
- **Tùy chọn**: Triển khai caching với Redis để tối ưu hóa các truy vấn thường xuyên.  
- **Ví dụ**: Triển khai API dự án trên Railway với PostgreSQL và CI/CD.  

### Dự án 4: Microservices
- **Mục tiêu**: Chia API từ Dự án 1 thành các microservices được điều phối.  
- **Công nghệ**: Spring Cloud (Eureka, Gateway), Docker Compose, REST để giao tiếp.  
- **Tính năng**: Microservices cho `Tasks` và `Users`, với khám phá dịch vụ.  
- **Tùy chọn**: Sử dụng RabbitMQ để giao tiếp bất đồng bộ giữa các microservices.  
- **Ví dụ**: Tách logic tác vụ và người dùng thành hai dịch vụ, được điều phối với Docker.  

### Dự án 5: Tích hợp API bên ngoài
- **Mục tiêu**: Sử dụng API bên ngoài để nâng cao chức năng.  
- **Công nghệ**: Spring RestTemplate hoặc WebClient, xác thực API (ví dụ: OAuth2).  
- **Tính năng**: Tích hợp với API công khai (ví dụ: gửi thông báo qua email với SendGrid).  
- **Tùy chọn**: Thêm GraphQL query để truy xuất tác vụ/người dùng và lưu trữ metadata trong MongoDB.  
- **Ví dụ**: Thêm thông báo email khi hoàn thành tác vụ.  

### Thực hành tốt cho Portfolio
- **Git**: Commit cho mỗi tính năng (ví dụ: `feature/crud`, `feature/upload`), các nhánh rõ ràng.  
- **Tài liệu**: README với mô tả, thiết lập, endpoints, triển khai và ảnh chụp màn hình.  
- **Đăng tải**: Lưu trữ trên GitHub với giấy phép mã nguồn mở (ví dụ: MIT).  

### Tài nguyên
- [GitHub Guides](https://guides.github.com)  
- [Spring Boot Official Docs](https://spring.io/projects/spring-boot)  
- [Baeldung – Spring Boot Tutorials](https://www.baeldung.com)  
- [Spring Cloud Documentation](https://spring.io/projects/spring-cloud)  
- [Docker Official Docs](https://docs.docker.com)  
- [Railway Documentation](https://docs.railway.app)  
- [Heroku Dev Center](https://devcenter.heroku.com)  
- [AWS Elastic Beanstalk](https://docs.aws.amazon.com/elasticbeanstalk)  
- [SendGrid API Docs](https://docs.sendgrid.com)  
- [Awesome Open Source](https://awesomeopensource.com)  
- [Practical MongoDB Aggregations](https://university.mongodb.com/courses/MongoDB-Aggregations)