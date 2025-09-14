# Фаза 6 – Финальные проекты (постоянно)

### Проект 1: Полный CRUD с аутентификацией
- **Цель**: Создание надежного RESTful API с безопасной аутентификацией и тестированием.  
- **Технологии**: Spring Boot, Spring Data JPA (PostgreSQL), Spring Security (JWT), JUnit 5, Testcontainers.  
- **Функции**: CRUD для сущностей (например, задачи, пользователи), аутентификация с ролями (ADMIN, USER), документация с Swagger.  
- **Опционально**: Добавление интерфейса Thymeleaf для просмотра/управления задачами.  
- **Пример**: API для управления проектами (сущности: `Project`, `Task`, `User`) с защищенными эндпоинтами.  

### Проект 2: Загрузка файлов
- **Цель**: Добавление функциональности загрузки файлов в API из Проекта 1.  
- **Технологии**: Spring Boot (`MultipartFile`), Amazon S3 или локальное хранилище, валидация файлов.  
- **Функции**: Загрузка изображений/документов, связанных с задачами, проверка типа/размера.  
- **Пример**: Возможность загрузки вложений (например, PDF, PNG) для задач в API.  

### Проект 3: Развертывание в облаке
- **Цель**: Развертывание API на облачной платформе с CI/CD.  
- **Технологии**: Railway, Heroku или AWS (Elastic Beanstalk), GitHub Actions, Docker.  
- **Функции**: Упаковка в JAR/Docker, настройка переменных окружения, автоматизация развертывания.  
- **Опционально**: Реализация кэширования с Redis для оптимизации частых запросов.  
- **Пример**: Развертывание API проекта на Railway с PostgreSQL и CI/CD.  

### Проект 4: Микросервисы
- **Цель**: Разделение API из Проекта 1 на оркестрированные микросервисы.  
- **Технологии**: Spring Cloud (Eureka, Gateway), Docker Compose, REST для взаимодействия.  
- **Функции**: Микросервисы для `Tasks` и `Users` с обнаружением сервисов.  
- **Опционально**: Использование RabbitMQ для асинхронного взаимодействия между микросервисами.  
- **Пример**: Разделение логики задач и пользователей на два сервиса, оркестрированных с Docker.  

### Проект 5: Интеграция с внешним API
- **Цель**: Использование внешнего API для расширения функциональности.  
- **Технологии**: Spring RestTemplate или WebClient, аутентификация API (например, OAuth2).  
- **Функции**: Интеграция с публичным API (например, отправка уведомлений по email через SendGrid).  
- **Опционально**: Добавление GraphQL-запроса для получения задач/пользователей и хранения метаданных в MongoDB.  
- **Пример**: Добавление email-уведомлений о завершении задач.  

### Лучшие практики портфолио
- **Git**: Коммиты для каждой функции (например, `feature/crud`, `feature/upload`), четкие ветки.  
- **Документация**: README с описанием, настройкой, эндпоинтами, развертыванием и скриншотами.  
- **Публикация**: Размещение на GitHub с открытой лицензией (например, MIT).  

### Ресурсы
- [GitHub Guides](https://guides.github.com)  
- [Spring Boot Official Docs](https://spring.io/projects/spring-boot)  
- [Baeldung – Spring Boot Tutorials](https://www.baeldung.com)  
- [Spring Cloud Documentation](https://spring.io/projects/spring-cloud)  
- [Docker Official Docs](https://docs.docker.com)  
- [Railway Documentation](https://docs.railway.app)  
- [Heroku Dev Center](https://devcenter.heroku.com)  
- [AWS Elastic Beanstalk](https://docs.aws.amazon.com/elasticbeanstalk)  
- [SendGrid API Docs](https://docs.sendgrid.com)  
- [Awesome Open Source](https://awesomeopensource.com)  
- [Practical MongoDB Aggregations](https://university.mongodb.com/courses/MongoDB-Aggregations)