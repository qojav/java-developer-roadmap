# Giai đoạn 4 – Frameworks và Ứng dụng Web (3–4 tháng)

### Spring Boot, Spring Core và Spring Data JPA
- **Spring Core**: Dependency injection (`@Bean`, `@Autowired`), IoC container.  
- **Spring Boot**: Tự động cấu hình, starters (`spring-boot-starter-web`, `spring-boot-starter-data-jpa`), `application.yml`.  
- **Spring Data JPA**: Repositories (`CrudRepository`, `JpaRepository`), truy vấn với `@Query`, phân trang.  
- **Ví dụ**: Tạo REST endpoints để quản lý tác vụ (**CRUD**) trong ứng dụng tác vụ.  

### Spring Security (JWT, OAuth2)
- **Khái niệm**: Xác thực, phân quyền, bộ lọc bảo mật.  
- **JWT**: Tạo và xác thực token, sử dụng `JwtAuthenticationFilter`.  
- **OAuth2**: Cấu hình Resource Server, tích hợp với nhà cung cấp (ví dụ: Google).  
- **Ví dụ**: Bảo vệ các endpoints tác vụ với JWT và vai trò (`ADMIN`, `USER`).  

### Kiểm thử đơn vị và tích hợp
- **Kiểm thử đơn vị**: JUnit 5, Mockito (`@Mock`, `@InjectMocks`), kiểm thử logic nghiệp vụ.  
- **Kiểm thử tích hợp**: `@SpringBootTest`, `@WebMvcTest`, cơ sở dữ liệu **H2** để kiểm thử.  
- **Testcontainers**: Kiểm thử với PostgreSQL trong container Docker.  
- **Ví dụ**: Kiểm thử các dịch vụ và endpoints của ứng dụng tác vụ.  

### RESTful APIs và tài liệu với Swagger
- **REST**: Các phương thức HTTP, mã trạng thái, nguyên tắc RESTful.  
- **Spring REST**: `@RestController`, `@RequestMapping`, `@PathVariable`.  
- **Swagger**: Cấu hình **springdoc-openapi**, chú thích với `@Operation`.  
- **Ví dụ**: Tài liệu hóa các endpoints của ứng dụng tác vụ với **Swagger UI**.  

### Giới thiệu về GraphQL
- **Khái niệm**: Queries, mutations, schema.  
- **Spring Boot với GraphQL**: Thiết lập với spring-boot-starter-graphql.  
- **Ví dụ**: Tạo một GraphQL query để liệt kê các tác vụ theo trạng thái.  

### Tích hợp Frontend cơ bản
- **Thymeleaf**: Mẫu để hiển thị các trang HTML với Spring Boot.  
- **Ví dụ**: Tạo giao diện web đơn giản để xem và tạo tác vụ.  

### Công cụ xây dựng: Maven và Gradle
- **Maven**: Cấu trúc của `pom.xml`, quản lý phụ thuộc, plugin.  
- **Gradle**: Tệp `build.gradle`, các tác vụ, quản lý phụ thuộc.  
- **Ví dụ**: Cấu hình ứng dụng tác vụ với Maven và Gradle.  

### Triển khai dự án
- **Nền tảng**: Railway, Heroku, AWS (Elastic Beanstalk).  
- **Các bước**: Đóng gói thành JAR, cấu hình CI/CD với GitHub Actions.  
- **Ví dụ**: Triển khai ứng dụng tác vụ trên Railway với PostgreSQL.  

### Dự án cuối kỳ
**Hệ thống quản lý tác vụ**  
- Cơ sở dữ liệu: Bảng `Task` (tiêu đề, mô tả, trạng thái) và `User` (quan hệ 1:N).  
- Java: REST API với Spring Boot, Spring Data JPA cho CRUD.  
- Bảo mật: Xác thực JWT, vai trò (`ADMIN`, `USER`).  
- Kiểm thử: Kiểm thử đơn vị (dịch vụ) và kiểm thử tích hợp (endpoints với Testcontainers).  
- Tài liệu: Swagger UI với mô tả các endpoints.  
- **Tùy chọn**: Thêm GraphQL query để liệt kê tác vụ và giao diện Thymeleaf để tương tác.  
- Git: Commit cho mỗi tính năng (ví dụ: `feature/rest-api`, `feature/security`).  
- Đăng lên GitHub với README (cấu hình, endpoints, triển khai).  

### Tài nguyên
- [Spring Boot Official Docs](https://spring.io/projects/spring-boot)  
- [Baeldung – Spring Boot Tutorials](https://www.baeldung.com/spring-boot)  
- [Spring Security Guide](https://spring.io/guides/topicals/spring-security-architecture)  
- [Testcontainers Official Docs](https://testcontainers.org/)  
- [Springdoc OpenAPI (Swagger)](https://springdoc.org/)  
- [AWS Free Tier Tutorials](https://aws.amazon.com/free/)  
- [GraphQL Official](https://graphql.org/learn/)  
- [Spring Boot with Thymeleaf](https://spring.io/guides/gs/serving-web-content/)  
- [Railway Documentation](https://docs.railway.app/)  
- [Heroku Dev Center](https://devcenter.heroku.com/)  
- [GitHub Actions Documentation](https://docs.github.com/en/actions)