# Phase 4 – Frameworks et Applications Web (3–4 mois)

### Spring Boot, Spring Core et Spring Data JPA
- **Spring Core** : Injection de dépendances (`@Bean`, `@Autowired`), conteneur IoC.  
- **Spring Boot** : Auto-configuration, starters (`spring-boot-starter-web`, `spring-boot-starter-data-jpa`), `application.yml`.  
- **Spring Data JPA** : Repositories (`CrudRepository`, `JpaRepository`), requêtes avec `@Query`, pagination.  
- **Exemple** : Créer des endpoints REST pour gérer des tâches (**CRUD**) dans une application de tâches.  

### Spring Security (JWT, OAuth2)
- **Concepts** : Authentification, autorisation, filtres de sécurité.  
- **JWT** : Créer et valider des tokens, utiliser `JwtAuthenticationFilter`.  
- **OAuth2** : Configurer un Resource Server, intégrer avec un fournisseur (par exemple, Google).  
- **Exemple** : Protéger les endpoints des tâches avec JWT et roles (`ADMIN`, `USER`).  

### Tests Unitaires et d’Intégration
- **Unit tests** : JUnit 5, Mockito (`@Mock`, `@InjectMocks`), tester la logique métier.  
- **Integration tests** : `@SpringBootTest`, `@WebMvcTest`, base de données **H2** pour les tests.  
- **Testcontainers** : Tester avec PostgreSQL dans des conteneurs Docker.  
- **Exemple** : Tester les services et endpoints de l’application de tâches.  

### APIs RESTful et Documentation avec Swagger
- **REST** : Méthodes HTTP, codes de statut, principes RESTful.  
- **Spring REST** : `@RestController`, `@RequestMapping`, `@PathVariable`.  
- **Swagger** : Configurer **springdoc-openapi**, annoter avec `@Operation`.  
- **Exemple** : Documenter les endpoints de l’application de tâches avec **Swagger UI**.  

### Introduction à GraphQL
- **Concepts** : Queries, mutations, schema.  
- **Spring Boot avec GraphQL** : Configuration avec spring-boot-starter-graphql.  
- **Exemple** : Créer une query GraphQL pour lister les tâches par statut.  

### Intégration Frontend de Base
- **Thymeleaf** : Templates pour rendre des pages HTML avec Spring Boot.  
- **Exemple** : Créer une interface web simple pour visualiser et créer des tâches.  

### Outils de Build : Maven et Gradle
- **Maven** : Structure du `pom.xml`, dépendances, plugins.  
- **Gradle** : Fichier `build.gradle`, tâches, gestion des dépendances.  
- **Exemple** : Configurer l’application de tâches avec Maven et Gradle.  

### Déploiement de Projet
- **Plateformes** : Railway, Heroku, AWS (Elastic Beanstalk).  
- **Étapes** : Empaqueter en JAR, configurer CI/CD avec GitHub Actions.  
- **Exemple** : Déployer l’application de tâches sur Railway avec PostgreSQL.  

### Projet Final
**Système de Gestion de Tâches**  
- Base de données : Tables `Task` (titre, description, statut) et `User` (relation 1:N).  
- Java : API REST avec Spring Boot, Spring Data JPA pour CRUD.  
- Sécurité : Authentification JWT, roles (`ADMIN`, `USER`).  
- Tests : Tests unitaires (services) et tests d’intégration (endpoints avec Testcontainers).  
- Documentation : Swagger UI avec descriptions des endpoints.  
- **Optionnel** : Ajouter une query GraphQL pour lister les tâches et une interface Thymeleaf pour l’interaction.  
- Git : Commits par fonctionnalité (par exemple, `feature/rest-api`, `feature/security`).  
- Publier : Sur GitHub avec un README (configuration, endpoints, déploiement).  

### Ressources
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