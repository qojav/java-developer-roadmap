# 第三阶段 – 数据持久化与Streams（2-3个月）

### 基本SQL
- **DDL**: `CREATE`, `ALTER`.  
- **DML**: `SELECT`, `INSERT`, `UPDATE`, `DELETE`.  
- **Joins**: `INNER`, `LEFT`, `RIGHT`.  
- **Keys**: 主键和外键.  
- **Normalization**: 1NF, 2NF, 3NF.  
- **示例**: 为产品和类别创建表.  

### JDBC与Connection Pool
- **Classes**: `Connection`, `Statement`, `PreparedStatement`, `ResultSet`.  
- 使用Connection Pool (**HikariCP**).  
- **最佳实践**: `try-with-resources`, 处理`SQLException`.  

### Hibernate + JPA实践
- **Annotations**: `@Entity`, `@Id`, `@ManyToOne`, `@OneToMany`.  
- **Configuration**: `persistence.xml` 或 `application.properties`.  
- 使用`EntityManager`进行**CRUD**操作.  
- 数据库迁移介绍，使用Flyway或Liquibase.

### NoSQL数据库介绍
- **概念**: 文档、集合、水平扩展.  
- **MongoDB**: 设置，CRUD操作使用MongoRepository.  
- **Spring Data MongoDB**: 与Spring Boot集成.  
- **示例**: 在MongoDB中存储产品系统活动日志.

### Streams与Lambda Expressions
- **操作**: `filter`, `map`, `sorted`, `collect`, `forEach`, `reduce`.  
- **示例**: 按价格过滤产品，按名称排序.  

### Optional与Functional Interfaces
- `Optional`: `orElse`, `ifPresent`, `orElseThrow`.  
- **Functional interfaces**: `Function`, `Predicate`, `Consumer`.  
- **示例**: 在Streams中使用`Predicate`过滤数据.  

### 高级集合
- **LinkedList**: 高效插入/删除.  
- **TreeMap**: 有序键值对.  
- **PriorityQueue**: 优先级队列.  
- **LinkedHashMap** 和 **Deque** (介绍).  

### Logging (SLF4J/Logback)
- 配置SLF4J与Logback.  
- **级别**: `INFO`, `DEBUG`, `ERROR`.  
- **示例**: 记录Hibernate queries.  

### 事务概念 (ACID)
- 原子性、一致性、隔离性、持久性.  
- JDBC事务 (`commit`, `rollback`) 和 Hibernate (`@Transactional`).  

### 索引与执行计划
- **Indexes**: 主键、唯一、复合索引.  
- 使用**EXPLAIN**优化queries.  
- **示例**: 在经常搜索的列上创建索引.  

### 文件操作 (可选)
- 使用`Files`, `BufferedReader`进行读写.  
- **示例**: 使用Streams将产品报告导出为CSV.  

### 数据库测试 (介绍)
- 使用**H2**和**JUnit**进行集成测试.  
- **示例**: 测试Hibernate的CRUD操作.  

### 最终项目
**产品管理系统**  
- 数据库: **Product** 和 **Category** 表 (1:N关系).  
- Java: 使用JPA的类 (`Product`, `Category`), 使用Hibernate进行CRUD.  
- **可选**: 在MongoDB中存储产品变更日志.  
- **可选**: 在MongoDB中存储产品的动态属性（例如，技术规格）.  
- Streams: 过滤/排序产品（例如，按价格或类别）.  
- Logging: 监控数据库操作.  
- Git: 按功能提交（例如，`feature/crud`, `feature/streams`）.  
- 在GitHub上发布，附带说明性README.  

### 资源
- [SQLBolt](https://sqlbolt.com/)
- [PostgreSQL Official Docs](https://www.postgresql.org/docs/)  
- [Baeldung](https://www.baeldung.com/)  
- [Use The Index, Luke!](https://use-the-index-luke.com/)
- [Hibernate Official Docs](https://hibernate.org/orm/documentation/) 
- [Baeldung – Logging with SLF4J](https://www.baeldung.com/slf4j)
- [Flyway](https://flywaydb.org/)
- [MongoDB University](https://university.mongodb.com/)