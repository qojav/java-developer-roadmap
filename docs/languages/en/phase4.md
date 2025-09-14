# Phase 4 – Frameworks and Web Applications (3–4 months)

### Spring Boot, Spring Core, and Spring Data JPA
- **Spring Core**: Dependency injection (`@Bean`, `@Autowired`), IoC container.  
- **Spring Boot**: Auto-configuration, starters (`spring-boot-starter-web`, `spring-boot-starter-data-jpa`), `application.yml`.  
- **Spring Data JPA**: Repositories (`CrudRepository`, `JpaRepository`), queries with `@Query`, pagination.  
- **Example**: Create REST endpoints for managing tasks (**CRUD**) in a task app.  

### Spring Security (JWT, OAuth2)
- **Concepts**: Authentication, authorization, security filters.  
- **JWT**: Create and validate tokens, use `JwtAuthenticationFilter`.  
- **OAuth2**: Configure Resource Server, integrate with a provider (e.g., Google).  
- **Example**: Protect task endpoints with JWT and roles (`ADMIN`, `USER`).  

### Unit and Integration Testing
- **Unit tests**: JUnit 5, Mockito (`@Mock`, `@InjectMocks`), test business logic.  
- **Integration tests**: `@SpringBootTest`, `@WebMvcTest`, **H2** database for testing.  
- **Testcontainers**: Test with PostgreSQL in Docker containers.  
- **Example**: Test services and endpoints of the task app.  

### RESTful APIs and Documentation with Swagger
- **REST**: HTTP methods, status codes, RESTful principles.  
- **Spring REST**: `@RestController`, `@RequestMapping`, `@PathVariable`.  
- **Swagger**: Configure **springdoc-openapi**, annotate with `@Operation`.  
- **Example**: Document task app endpoints with **Swagger UI**.  

### Introduction to GraphQL
- **Concepts**: Queries, mutations, schema.  
- **Spring Boot with GraphQL**: Setup with spring-boot-starter-graphql.  
- **Example**: Create a GraphQL query to list tasks by status.  

### Basic Frontend Integration
- **Thymeleaf**: Templates for rendering HTML pages with Spring Boot.  
- **Example**: Create a simple web interface to view and create tasks.  

### Build Tools: Maven and Gradle
- **Maven**: Structure of `pom.xml`, dependencies, plugins.  
- **Gradle**: `build.gradle` file, tasks, dependency management.  
- **Example**: Configure the task app with Maven and Gradle.  

### Project Deployment
- **Platforms**: Railway, Heroku, AWS (Elastic Beanstalk).  
- **Steps**: Package as JAR, configure CI/CD with GitHub Actions.  
- **Example**: Deploy the task app on Railway with PostgreSQL.  

### Final Project
**Task Management System**  
- Database: `Task` (title, description, status) and `User` tables (1:N relationship).  
- Java: REST API with Spring Boot, Spring Data JPA for CRUD.  
- Security: JWT authentication, roles (`ADMIN`, `USER`).  
- Tests: Unit tests (services) and integration tests (endpoints with Testcontainers).  
- Documentation: Swagger UI with endpoint descriptions.  
- **Optional**: Add a GraphQL query to list tasks and a Thymeleaf interface for interaction.  
- Git: Commits per feature (e.g., `feature/rest-api`, `feature/security`).  
- Publish: On GitHub with README (setup, endpoints, deployment).  

### Resources
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