# Фаза 4 – Фреймворки и веб-приложения (3–4 месяца)

### Spring Boot, Spring Core и Spring Data JPA
- **Spring Core**: Внедрение зависимостей (`@Bean`, `@Autowired`), IoC-контейнер.  
- **Spring Boot**: Автоконфигурация, стартеры (`spring-boot-starter-web`, `spring-boot-starter-data-jpa`), `application.yml`.  
- **Spring Data JPA**: Репозитории (`CrudRepository`, `JpaRepository`), запросы с `@Query`, пагинация.  
- **Пример**: Создание REST-эндпоинтов для управления задачами (**CRUD**) в приложении для задач.  

### Spring Security (JWT, OAuth2)
- **Концепции**: Аутентификация, авторизация, фильтры безопасности.  
- **JWT**: Создание и проверка токенов, использование `JwtAuthenticationFilter`.  
- **OAuth2**: Настройка Resource Server, интеграция с провайдером (например, Google).  
- **Пример**: Защита эндпоинтов задач с помощью JWT и ролей (`ADMIN`, `USER`).  

### Юнит- и интеграционное тестирование
- **Юнит-тесты**: JUnit 5, Mockito (`@Mock`, `@InjectMocks`), тестирование бизнес-логики.  
- **Интеграционные тесты**: `@SpringBootTest`, `@WebMvcTest`, база данных **H2** для тестирования.  
- **Testcontainers**: Тестирование с PostgreSQL в контейнерах Docker.  
- **Пример**: Тестирование сервисов и эндпоинтов приложения для задач.  

### RESTful API и документация с Swagger
- **REST**: HTTP-методы, коды состояния, принципы RESTful.  
- **Spring REST**: `@RestController`, `@RequestMapping`, `@PathVariable`.  
- **Swagger**: Настройка **springdoc-openapi**, аннотации с `@Operation`.  
- **Пример**: Документирование эндпоинтов приложения для задач с помощью **Swagger UI**.  

### Введение в GraphQL
- **Концепции**: Запросы, мутации, схема.  
- **Spring Boot с GraphQL**: Настройка с spring-boot-starter-graphql.  
- **Пример**: Создание GraphQL-запроса для получения списка задач по статусу.  

### Базовая интеграция фронтенда
- **Thymeleaf**: Шаблоны для рендеринга HTML-страниц с Spring Boot.  
- **Пример**: Создание простого веб-интерфейса для просмотра и создания задач.  

### Инструменты сборки: Maven и Gradle
- **Maven**: Структура `pom.xml`, зависимости, плагины.  
- **Gradle**: Файл `build.gradle`, задачи, управление зависимостями.  
- **Пример**: Настройка приложения для задач с Maven и Gradle.  

### Развертывание проекта
- **Платформы**: Railway, Heroku, AWS (Elastic Beanstalk).  
- **Шаги**: Упаковка в JAR, настройка CI/CD с GitHub Actions.  
- **Пример**: Развертывание приложения для задач на Railway с PostgreSQL.  

### Финальный проект
**Система управления задачами**  
- База данных: Таблицы `Task` (заголовок, описание, статус) и `User` (отношение 1:N).  
- Java: REST API с Spring Boot, Spring Data JPA для CRUD.  
- Безопасность: JWT-аутентификация, роли (`ADMIN`, `USER`).  
- Тесты: Юнит-тесты (сервисы) и интеграционные тесты (эндпоинты с Testcontainers).  
- Документация: Swagger UI с описанием эндпоинтов.  
- **Опционально**: Добавление GraphQL-запроса для получения списка задач и интерфейса Thymeleaf для взаимодействия.  
- Git: Коммиты для каждой функции (например, `feature/rest-api`, `feature/security`).  
- Публикация: На GitHub с README (настройка, эндпоинты, развертывание).  

### Ресурсы
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