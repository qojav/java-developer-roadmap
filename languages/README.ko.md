## 1단계 – 자바 기초 (1~2개월)

언어 기초

기본 데이터 유형

제어 구조 (if/else, switch)

반복문 (for, while, do-while)

메서드 및 변수 범위

배열 및 기본 컬렉션 소개

예외 처리 소개 (try/catch, throws, 사용자 정의 예외)

Git/GitHub (기본 버전 관리)

📚 자료:

- Oracle Java Tutorials: https://docs.oracle.com/javase/tutorial/
- Exercism.io: https://exercism.org/tracks/java
- Java Programming MOOC by the University of Helsinki: https://java-programming.mooc.fi/
- Git - The Simple Guide: https://rogerdudler.github.io/git-guide/
- GitHub Docs: https://docs.github.com/en/get-started
- Beecrowd: https://www.beecrowd.com.br

## 2단계 – 객체 지향 프로그래밍 (2~3개월)

클래스 및 객체 (수식어, 속성, 메서드)

인터페이스

추상화

캡슐화

상속

다형성

데이터 구조 소개 (리스트, 큐, 스택, 맵)

기본 알고리즘 (검색, 정렬, 재귀)

LeetCode/HackerRank에서 데이터 구조 및 알고리즘(DSA) 문제 해결

📚 자료:

- Oracle Java Tutorials (OOP): https://docs.oracle.com/javase/tutorial/java/concepts/
- Baeldung (Java OOP): https://www.baeldung.com/java-oop
- LeetCode: https://leetcode.com/
- HackerRank (Java Track): https://www.hackerrank.com/domains/java
- Khan Academy (Algorithms): https://www.khanacademy.org/computing/computer-science/algorithms
- Head First Java (Book)

## 3단계 – 데이터베이스 (2개월)

SQL 기초

PostgreSQL 및 MySQL (관계형)

Hibernate + JPA 실습

데이터베이스 마이그레이션 (Flyway/Liquibase)

MongoDB 및 Spring Data Mongo (NoSQL)

인메모리 캐시 및 Redis

메시징 통합 (Kafka/RabbitMQ – 선택 사항이지만 매우 가치 있음)

GraphQL 학습 (글로벌 기업에서 강한 트렌드)

인덱싱 및 쿼리 최적화 연구

📚 자료:

- SQLBolt: https://sqlbolt.com/
- Mode SQL Tutorial: https://mode.com/sql-tutorial/
- PostgreSQL Official Docs: https://www.postgresql.org/docs/
- MySQL Official Docs: https://dev.mysql.com/doc/
- Flyway: https://flywaydb.org/
- Liquibase: https://www.liquibase.org/
- MongoDB University: https://learn.mongodb.com/
- Practical MongoDB Aggregations (Free eBook)
- Redis University: https://university.redis.com/
- Apache Kafka: https://kafka.apache.org/documentation/
- RabbitMQ: https://www.rabbitmq.com/tutorials/
- GraphQL Official: https://graphql.org/
- Use The Index, Luke! (SQL Indexing): https://use-the-index-luke.com/

## 4단계 – 주요 프레임워크 (3~4개월)

Spring Boot

Spring Data JPA

Spring Security (인증/인가, JWT, OAuth2)

Hibernate (ORM)

Maven 및 Gradle (빌드 및 의존성 관리)

JUnit + Mockito (단위 테스트 및 통합 테스트)

Testcontainers (실제 데이터베이스를 사용한 테스트)

최소한 하나의 완전한 프로젝트를 AWS에 배포 (또는 Railway/Heroku, 하지만 AWS가 더 중요)

📚 자료:

- Spring Boot Official Documentation: https://spring.io/projects/spring-boot
- Spring Guides: https://spring.io/guides
- Baeldung (Spring Boot): https://www.baeldung.com/spring-boot
- JUnit: https://junit.org/junit5/
- Mockito: https://site.mockito.org/
- Maven: https://maven.apache.org/
- Gradle: https://gradle.org/
- Testcontainers: https://testcontainers.org/
- AWS Free Tier Tutorials: https://aws.amazon.com/free/
- Railway.app: https://railway.app/

## 5단계 – 시스템 아키텍처 (3개월)

클린 코드 원칙을 적용한 프로젝트

자바에서 자주 사용되는 디자인 패턴 (Factory, Singleton, Builder, Strategy, Observer 등)

SOLID 및 코딩 모범 사례

클린 아키텍처

테스트 케이스 및 TDD

Swagger를 사용한 API 문서화

외부 API와의 통합 (예: Spring OpenAI)

DevOps/클라우드 소개:

Docker 및 Docker Compose

AWS 또는 GCP에 배포

GitHub Actions를 사용한 CI/CD

시스템 설계 학습 (확장성, 고가용성, 서비스 간 통신)

Kubernetes 기초 연구

📚 자료:

- Refactoring Guru (Design Patterns): https://refactoring.guru/design-patterns/java
- MartinFowler.com (Architecture): https://martinfowler.com/
- Docker Official Docs: https://docs.docker.com/
- GitHub Actions: https://docs.github.com/en/actions
- Kubernetes Official Docs: https://kubernetes.io/docs/
- Prometheus: https://prometheus.io/docs/
- Grafana: https://grafana.com/docs/
- Elastic Docs: https://www.elastic.co/guide/
- System Design Primer: https://github.com/donnemartin/system-design-primer
- Clean Architecture (Book, Robert C. Martin)
- Designing Data-Intensive Applications (Book, Martin Kleppmann)

최종 프로젝트 (학습 강화)

인증을 포함한 완전한 CRUD

독립적인 인증 모듈 (JWT + OAuth2)

파일 및 이미지 업로드

데이터베이스 간 데이터 복제

Swagger를 사용한 API 문서화

클라우드에 배포 (예: AWS 또는 Railway)

(보너스) Spring Cloud를 사용한 마이크로서비스 아키텍처

예시:

CRUD + 인증 → CI/CD 파이프라인을 통해 AWS에 배포

파일 및 이미지 업로드 → AWS S3 사용

데이터 복제 → PostgreSQL + MongoDB

문서화된 API (Swagger + README)

## 추가 주제 (편안하다면)

String, StringBuilder, StringBuffer 사용

Stream API 및 Optional

SLF4J/Logback을 사용한 로깅

Spring Boot Profiles + Actuator

트랜잭션 개념 (ACID)

인덱스 및 실행 계획 (EXPLAIN)

헥사고날 아키텍처

관찰 가능성 소개: 중앙화된 메트릭 및 로그 (Prometheus, Grafana 또는 ELK)

복원력: Circuit Breaker (Resilience4j)

보안: OWASP Top Ten (SQL Injection, XSS, CSRF 등) 및 예방 방법

📚 자료:

- Oracle Documentation (Stream API, Optional): https://docs.oracle.com/javase/8/docs/api/
- SLF4J: https://www.slf4j.org/
- Resilience4j: https://resilience4j.readme.io/
- OWASP Top Ten: https://owasp.org/www-project-top-ten/
- Loiane Groner: https://www.youtube.com/@LoianeGroner
- DevDojo: https://www.youtube.com/@DevDojo
