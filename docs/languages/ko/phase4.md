# 4단계 – 프레임워크와 웹 애플리케이션 (3~4개월)

### Spring Boot, Spring Core, Spring Data JPA
- **Spring Core**: Dependency Injection (`@Bean`, `@Autowired`), IoC Container.  
- **Spring Boot**: Auto-Configuration, Starters (`spring-boot-starter-web`, `spring-boot-starter-data-jpa`), `application.yml`.  
- **Spring Data JPA**: Repositories (`CrudRepository`, `JpaRepository`), `@Query`를 사용한 쿼리, 페이지네이션.  
- **예제**: 태스크 앱에서 태스크를 관리하기 위한 REST endpoints 생성 (**CRUD**).  

### Spring Security (JWT, OAuth2)
- **개념**: Authentication, Authorization, Security Filters.  
- **JWT**: 토큰 생성 및 검증, `JwtAuthenticationFilter` 사용.  
- **OAuth2**: Resource Server 설정, 공급자(예: Google)와 통합.  
- **예제**: JWT와 롤(`ADMIN`, `USER`)로 태스크 endpoints 보호.  

### 유닛 및 통합 테스트
- **Unit Tests**: JUnit 5, Mockito (`@Mock`, `@InjectMocks`), 비즈니스 로직 테스트.  
- **Integration Tests**: `@SpringBootTest`, `@WebMvcTest`, 테스트용 **H2** 데이터베이스.  
- **Testcontainers**: Docker 컨테이너에서 PostgreSQL로 테스트.  
- **예제**: 태스크 앱의 서비스와 endpoints 테스트.  

### RESTful APIs와 Swagger를 사용한 문서화
- **REST**: HTTP 메서드, 상태 코드, RESTful 원칙.  
- **Spring REST**: `@RestController`, `@RequestMapping`, `@PathVariable`.  
- **Swagger**: **springdoc-openapi** 설정, `@Operation`으로 주석 추가.  
- **예제**: **Swagger UI**로 태스크 앱 endpoints 문서화.  

### GraphQL 소개
- **개념**: Queries, Mutations, Schema.  
- **Spring Boot with GraphQL**: spring-boot-starter-graphql로 설정.  
- **예제**: 상태별 태스크를 나열하는 GraphQL Query 생성.  

### 기본 프론트엔드 통합
- **Thymeleaf**: Spring Boot로 HTML 페이지를 렌더링하는 템플릿.  
- **예제**: 태스크를 보고 생성하는 간단한 웹 인터페이스 생성.  

### 빌드 도구: Maven과 Gradle
- **Maven**: `pom.xml` 구조, 의존성, 플러그인.  
- **Gradle**: `build.gradle` 파일, 태스크, 의존성 관리.  
- **예제**: Maven과 Gradle로 태스크 앱 설정.  

### 프로젝트 배포
- **플랫폼**: Railway, Heroku, AWS (Elastic Beanstalk).  
- **단계**: JAR로 패키징, GitHub Actions로 CI/CD 설정.  
- **예제**: PostgreSQL을 사용하여 Railway에 태스크 앱 배포.  

### 최종 프로젝트
**태스크 관리 시스템**  
- 데이터베이스: `Task` (제목, 설명, 상태) 및 `User` 테이블 (1:N 관계).  
- Java: Spring Boot, Spring Data JPA를 사용한 REST API로 CRUD.  
- 보안: JWT Authentication, 롤(`ADMIN`, `USER`).  
- 테스트: 유닛 테스트(서비스) 및 통합 테스트(Testcontainers를 사용한 endpoints).  
- 문서화: endpoints 설명이 포함된 Swagger UI.  
- **선택 사항**: 태스크 나열을 위한 GraphQL Query와 상호작용을 위한 Thymeleaf 인터페이스 추가.  
- Git: 기능별 commit (예: `feature/rest-api`, `feature/security`).  
- 공개: GitHub에 README(설정, endpoints, 배포)와 함께 공개.  

### 리소스
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