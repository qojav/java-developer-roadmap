# Giai đoạn 3 – Lưu trữ dữ liệu và Streams (2–3 tháng)

### SQL cơ bản
- **DDL**: `CREATE`, `ALTER`.  
- **DML**: `SELECT`, `INSERT`, `UPDATE`, `DELETE`.  
- **Joins**: `INNER`, `LEFT`, `RIGHT`.  
- **Keys**: khóa chính và khóa ngoại.  
- **Chuẩn hóa**: 1NF, 2NF, 3NF.  
- **Ví dụ**: tạo bảng cho sản phẩm và danh mục.  

### JDBC và Connection Pool
- **Classes**: `Connection`, `Statement`, `PreparedStatement`, `ResultSet`.  
- Sử dụng Connection Pool (**HikariCP**).  
- **Thực hành tốt**: `try-with-resources`, xử lý `SQLException`.  

### Hibernate + JPA trong thực tế
- **Annotations**: `@Entity`, `@Id`, `@ManyToOne`, `@OneToMany`.  
- **Cấu hình**: `persistence.xml` hoặc `application.properties`.  
- **CRUD** operations với `EntityManager`.  
- Giới thiệu về di chuyển cơ sở dữ liệu với Flyway hoặc Liquibase.

### Giới thiệu về cơ sở dữ liệu NoSQL
- **Khái niệm**: documents, collections, khả năng mở rộng ngang.  
- **MongoDB**: thiết lập, CRUD operations với MongoRepository.  
- **Spring Data MongoDB**: tích hợp với Spring Boot.  
- **Ví dụ**: lưu trữ nhật ký hoạt động hệ thống cho sản phẩm trong MongoDB.

### Streams và Lambda Expressions
- **Operations**: `filter`, `map`, `sorted`, `collect`, `forEach`, `reduce`.  
- **Ví dụ**: lọc sản phẩm theo giá, sắp xếp theo tên.  

### Optional và Functional Interfaces
- `Optional`: `orElse`, `ifPresent`, `orElseThrow`.  
- **Functional interfaces**: `Function`, `Predicate`, `Consumer`.  
- **Ví dụ**: sử dụng `Predicate` trong Streams để lọc dữ liệu.  

### Bộ sưu tập nâng cao
- **LinkedList**: thêm/xóa hiệu quả.  
- **TreeMap**: cặp khóa-giá trị được sắp xếp.  
- **PriorityQueue**: hàng đợi ưu tiên.  
- **LinkedHashMap** và **Deque** (giới thiệu).  

### Logging (SLF4J/Logback)
- Cấu hình SLF4J với Logback.  
- **Levels**: `INFO`, `DEBUG`, `ERROR`.  
- **Ví dụ**: ghi nhật ký các truy vấn Hibernate.  

### Khái niệm giao dịch (ACID)
- Tính nguyên tử, nhất quán, cô lập, bền vững.  
- Giao dịch với JDBC (`commit`, `rollback`) và Hibernate (`@Transactional`).  

### Chỉ mục và kế hoạch thực thi
- **Indexes**: chính, duy nhất, tổng hợp.  
- Sử dụng **EXPLAIN** để tối ưu hóa truy vấn.  
- **Ví dụ**: tạo chỉ mục cho cột thường xuyên được tìm kiếm.  

### Thao tác với tệp (Tùy chọn)
- Đọc và ghi với `Files`, `BufferedReader`.  
- **Ví dụ**: xuất báo cáo sản phẩm sang CSV bằng Streams.  

### Kiểm thử cơ sở dữ liệu (Giới thiệu)
- Kiểm thử tích hợp với **H2** và **JUnit**.  
- **Ví dụ**: kiểm thử CRUD operations với Hibernate.  

### Dự án cuối kỳ
**Hệ thống quản lý sản phẩm**  
- Cơ sở dữ liệu: bảng **Product** và **Category** (quan hệ 1:N).  
- Java: các lớp với JPA (`Product`, `Category`), CRUD với Hibernate.  
- **Tùy chọn**: lưu trữ nhật ký thay đổi sản phẩm trong MongoDB.  
- **Tùy chọn**: lưu trữ các thuộc tính động của sản phẩm (ví dụ: thông số kỹ thuật) trong MongoDB.  
- Streams: lọc/sắp xếp sản phẩm (ví dụ: theo giá hoặc danh mục).  
- Logging: giám sát các hoạt động cơ sở dữ liệu.  
- Git: commit cho mỗi tính năng (ví dụ: `feature/crud`, `feature/streams`).  
- Đăng lên GitHub với README giải thích rõ ràng.  

### Tài nguyên
- [SQLBolt](https://sqlbolt.com/)
- [PostgreSQL Official Docs](https://www.postgresql.org/docs/)  
- [Baeldung](https://www.baeldung.com/)  
- [Use The Index, Luke!](https://use-the-index-luke.com/)
- [Hibernate Official Docs](https://hibernate.org/orm/documentation/) 
- [Baeldung – Logging with SLF4J](https://www.baeldung.com/slf4j)
- [Flyway](https://flywaydb.org/)
- [MongoDB University](https://university.mongodb.com/)