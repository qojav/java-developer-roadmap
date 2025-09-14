# Фаза 5 – Архитектура и конкурентность (2–3 месяца)

### Чистый код и принципы SOLID
- **Чистый код**: Понятные имена, короткие функции, полезные комментарии, единообразное форматирование.  
- **SOLID**:  
  - SRP (Single Responsibility Principle)  
  - OCP (Open/Closed Principle)  
  - LSP (Liskov Substitution Principle)  
  - ISP (Interface Segregation Principle)  
  - DIP (Dependency Inversion Principle)  

**Пример:** Рефакторинг сервиса в менеджере задач для соответствия принципам SOLID.  

### Шаблоны проектирования
- **Шаблоны**: Factory (создание), Singleton (единственный экземпляр), Builder (конструкция объектов), Strategy (поведение), Observer (события).  
- **Применение**: Выбор шаблонов, подходящих для контекста проекта.  

**Пример:** Использование Strategy для различных алгоритмов приоритизации задач.  

### Потоки и конкурентность
- **Концепции**: Thread, Runnable, ExecutorService, ForkJoinPool.  
- **Техники**: Создание и управление пулами потоков, асинхронные задачи.  

**Пример:** Параллельная обработка отчетов по задачам с помощью ExecutorService.  

### Синхронизация и проблемы конкурентности
- **Механизмы**: `synchronized`, `Lock`, `ReentrantLock`, `ConcurrentHashMap`.  
- **Проблемы**: Deadlock, race condition, starvation.  

**Пример:** Реализация безопасного доступа к общему списку задач.  

### Введение в микросервисы
- **Концепции**: Архитектура микросервисов, REST-взаимодействие, обнаружение сервисов.  
- **Инструменты**: Spring Cloud (например, Eureka для обнаружения сервисов).  

**Пример:** Разделение менеджера задач на микросервисы (задачи и пользователи).  

### Основы очередей сообщений (опционально)
- **Концепции**: Издатель/подписчик, очереди, топики.  
- **RabbitMQ**: Настройка, отправка и получение сообщений.  

**Пример:** Уведомление пользователей об обновлениях задач через RabbitMQ.  

### Оптимизация производительности
- **Кэширование**: Spring Cache с Redis для сокращения обращений к базе данных.  
- **Настройка JVM**: Основные концепции (heap, garbage collection).  

**Пример:** Реализация кэширования для частых запросов в системе задач.  

### Введение в DevOps/Cloud: Docker и CI/CD
- **Docker**: Контейнеры, образы, Dockerfile, Docker Compose.  
- **CI/CD**: Настройка конвейеров с GitHub Actions для сборки и развертывания.  

**Пример:** Создание Dockerfile для приложения задач и развертывание через GitHub Actions.  

### Наблюдаемость
- **Инструменты**: Prometheus (метрики), Grafana (визуализация), ELK Stack (логи).  
- **Концепции**: Мониторинг производительности, централизованные логи, оповещения.  

**Пример:** Мониторинг времени ответа API задач с помощью Prometheus и Grafana.  

### Безопасность: OWASP Top Ten
- **Концепции**: Инъекции, сбои аутентификации, утечка конфиденциальных данных.  
- **Практики**: Валидация ввода, санитизация, безопасная конфигурация.  

**Пример:** Защита API задач от SQL-инъекций и XSS.  

### Финальный проект
**Продвинутая система управления задачами**  
- Backend: Расширение API задач (Фаза 4) с микросервисами (задачи и пользователи).  
- Архитектура: Рефакторинг с использованием чистого кода, SOLID и шаблонов проектирования (например, Strategy).  
- Конкурентность: Параллельная обработка отчетов с помощью ExecutorService.  
- **Опционально**: Добавление взаимодействия микросервисов через RabbitMQ и кэширование с Redis для частых запросов.  
- DevOps: Упаковка в Docker, настройка CI/CD с GitHub Actions.  
- Наблюдаемость: Добавление Prometheus и Grafana для метрик.  
- Безопасность: Реализация защиты от OWASP Top Ten.  
- Git: Коммиты для каждой функции (например, `feature/microservices`, `feature/concurrency`).  
- Публикация: На GitHub с подробным README (настройка, архитектура, развертывание).  

### Ресурсы
- *The Pragmatic Programmer* (Книга)  
- *Effective Java* (Книга)  
- *Java Concurrency in Practice* (Книга)  
- [Spring Cloud Documentation](https://spring.io/projects/spring-cloud)  
- [RabbitMQ Tutorials](https://www.rabbitmq.com/getstarted.html)  
- [Redis University](https://university.redis.com/)  
- [Docker Official Docs](https://docs.docker.com/)  
- [Prometheus Documentation](https://prometheus.io/docs/introduction/overview/)  
- [Grafana Documentation](https://grafana.com/docs/)  
- [ELK Stack Guide](https://www.elastic.co/what-is/elk-stack)  
- [OWASP Top Ten](https://owasp.org/www-project-top-ten/)  
- [GitHub Actions Documentation](https://docs.github.com/en/actions)