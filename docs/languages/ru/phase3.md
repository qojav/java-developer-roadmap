# Фаза 3 – Сохранение данных и потоки (2–3 месяца)

### Основы SQL
- **DDL**: `CREATE`, `ALTER`.  
- **DML**: `SELECT`, `INSERT`, `UPDATE`, `DELETE`.  
- **Joins**: `INNER`, `LEFT`, `RIGHT`.  
- **Keys**: первичные и внешние ключи.  
- **Нормализация**: 1NF, 2NF, 3NF.  
- **Пример**: создание таблиц для продуктов и категорий.  

### JDBC и пул соединений
- **Классы**: `Connection`, `Statement`, `PreparedStatement`, `ResultSet`.  
- Использование пула соединений (**HikariCP**).  
- **Лучшие практики**: `try-with-resources`, обработка `SQLException`.  

### Hibernate + JPA на практике
- **Аннотации**: `@Entity`, `@Id`, `@ManyToOne`, `@OneToMany`.  
- **Конфигурация**: `persistence.xml` или `application.properties`.  
- **CRUD**-операции с `EntityManager`.  
- Введение в миграции баз данных с Flyway или Liquibase.

### Введение в NoSQL базы данных
- **Концепции**: документы, коллекции, горизонтальная масштабируемость.  
- **MongoDB**: настройка, CRUD-операции с MongoRepository.  
- **Spring Data MongoDB**: интеграция с Spring Boot.  
- **Пример**: хранение логов активности системы для продуктов в MongoDB.

### Потоки и лямбда-выражения
- **Операции**: `filter`, `map`, `sorted`, `collect`, `forEach`, `reduce`.  
- **Пример**: фильтрация продуктов по цене, сортировка по названию.  

### Optional и функциональные интерфейсы
- `Optional`: `orElse`, `ifPresent`, `orElseThrow`.  
- **Функциональные интерфейсы**: `Function`, `Predicate`, `Consumer`.  
- **Пример**: использование `Predicate` в Streams для фильтрации данных.  

### Продвинутые коллекции
- **LinkedList**: эффективная вставка/удаление.  
- **TreeMap**: упорядоченные пары ключ-значение.  
- **PriorityQueue**: очередь с приоритетом.  
- **LinkedHashMap** и **Deque** (введение).  

### Логирование (SLF4J/Logback)
- Конфигурация SLF4J с Logback.  
- **Уровни**: `INFO`, `DEBUG`, `ERROR`.  
- **Пример**: логирование запросов Hibernate.  

### Концепции транзакций (ACID)
- Атомарность, согласованность, изолированность, долговечность.  
- Транзакции с JDBC (`commit`, `rollback`) и Hibernate (`@Transactional`).  

### Индексы и планы выполнения
- **Индексы**: первичные, уникальные, составные.  
- Использование **EXPLAIN** для оптимизации запросов.  
- **Пример**: создание индекса для часто запрашиваемого столбца.  

### Работа с файлами (опционально)
- Чтение и запись с помощью `Files`, `BufferedReader`.  
- **Пример**: экспорт отчета о продуктах в CSV с использованием Streams.  

### Тестирование баз данных (введение)
- Интеграционные тесты с **H2** и **JUnit**.  
- **Пример**: тестирование CRUD-операций с Hibernate.  

### Финальный проект
**Система управления продуктами**  
- База данных: таблицы **Product** и **Category** (отношение 1:N).  
- Java: классы с JPA (`Product`, `Category`), CRUD с Hibernate.  
- **Опционально**: хранение логов изменений продуктов в MongoDB.  
- **Опционально**: хранение динамических атрибутов продуктов (например, технических характеристик) в MongoDB.  
- Streams: фильтрация/сортировка продуктов (например, по цене или категории).  
- Логирование: мониторинг операций с базой данных.  
- Git: коммит для каждой функции (например, `feature/crud`, `feature/streams`).  
- Публикация на GitHub с поясняющим README.  

### Ресурсы
- [SQLBolt](https://sqlbolt.com/)
- [PostgreSQL Official Docs](https://www.postgresql.org/docs/)  
- [Baeldung](https://www.baeldung.com/)  
- [Use The Index, Luke!](https://use-the-index-luke.com/)
- [Hibernate Official Docs](https://hibernate.org/orm/documentation/) 
- [Baeldung – Logging with SLF4J](https://www.baeldung.com/slf4j)
- [Flyway](https://flywaydb.org/)
- [MongoDB University](https://university.mongodb.com/)