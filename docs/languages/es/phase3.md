# Fase 3 – Persistencia de Datos y Streams (2–3 meses)

### SQL Básico
- **DDL**: `CREATE`, `ALTER`.  
- **DML**: `SELECT`, `INSERT`, `UPDATE`, `DELETE`.  
- **Joins**: `INNER`, `LEFT`, `RIGHT`.  
- **Keys**: claves primarias y foráneas.  
- **Normalization**: 1NF, 2NF, 3NF.  
- **Ejemplo**: crear tablas para productos y categorías.  

### JDBC y Connection Pool
- **Classes**: `Connection`, `Statement`, `PreparedStatement`, `ResultSet`.  
- Uso de Connection Pool (**HikariCP**).  
- **Mejores prácticas**: `try-with-resources`, manejo de `SQLException`.  

### Hibernate + JPA en la Práctica
- **Annotations**: `@Entity`, `@Id`, `@ManyToOne`, `@OneToMany`.  
- **Configuration**: `persistence.xml` o `application.properties`.  
- Operaciones **CRUD** con `EntityManager`.  
- Introducción a migraciones de base de datos con Flyway o Liquibase.

### Introducción a Bases de Datos NoSQL
- **Conceptos**: documentos, colecciones, escalabilidad horizontal.  
- **MongoDB**: configuración, operaciones CRUD con MongoRepository.  
- **Spring Data MongoDB**: integración con Spring Boot.  
- **Ejemplo**: almacenar logs de actividad del sistema para productos en MongoDB.

### Streams y Lambda Expressions
- **Operaciones**: `filter`, `map`, `sorted`, `collect`, `forEach`, `reduce`.  
- **Ejemplo**: filtrar productos por precio, ordenar por nombre.  

### Optional e Interfaces Funcionales
- `Optional`: `orElse`, `ifPresent`, `orElseThrow`.  
- **Functional interfaces**: `Function`, `Predicate`, `Consumer`.  
- **Ejemplo**: usar `Predicate` en Streams para filtrar datos.  

### Colecciones Avanzadas
- **LinkedList**: inserción/eliminación eficiente.  
- **TreeMap**: pares clave-valor ordenados.  
- **PriorityQueue**: cola de prioridad.  
- **LinkedHashMap** y **Deque** (introducción).  

### Logging (SLF4J/Logback)
- Configuración de SLF4J con Logback.  
- **Niveles**: `INFO`, `DEBUG`, `ERROR`.  
- **Ejemplo**: registrar queries de Hibernate.  

### Conceptos de Transacciones (ACID)
- Atomicidad, Consistencia, Aislamiento, Durabilidad.  
- Transacciones con JDBC (`commit`, `rollback`) y Hibernate (`@Transactional`).  

### Índices y Planes de Ejecución
- **Indexes**: primarios, únicos, compuestos.  
- Uso de **EXPLAIN** para optimizar queries.  
- **Ejemplo**: crear un índice en una columna de búsqueda frecuente.  

### Manipulación de Archivos (Opcional)
- Lectura y escritura con `Files`, `BufferedReader`.  
- **Ejemplo**: exportar un informe de productos a CSV usando Streams.  

### Pruebas con Bases de Datos (Introducción)
- Pruebas de integración con **H2** y **JUnit**.  
- **Ejemplo**: probar operaciones CRUD con Hibernate.  

### Proyecto Final
**Sistema de Gestión de Productos**  
- Base de datos: tablas **Product** y **Category** (relación 1:N).  
- Java: clases con JPA (`Product`, `Category`), CRUD con Hibernate.  
- **Opcional**: almacenar logs de cambios de productos en MongoDB.  
- **Opcional**: almacenar atributos dinámicos de productos (por ejemplo, especificaciones técnicas) en MongoDB.  
- Streams: filtrar/ordenar productos (por ejemplo, por precio o categoría).  
- Logging: monitorear operaciones de base de datos.  
- Git: commit por funcionalidad (por ejemplo, `feature/crud`, `feature/streams`).  
- Publicar en GitHub con README explicativo.  

### Recursos
- [SQLBolt](https://sqlbolt.com/)
- [PostgreSQL Official Docs](https://www.postgresql.org/docs/)  
- [Baeldung](https://www.baeldung.com/)  
- [Use The Index, Luke!](https://use-the-index-luke.com/)
- [Hibernate Official Docs](https://hibernate.org/orm/documentation/) 
- [Baeldung – Logging with SLF4J](https://www.baeldung.com/slf4j)
- [Flyway](https://flywaydb.org/)
- [MongoDB University](https://university.mongodb.com/)