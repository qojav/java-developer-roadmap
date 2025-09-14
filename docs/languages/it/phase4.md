# Fase 4 – Framework e Applicazioni Web (3–4 mesi)

### Spring Boot, Spring Core e Spring Data JPA
- **Spring Core**: Dependency injection (`@Bean`, `@Autowired`), IoC container.  
- **Spring Boot**: Auto-configurazione, starters (`spring-boot-starter-web`, `spring-boot-starter-data-jpa`), `application.yml`.  
- **Spring Data JPA**: Repositories (`CrudRepository`, `JpaRepository`), query con `@Query`, paginazione.  
- **Esempio**: Creare REST endpoints per la gestione delle attività (**CRUD**) in un'app di attività.  

### Spring Security (JWT, OAuth2)
- **Concetti**: Autenticazione, autorizzazione, filtri di sicurezza.  
- **JWT**: Creare e validare token, utilizzare `JwtAuthenticationFilter`.  
- **OAuth2**: Configurare Resource Server, integrare con un provider (es. Google).  
- **Esempio**: Proteggere gli endpoint delle attività con JWT e ruoli (`ADMIN`, `USER`).  

### Test Unitari e di Integrazione
- **Test unitari**: JUnit 5, Mockito (`@Mock`, `@InjectMocks`), test della logica di business.  
- **Test di integrazione**: `@SpringBootTest`, `@WebMvcTest`, database **H2** per i test.  
- **Testcontainers**: Test con PostgreSQL in container Docker.  
- **Esempio**: Testare i servizi e gli endpoint dell'app di attività.  

### API RESTful e Documentazione con Swagger
- **REST**: Metodi HTTP, codici di stato, principi RESTful.  
- **Spring REST**: `@RestController`, `@RequestMapping`, `@PathVariable`.  
- **Swagger**: Configurare **springdoc-openapi**, annotare con `@Operation`.  
- **Esempio**: Documentare gli endpoint dell'app di attività con **Swagger UI**.  

### Introduzione a GraphQL
- **Concetti**: Queries, mutations, schema.  
- **Spring Boot con GraphQL**: Configurazione con spring-boot-starter-graphql.  
- **Esempio**: Creare una query GraphQL per elencare le attività per stato.  

### Integrazione Frontend di Base
- **Thymeleaf**: Template per il rendering di pagine HTML con Spring Boot.  
- **Esempio**: Creare un'interfaccia web semplice per visualizzare e creare attività.  

### Strumenti di Build: Maven e Gradle
- **Maven**: Struttura di `pom.xml`, dipendenze, plugin.  
- **Gradle**: File `build.gradle`, attività, gestione delle dipendenze.  
- **Esempio**: Configurare l'app di attività con Maven e Gradle.  

### Distribuzione del Progetto
- **Piattaforme**: Railway, Heroku, AWS (Elastic Beanstalk).  
- **Passaggi**: Pacchettizzare come JAR, configurare CI/CD con GitHub Actions.  
- **Esempio**: Distribuire l'app di attività su Railway con PostgreSQL.  

### Progetto Finale
**Sistema di Gestione delle Attività**  
- Database: Tabelle `Task` (titolo, descrizione, stato) e `User` (relazione 1:N).  
- Java: REST API con Spring Boot, Spring Data JPA per CRUD.  
- Sicurezza: Autenticazione JWT, ruoli (`ADMIN`, `USER`).  
- Test: Test unitari (servizi) e test di integrazione (endpoint con Testcontainers).  
- Documentazione: Swagger UI con descrizioni degli endpoint.  
- **Opzionale**: Aggiungere una query GraphQL per elencare le attività e un'interfaccia Thymeleaf per l'interazione.  
- Git: Commit per ogni funzionalità (es. `feature/rest-api`, `feature/security`).  
- Pubblicazione: Su GitHub con README (configurazione, endpoint, distribuzione).  

### Risorse
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