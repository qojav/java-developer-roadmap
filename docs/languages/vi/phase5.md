# Giai đoạn 5 – Kiến trúc và Đồng thời (2–3 tháng)

### Clean Code và Nguyên tắc SOLID
- **Clean Code**: Đặt tên rõ ràng, hàm ngắn gọn, bình luận hữu ích, định dạng nhất quán.  
- **SOLID**:  
  - SRP (Single Responsibility Principle)  
  - OCP (Open/Closed Principle)  
  - LSP (Liskov Substitution Principle)  
  - ISP (Interface Segregation Principle)  
  - DIP (Dependency Inversion Principle)  

**Ví dụ:** Tái cấu trúc một dịch vụ trong Task Manager để tuân theo nguyên tắc SOLID.  

### Mẫu thiết kế
- **Mẫu**: Factory (tạo), Singleton (một thể hiện duy nhất), Builder (xây dựng đối tượng), Strategy (hành vi), Observer (sự kiện).  
- **Ứng dụng**: Chọn các mẫu phù hợp với ngữ cảnh dự án.  

**Ví dụ:** Sử dụng Strategy cho các thuật toán ưu tiên tác vụ khác nhau.  

### Luồng và Đồng thời
- **Khái niệm**: Thread, Runnable, ExecutorService, ForkJoinPool.  
- **Kỹ thuật**: Tạo và quản lý pool luồng, tác vụ bất đồng bộ.  

**Ví dụ:** Xử lý báo cáo tác vụ song song với ExecutorService.  

### Đồng bộ hóa và Vấn đề Đồng thời
- **Cơ chế**: `synchronized`, `Lock`, `ReentrantLock`, `ConcurrentHashMap`.  
- **Vấn đề**: Deadlock, race condition, starvation.  

**Ví dụ:** Triển khai truy cập an toàn vào danh sách tác vụ chia sẻ.  

### Giới thiệu về Microservices
- **Khái niệm**: Kiến trúc microservices, giao tiếp REST, khám phá dịch vụ.  
- **Công cụ**: Spring Cloud (ví dụ: Eureka để khám phá dịch vụ).  

**Ví dụ:** Chia Task Manager thành các microservices (tác vụ và người dùng).  

### Cơ bản về Hàng đợi Tin nhắn (Tùy chọn)
- **Khái niệm**: Publisher/subscriber, queues, topics.  
- **RabbitMQ**: Thiết lập, gửi và nhận tin nhắn.  

**Ví dụ:** Thông báo người dùng về cập nhật tác vụ qua RabbitMQ.  

### Tối ưu hóa Hiệu suất
- **Caching**: Spring Cache với Redis để giảm truy cập cơ sở dữ liệu.  
- **Tuning JVM**: Khái niệm cơ bản (heap, garbage collection).  

**Ví dụ:** Triển khai cache cho các truy vấn thường xuyên trong hệ thống tác vụ.  

### Giới thiệu về DevOps/Cloud: Docker và CI/CD
- **Docker**: Containers, images, Dockerfile, Docker Compose.  
- **CI/CD**: Cấu hình pipeline với GitHub Actions để xây dựng và triển khai.  

**Ví dụ:** Tạo Dockerfile cho ứng dụng tác vụ và triển khai qua GitHub Actions.  

### Quan sát (Observability)
- **Công cụ**: Prometheus (metrics), Grafana (hình ảnh hóa), ELK Stack (logs).  
- **Khái niệm**: Giám sát hiệu suất, logs tập trung, cảnh báo.  

**Ví dụ:** Giám sát thời gian phản hồi API tác vụ với Prometheus và Grafana.  

### Bảo mật: OWASP Top Ten
- **Khái niệm**: Injection, lỗi xác thực, lộ dữ liệu nhạy cảm.  
- **Thực hành**: Xác thực đầu vào, làm sạch dữ liệu, cấu hình an toàn.  

**Ví dụ:** Bảo vệ API tác vụ khỏi SQL injection và XSS.  

### Dự án cuối kỳ
**Hệ thống Quản lý Tác vụ Nâng cao**  
- Backend: Nâng cấp API tác vụ (Giai đoạn 4) với microservices (tác vụ và người dùng).  
- Kiến trúc: Tái cấu trúc với Clean Code, SOLID và các mẫu thiết kế (ví dụ: Strategy).  
- Đồng thời: Xử lý báo cáo song song với ExecutorService.  
- **Tùy chọn**: Thêm giao tiếp giữa các microservices qua RabbitMQ và caching với Redis cho các truy vấn thường xuyên.  
- DevOps: Đóng gói trong Docker, cấu hình CI/CD với GitHub Actions.  
- Quan sát: Thêm Prometheus và Grafana cho metrics.  
- Bảo mật: Triển khai các biện pháp bảo vệ khỏi OWASP Top Ten.  
- Git: Commit cho mỗi tính năng (ví dụ: `feature/microservices`, `feature/concurrency`).  
- Đăng lên GitHub với README chi tiết (cấu hình, kiến trúc, triển khai).  

### Tài nguyên
- *The Pragmatic Programmer* (Sách)  
- *Effective Java* (Sách)  
- *Java Concurrency in Practice* (Sách)  
- [Spring Cloud Documentation](https://spring.io/projects/spring-cloud)  
- [RabbitMQ Tutorials](https://www.rabbitmq.com/getstarted.html)  
- [Redis University](https://university.redis.com/)  
- [Docker Official Docs](https://docs.docker.com/)  
- [Prometheus Documentation](https://prometheus.io/docs/introduction/overview/)  
- [Grafana Documentation](https://grafana.com/docs/)  
- [ELK Stack Guide](https://www.elastic.co/what-is/elk-stack)  
- [OWASP Top Ten](https://owasp.org/www-project-top-ten/)  
- [GitHub Actions Documentation](https://docs.github.com/en/actions)