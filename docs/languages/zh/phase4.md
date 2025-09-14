# 第四阶段 – 框架与Web应用（3-4个月）

### Spring Boot、Spring Core 和 Spring Data JPA
- **Spring Core**: 依赖注入 (`@Bean`, `@Autowired`)，IoC容器。  
- **Spring Boot**: 自动配置，starters (`spring-boot-starter-web`, `spring-boot-starter-data-jpa`)，`application.yml`。  
- **Spring Data JPA**: 仓储 (`CrudRepository`, `JpaRepository`)，使用 `@Query` 进行查询，分页。  
- **示例**: 在任务应用中创建 REST endpoints 用于管理任务 (**CRUD**)。  

### Spring Security (JWT, OAuth2)
- **概念**: 认证、授权、安全过滤器。  
- **JWT**: 创建和验证 tokens，使用 `JwtAuthenticationFilter`。  
- **OAuth2**: 配置 Resource Server，与提供商集成（例如 Google）。  
- **示例**: 使用 JWT 和 roles (`ADMIN`, `USER`) 保护任务 endpoints。  

### 单元测试与集成测试
- **单元测试**: JUnit 5, Mockito (`@Mock`, `@InjectMocks`)，测试业务逻辑。  
- **集成测试**: `@SpringBootTest`, `@WebMvcTest`，使用 **H2** 数据库进行测试。  
- **Testcontainers**: 在 Docker 容器中使用 PostgreSQL 进行测试。  
- **示例**: 测试任务应用的服务和 endpoints。  

### RESTful APIs 与 Swagger 文档
- **REST**: HTTP 方法、状态码、RESTful 原则。  
- **Spring REST**: `@RestController`, `@RequestMapping`, `@PathVariable`。  
- **Swagger**: 配置 **springdoc-openapi**，使用 `@Operation` 注解。  
- **示例**: 使用 **Swagger UI** 文档化任务应用 endpoints。  

### GraphQL 介绍
- **概念**: Queries, mutations, schema。  
- **Spring Boot 与 GraphQL**: 使用 spring-boot-starter-graphql 进行设置。  
- **示例**: 创建一个 GraphQL query 以按状态列出任务。  

### 基础前端集成
- **Thymeleaf**: 使用 Spring Boot 渲染 HTML 页面模板。  
- **示例**: 创建一个简单的 Web 界面以查看和创建任务。  

### 构建工具：Maven 和 Gradle
- **Maven**: `pom.xml` 结构，依赖，插件。  
- **Gradle**: `build.gradle` 文件，任务，依赖管理。  
- **示例**: 使用 Maven 和 Gradle 配置任务应用。  

### 项目部署
- **平台**: Railway, Heroku, AWS (Elastic Beanstalk)。  
- **步骤**: 打包为 JAR，配置 CI/CD 使用 GitHub Actions。  
- **示例**: 在 Railway 上部署任务应用，结合 PostgreSQL。  

### 最终项目
**任务管理系统**  
- 数据库: `Task`（标题、描述、状态）和 `User` 表（1:N 关系）。  
- Java: 使用 Spring Boot 和 Spring Data JPA 实现 REST API 进行 CRUD。  
- 安全: JWT 认证，roles (`ADMIN`, `USER`)。  
- 测试: 单元测试（服务）和集成测试（使用 Testcontainers 测试 endpoints）。  
- 文档: 使用 Swagger UI 提供 endpoints 描述。  
- **可选**: 添加 GraphQL query 以列出任务，以及 Thymeleaf 界面用于交互。  
- Git: 按功能提交（例如，`feature/rest-api`, `feature/security`）。  
- 发布: 在 GitHub 上发布，附带 README（设置、endpoints、部署）。  

### 资源
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