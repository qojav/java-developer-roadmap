# 3단계 – 데이터 지속성과 Streams (2~3개월)

### 기본 SQL
- **DDL**: `CREATE`, `ALTER`.  
- **DML**: `SELECT`, `INSERT`, `UPDATE`, `DELETE`.  
- **Joins**: `INNER`, `LEFT`, `RIGHT`.  
- **Keys**: Primary Key와 Foreign Key.  
- **정규화**: 1NF, 2NF, 3NF.  
- **예제**: 제품 및 카테고리 테이블 생성.  

### JDBC와 Connection Pool
- **Classes**: `Connection`, `Statement`, `PreparedStatement`, `ResultSet`.  
- Connection Pool (**HikariCP**) 사용.  
- **모범 사례**: `try-with-resources`, `SQLException` 처리.  

### Hibernate + JPA 실습
- **Annotations**: `@Entity`, `@Id`, `@ManyToOne`, `@OneToMany`.  
- **설정**: `persistence.xml` 또는 `application.properties`.  
- `EntityManager`를 사용한 **CRUD** 작업.  
- Flyway 또는 Liquibase를 사용한 데이터베이스 마이그레이션 소개.

### NoSQL 데이터베이스 소개
- **개념**: 문서, 컬렉션, 수평적 확장성.  
- **MongoDB**: 설정, MongoRepository를 사용한 CRUD 작업.  
- **Spring Data MongoDB**: Spring Boot와의 통합.  
- **예제**: MongoDB에 제품의 시스템 활동 로그 저장.  

### Streams와 Lambda Expressions
- **작업**: `filter`, `map`, `sorted`, `collect`, `forEach`, `reduce`.  
- **예제**: 가격으로 제품 필터링, 이름으로 정렬.  

### Optional과 Functional Interfaces
- `Optional`: `orElse`, `ifPresent`, `orElseThrow`.  
- **Functional Interfaces**: `Function`, `Predicate`, `Consumer`.  
- **예제**: Streams에서 데이터를 필터링하기 위해 `Predicate` 사용.  

### 고급 Collections
- **LinkedList**: 효율적인 삽입/삭제.  
- **TreeMap**: 정렬된 key-value 쌍.  
- **PriorityQueue**: 우선순위 큐.  
- **LinkedHashMap** 및 **Deque** (소개).  

### 로깅 (SLF4J/Logback)
- SLF4J와 Logback 설정.  
- **레벨**: `INFO`, `DEBUG`, `ERROR`.  
- **예제**: Hibernate 쿼리 로깅.  

### 트랜잭션 개념 (ACID)
- 원자성, 일관성, 격리성, 지속성.  
- JDBC (`commit`, `rollback`) 및 Hibernate (`@Transactional`)를 사용한 트랜잭션.  

### 인덱스와 실행 계획
- **Indexes**: Primary, Unique, Composite.  
- 쿼리 최적화를 위한 **EXPLAIN** 사용.  
- **예제**: 자주 검색되는 컬럼에 인덱스 생성.  

### 파일 조작 (선택 사항)
- `Files`, `BufferedReader`를 사용한 읽기 및 쓰기.  
- **예제**: Streams를 사용하여 CSV로 제품 보고서 내보내기.  

### 데이터베이스 테스트 (소개)
- **H2** 및 **JUnit**를 사용한 통합 테스트.  
- **예제**: Hibernate를 사용한 CRUD 작업 테스트.  

### 최종 프로젝트
**제품 관리 시스템**  
- 데이터베이스: **Product** 및 **Category** 테이블 (1:N 관계).  
- Java: JPA (`Product`, `Category`)를 사용한 클래스, Hibernate로 CRUD.  
- **선택 사항**: MongoDB에 제품 변경 로그 저장.  
- **선택 사항**: MongoDB에 동적 제품 속성 (예: 기술 사양) 저장.  
- Streams: 제품 필터링/정렬 (예: 가격 또는 카테고리 기준).  
- 로깅: 데이터베이스 작업 모니터링.  
- Git: 기능별 commit (예: `feature/crud`, `feature/streams`).  
- 설명이 포함된 README와 함께 GitHub에 공개.  

### 리소스
- [SQLBolt](https://sqlbolt.com/)
- [PostgreSQL Official Docs](https://www.postgresql.org/docs/)  
- [Baeldung](https://www.baeldung.com/)  
- [Use The Index, Luke!](https://use-the-index-luke.com/)
- [Hibernate Official Docs](https://hibernate.org/orm/documentation/) 
- [Baeldung – Logging with SLF4J](https://www.baeldung.com/slf4j)
- [Flyway](https://flywaydb.org/)
- [MongoDB University](https://university.mongodb.com/)