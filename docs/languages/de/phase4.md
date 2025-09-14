# Phase 4 – Frameworks und Webanwendungen (3–4 Monate)

### Spring Boot, Spring Core und Spring Data JPA
- **Spring Core**: Dependency Injection (`@Bean`, `@Autowired`), IoC Container.  
- **Spring Boot**: Auto-Configuration, Starters (`spring-boot-starter-web`, `spring-boot-starter-data-jpa`), `application.yml`.  
- **Spring Data JPA**: Repositories (`CrudRepository`, `JpaRepository`), Queries mit `@Query`, Paginierung.  
- **Beispiel**: Erstellen von REST Endpoints für die Verwaltung von Aufgaben (**CRUD**) in einer Task-App.  

### Spring Security (JWT, OAuth2)
- **Konzepte**: Authentication, Authorization, Security Filters.  
- **JWT**: Erstellen und Validieren von Tokens, Verwendung von `JwtAuthenticationFilter`.  
- **OAuth2**: Konfiguration eines Resource Servers, Integration mit einem Anbieter (z. B. Google).  
- **Beispiel**: Schützen von Task Endpoints mit JWT und Rollen (`ADMIN`, `USER`).  

### Unit- und Integrationstests
- **Unit Tests**: JUnit 5, Mockito (`@Mock`, `@InjectMocks`), Testen der Business Logic.  
- **Integration Tests**: `@SpringBootTest`, `@WebMvcTest`, **H2** Datenbank für Tests.  
- **Testcontainers**: Tests mit PostgreSQL in Docker-Containern.  
- **Beispiel**: Testen von Services und Endpoints der Task-App.  

### RESTful APIs und Dokumentation mit Swagger
- **REST**: HTTP-Methoden, Statuscodes, RESTful Prinzipien.  
- **Spring REST**: `@RestController`, `@RequestMapping`, `@PathVariable`.  
- **Swagger**: Konfiguration von **springdoc-openapi**, Annotation mit `@Operation`.  
- **Beispiel**: Dokumentation der Task-App Endpoints mit **Swagger UI**.  

### Einführung in GraphQL
- **Konzepte**: Queries, Mutations, Schema.  
- **Spring Boot mit GraphQL**: Einrichtung mit spring-boot-starter-graphql.  
- **Beispiel**: Erstellen einer GraphQL Query, um Aufgaben nach Status aufzulisten.  

### Grundlegende Frontend-Integration
- **Thymeleaf**: Templates zur Darstellung von HTML-Seiten mit Spring Boot.  
- **Beispiel**: Erstellen einer einfachen Web-Oberfläche zum Anzeigen und Erstellen von Aufgaben.  

### Build Tools: Maven und Gradle
- **Maven**: Struktur von `pom.xml`, Abhängigkeiten, Plugins.  
- **Gradle**: `build.gradle` Datei, Tasks, Dependency Management.  
- **Beispiel**: Konfiguration der Task-App mit Maven und Gradle.  

### Projektbereitstellung
- **Plattformen**: Railway, Heroku, AWS (Elastic Beanstalk).  
- **Schritte**: Verpacken als JAR, Konfiguration von CI/CD mit GitHub Actions.  
- **Beispiel**: Bereitstellung der Task-App auf Railway mit PostgreSQL.  

### Abschlussprojekt
**Task-Management-System**  
- Datenbank: `Task` (Titel, Beschreibung, Status) und `User` Tabellen (1:N-Beziehung).  
- Java: REST API mit Spring Boot, Spring Data JPA für CRUD.  
- Security: JWT Authentication, Rollen (`ADMIN`, `USER`).  
- Tests: Unit Tests (Services) und Integration Tests (Endpoints mit Testcontainers).  
- Dokumentation: Swagger UI mit Beschreibungen der Endpoints.  
- **Optional**: Hinzufügen einer GraphQL Query zum Auflisten von Aufgaben und einer Thymeleaf-Oberfläche für Interaktionen.  
- Git: Commits pro Feature (z. B. `feature/rest-api`, `feature/security`).  
- Veröffentlichung: Auf GitHub mit README (Setup, Endpoints, Bereitstellung).  

### Ressourcen
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