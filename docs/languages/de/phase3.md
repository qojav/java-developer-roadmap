# Phase 3 – Datenpersistenz und Streams (2–3 Monate)

### Grundlegendes SQL
- **DDL**: `CREATE`, `ALTER`.  
- **DML**: `SELECT`, `INSERT`, `UPDATE`, `DELETE`.  
- **Joins**: `INNER`, `LEFT`, `RIGHT`.  
- **Keys**: Primär- und Fremdschlüssel.  
- **Normalisierung**: 1NF, 2NF, 3NF.  
- **Beispiel**: Erstellen von Tabellen für Produkte und Kategorien.  

### JDBC und Connection Pool
- **Classes**: `Connection`, `Statement`, `PreparedStatement`, `ResultSet`.  
- Verwendung von Connection Pool (**HikariCP**).  
- **Best Practices**: `try-with-resources`, Umgang mit `SQLException`.  

### Hibernate + JPA in der Praxis
- **Annotations**: `@Entity`, `@Id`, `@ManyToOne`, `@OneToMany`.  
- **Konfiguration**: `persistence.xml` oder `application.properties`.  
- **CRUD**-Operationen mit `EntityManager`.  
- Einführung in Datenbankmigrationen mit Flyway oder Liquibase.

### Einführung in NoSQL-Datenbanken
- **Konzepte**: Dokumente, Sammlungen, horizontale Skalierbarkeit.  
- **MongoDB**: Einrichtung, CRUD-Operationen mit MongoRepository.  
- **Spring Data MongoDB**: Integration mit Spring Boot.  
- **Beispiel**: Speichern von Systemaktivitätslogs für Produkte in MongoDB.

### Streams und Lambda-Ausdrücke
- **Operationen**: `filter`, `map`, `sorted`, `collect`, `forEach`, `reduce`.  
- **Beispiel**: Produkte nach Preis filtern, nach Name sortieren.  

### Optional und Functional Interfaces
- `Optional`: `orElse`, `ifPresent`, `orElseThrow`.  
- **Functional Interfaces**: `Function`, `Predicate`, `Consumer`.  
- **Beispiel**: Verwendung von `Predicate` in Streams zum Filtern von Daten.  

### Fortgeschrittene Collections
- **LinkedList**: Effizientes Einfügen/Entfernen.  
- **TreeMap**: Geordnete Key-Value-Paare.  
- **PriorityQueue**: Prioritätswarteschlange.  
- **LinkedHashMap** und **Deque** (Einführung).  

### Logging (SLF4J/Logback)
- Konfiguration von SLF4J mit Logback.  
- **Level**: `INFO`, `DEBUG`, `ERROR`.  
- **Beispiel**: Protokollieren von Hibernate-Queries.  

### Transaktionskonzepte (ACID)
- Atomicity, Consistency, Isolation, Durability.  
- Transaktionen mit JDBC (`commit`, `rollback`) und Hibernate (`@Transactional`).  

### Indizes und Ausführungspläne
- **Indexes**: Primär, eindeutig, zusammengesetzt.  
- Verwendung von **EXPLAIN** zur Optimierung von Queries.  
- **Beispiel**: Erstellen eines Index für eine häufig durchsuchte Spalte.  

### Dateimanipulation (optional)
- Lesen und Schreiben mit `Files`, `BufferedReader`.  
- **Beispiel**: Exportieren eines Produktberichts nach CSV mit Streams.  

### Datenbanktests (Einführung)
- Integrationstests mit **H2** und **JUnit**.  
- **Beispiel**: Testen von CRUD-Operationen mit Hibernate.  

### Abschlussprojekt
**Produktmanagementsystem**  
- Datenbank: **Product**- und **Category**-Tabellen (1:N-Beziehung).  
- Java: Klassen mit JPA (`Product`, `Category`), CRUD mit Hibernate.  
- **Optional**: Speichern von Änderungslogs für Produkte in MongoDB.  
- **Optional**: Speichern dynamischer Produktattribute (z. B. technische Spezifikationen) in MongoDB.  
- Streams: Filtern/Sortieren von Produkten (z. B. nach Preis oder Kategorie).  
- Logging: Überwachung von Datenbankoperationen.  
- Git: Commit pro Feature (z. B. `feature/crud`, `feature/streams`).  
- Veröffentlichung auf GitHub mit erklärendem README.  

### Ressourcen
- [SQLBolt](https://sqlbolt.com/)
- [PostgreSQL Official Docs](https://www.postgresql.org/docs/)  
- [Baeldung](https://www.baeldung.com/)  
- [Use The Index, Luke!](https://use-the-index-luke.com/)
- [Hibernate Official Docs](https://hibernate.org/orm/documentation/) 
- [Baeldung – Logging with SLF4J](https://www.baeldung.com/slf4j)
- [Flyway](https://flywaydb.org/)
- [MongoDB University](https://university.mongodb.com/)