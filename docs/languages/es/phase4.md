# Fase 4 – Frameworks y Aplicaciones Web (3–4 meses)

### Spring Boot, Spring Core y Spring Data JPA
- **Spring Core**: Inyección de dependencias (`@Bean`, `@Autowired`), contenedor IoC.  
- **Spring Boot**: Autoconfiguración, starters (`spring-boot-starter-web`, `spring-boot-starter-data-jpa`), `application.yml`.  
- **Spring Data JPA**: Repositorios (`CrudRepository`, `JpaRepository`), consultas con `@Query`, paginación.  
- **Ejemplo**: Crear endpoints REST para gestionar tareas (**CRUD**) en una aplicación de tareas.  

### Spring Security (JWT, OAuth2)
- **Conceptos**: Autenticación, autorización, filtros de seguridad.  
- **JWT**: Crear y validar tokens, usar `JwtAuthenticationFilter`.  
- **OAuth2**: Configurar Resource Server, integrar con un proveedor (por ejemplo, Google).  
- **Ejemplo**: Proteger endpoints de tareas con JWT y roles (`ADMIN`, `USER`).  

### Pruebas Unitarias e Integración
- **Pruebas unitarias**: JUnit 5, Mockito (`@Mock`, `@InjectMocks`), probar lógica de negocio.  
- **Pruebas de integración**: `@SpringBootTest`, `@WebMvcTest`, base de datos **H2** para pruebas.  
- **Testcontainers**: Probar con PostgreSQL en contenedores Docker.  
- **Ejemplo**: Probar servicios y endpoints de la aplicación de tareas.  

### APIs RESTful y Documentación con Swagger
- **REST**: Métodos HTTP, códigos de estado, principios RESTful.  
- **Spring REST**: `@RestController`, `@RequestMapping`, `@PathVariable`.  
- **Swagger**: Configurar **springdoc-openapi**, anotar con `@Operation`.  
- **Ejemplo**: Documentar endpoints de la aplicación de tareas con **Swagger UI**.  

### Introducción a GraphQL
- **Conceptos**: Queries, mutations, schema.  
- **Spring Boot con GraphQL**: Configuración con spring-boot-starter-graphql.  
- **Ejemplo**: Crear una query GraphQL para listar tareas por estado.  

### Integración Básica con Frontend
- **Thymeleaf**: Plantillas para renderizar páginas HTML con Spring Boot.  
- **Ejemplo**: Crear una interfaz web simple para visualizar y crear tareas.  

### Herramientas de Build: Maven y Gradle
- **Maven**: Estructura de `pom.xml`, dependencias, plugins.  
- **Gradle**: Archivo `build.gradle`, tareas, gestión de dependencias.  
- **Ejemplo**: Configurar la aplicación de tareas con Maven y Gradle.  

### Despliegue de Proyecto
- **Plataformas**: Railway, Heroku, AWS (Elastic Beanstalk).  
- **Pasos**: Empaquetar como JAR, configurar CI/CD con GitHub Actions.  
- **Ejemplo**: Desplegar la aplicación de tareas en Railway con PostgreSQL.  

### Proyecto Final
**Sistema de Gestión de Tareas**  
- Base de datos: Tablas `Task` (título, descripción, estado) y `User` (relación 1:N).  
- Java: API REST con Spring Boot, Spring Data JPA para CRUD.  
- Seguridad: Autenticación JWT, roles (`ADMIN`, `USER`).  
- Pruebas: Pruebas unitarias (servicios) y de integración (endpoints con Testcontainers).  
- Documentación: Swagger UI con descripciones de endpoints.  
- **Opcional**: Agregar una query GraphQL para listar tareas y una interfaz Thymeleaf para interacción.  
- Git: Commits por funcionalidad (por ejemplo, `feature/rest-api`, `feature/security`).  
- Publicar: En GitHub con README (configuración, endpoints, despliegue).  

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