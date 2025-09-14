# Phase 3 – Data Persistence and Streams (2–3 months)

### Basic SQL
- **DDL**: `CREATE`, `ALTER`.  
- **DML**: `SELECT`, `INSERT`, `UPDATE`, `DELETE`.  
- **Joins**: `INNER`, `LEFT`, `RIGHT`.  
- **Keys**: primary and foreign keys.  
- **Normalization**: 1NF, 2NF, 3NF.  
- **Example**: create tables for products and categories.  

### JDBC and Connection Pool
- **Classes**: `Connection`, `Statement`, `PreparedStatement`, `ResultSet`.  
- Use of Connection Pool (**HikariCP**).  
- **Best practices**: `try-with-resources`, handling of `SQLException`.  

### Hibernate + JPA in Practice
- **Annotations**: `@Entity`, `@Id`, `@ManyToOne`, `@OneToMany`.  
- **Configuration**: `persistence.xml` or `application.properties`.  
- **CRUD** operations with `EntityManager`.  
- Introduction to database migrations with Flyway or Liquibase.

### Introduction to NoSQL Databases
- **Concepts**: documents, collections, horizontal scalability.  
- **MongoDB**: setup, CRUD operations with MongoRepository.  
- **Spring Data MongoDB**: integration with Spring Boot.  
- **Example**: store system activity logs for products in MongoDB.

### Streams and Lambda Expressions
- **Operations**: `filter`, `map`, `sorted`, `collect`, `forEach`, `reduce`.  
- **Example**: filter products by price, sort by name.  

### Optional and Functional Interfaces
- `Optional`: `orElse`, `ifPresent`, `orElseThrow`.  
- **Functional interfaces**: `Function`, `Predicate`, `Consumer`.  
- **Example**: use `Predicate` in Streams to filter data.  

### Advanced Collections
- **LinkedList**: efficient insertion/removal.  
- **TreeMap**: ordered key-value pairs.  
- **PriorityQueue**: priority queue.  
- **LinkedHashMap** and **Deque** (introduction).  

### Logging (SLF4J/Logback)
- Configuration of SLF4J with Logback.  
- **Levels**: `INFO`, `DEBUG`, `ERROR`.  
- **Example**: log Hibernate queries.  

### Transaction Concepts (ACID)
- Atomicity, Consistency, Isolation, Durability.  
- Transactions with JDBC (`commit`, `rollback`) and Hibernate (`@Transactional`).  

### Indexes and Execution Plans
- **Indexes**: primary, unique, composite.  
- Use of **EXPLAIN** to optimize queries.  
- **Example**: create an index on a frequently searched column.  

### File Manipulation (Optional)
- Reading and writing with `Files`, `BufferedReader`.  
- **Example**: export product report to CSV using Streams.  

### Database Testing (Introduction)
- Integration tests with **H2** and **JUnit**.  
- **Example**: test CRUD operations with Hibernate.  

### Final Project
**Product Management System**  
- Database: **Product** and **Category** tables (1:N relationship).  
- Java: classes with JPA (`Product`, `Category`), CRUD with Hibernate.  
- **Optional**: store product change logs in MongoDB.  
- **Optional**: store dynamic product attributes (e.g., technical specifications) in MongoDB.  
- Streams: filter/sort products (e.g., by price or category).  
- Logging: monitor database operations.  
- Git: commit per feature (e.g., `feature/crud`, `feature/streams`).  
- Publish on GitHub with explanatory README.  

### Resources
- [SQLBolt](https://sqlbolt.com/)
- [PostgreSQL Official Docs](https://www.postgresql.org/docs/)  
- [Baeldung](https://www.baeldung.com/)  
- [Use The Index, Luke!](https://use-the-index-luke.com/)
- [Hibernate Official Docs](https://hibernate.org/orm/documentation/) 
- [Baeldung – Logging with SLF4J](https://www.baeldung.com/slf4j)
- [Flyway](https://flywaydb.org/)
- [MongoDB University](https://university.mongodb.com/)