# Fase 4 – Frameworks e Aplicações Web (3–4 meses)

### Spring Boot, Spring Core e Spring Data JPA
- **Spring Core**: Injeção de dependência (`@Bean`, `@Autowired`), contêiner IoC.  
- **Spring Boot**: Autoconfiguração, starters (`spring-boot-starter-web`, `spring-boot-starter-data-jpa`), `application.yml`.  
- **Spring Data JPA**: Repositórios (`CrudRepository`, `JpaRepository`), consultas com `@Query`, paginação.  
- **Exemplo**: Criar endpoints REST para gerenciar tarefas (**CRUD**) em um app de tarefas.  

### Spring Security (JWT, OAuth2)
- **Conceitos**: autenticação, autorização, filtros de segurança.  
- **JWT**: criar e validar tokens, usar `JwtAuthenticationFilter`.  
- **OAuth2**: configurar Resource Server, integrar com provedor (ex.: Google).  
- **Exemplo**: proteger endpoints de tarefas com JWT e papéis (`ADMIN`, `USER`).  

### Testes Unitários e de Integração
- **Unitários**: JUnit 5, Mockito (`@Mock`, `@InjectMocks`), testar lógica de negócio.  
- **Integração**: `@SpringBootTest`, `@WebMvcTest`, banco **H2** para testes.  
- **Testcontainers**: testar com PostgreSQL em contêineres Docker.  
- **Exemplo**: testar serviços e endpoints do app de tarefas.  

### APIs RESTful e Documentação com Swagger
- **REST**: métodos HTTP, códigos de status, princípios RESTful.  
- **Spring REST**: `@RestController`, `@RequestMapping`, `@PathVariable`.  
- **Swagger**: configurar **springdoc-openapi**, anotar com `@Operation`.  
- **Exemplo**: documentar endpoints do app de tarefas com **Swagger UI**.  

### Introdução ao GraphQL
- **Conceitos**: queries, mutations, schema.
- **Spring Boot com GraphQL**: configuração com spring-boot-starter-graphql.
- **Exemplo**: criar uma query GraphQL para listar tarefas por status.

### Integração Básica com Frontend
- **Thymeleaf**: templates para renderizar páginas HTML com Spring Boot.
- **Exemplo**: criar uma interface web simples para visualizar e criar tarefas.

### Ferramentas de Build: Maven e Gradle
- **Maven**: estrutura do `pom.xml`, dependências, plugins.  
- **Gradle**: arquivo `build.gradle`, tarefas, gerenciamento de dependências.  
- **Exemplo**: configurar o app de tarefas com Maven e Gradle.  

### Deploy de Projeto
- **Plataformas**: Railway, Heroku, AWS (Elastic Beanstalk).  
- **Passos**: empacotar como JAR, configurar CI/CD com GitHub Actions.  
- **Exemplo**: fazer deploy do app de tarefas no Railway com PostgreSQL.  

### Projeto Final
**Sistema de Gerenciamento de Tarefas**  
- Banco: tabelas `Task` (título, descrição, status) e `User` (relacionamento 1:N).  
- Java: API REST com Spring Boot, Spring Data JPA para CRUD.  
- Segurança: autenticação JWT, papéis (`ADMIN`, `USER`).  
- Testes: unitários (serviços) e integração (endpoints com Testcontainers).  
- Documentação: Swagger UI com descrição de endpoints.  
- **Opcional**: adicionar uma query GraphQL para listar tarefas e uma interface Thymeleaf para interação.
- Git: commits por funcionalidade (ex.: `feature/rest-api`, `feature/security`).  
- Publicar: no GitHub com README (setup, endpoints, deploy).  

### Recursos
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
