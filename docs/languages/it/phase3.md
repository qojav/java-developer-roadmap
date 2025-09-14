# Fase 3 – Persistenza dei Dati e Streams (2–3 mesi)

### SQL di Base
- **DDL**: `CREATE`, `ALTER`.  
- **DML**: `SELECT`, `INSERT`, `UPDATE`, `DELETE`.  
- **Joins**: `INNER`, `LEFT`, `RIGHT`.  
- **Keys**: chiavi primarie e chiavi esterne.  
- **Normalizzazione**: 1NF, 2NF, 3NF.  
- **Esempio**: creare tabelle per prodotti e categorie.  

### JDBC e Connection Pool
- **Classi**: `Connection`, `Statement`, `PreparedStatement`, `ResultSet`.  
- Uso di Connection Pool (**HikariCP**).  
- **Migliori pratiche**: `try-with-resources`, gestione di `SQLException`.  

### Hibernate + JPA nella Pratica
- **Annotazioni**: `@Entity`, `@Id`, `@ManyToOne`, `@OneToMany`.  
- **Configurazione**: `persistence.xml` o `application.properties`.  
- Operazioni **CRUD** con `EntityManager`.  
- Introduzione alle migrazioni di database con Flyway o Liquibase.

### Introduzione ai Database NoSQL
- **Concetti**: documents, collections, scalabilità orizzontale.  
- **MongoDB**: configurazione, operazioni CRUD con MongoRepository.  
- **Spring Data MongoDB**: integrazione con Spring Boot.  
- **Esempio**: memorizzare i log delle attività di sistema per i prodotti in MongoDB.

### Streams e Lambda Expressions
- **Operazioni**: `filter`, `map`, `sorted`, `collect`, `forEach`, `reduce`.  
- **Esempio**: filtrare i prodotti per prezzo, ordinare per nome.  

### Optional e Interfacce Funzionali
- `Optional`: `orElse`, `ifPresent`, `orElseThrow`.  
- **Interfacce funzionali**: `Function`, `Predicate`, `Consumer`.  
- **Esempio**: utilizzare `Predicate` negli Streams per filtrare i dati.  

### Collezioni Avanzate
- **LinkedList**: inserimento/rimozione efficiente.  
- **TreeMap**: coppie chiave-valore ordinate.  
- **PriorityQueue**: coda di priorità.  
- **LinkedHashMap** e **Deque** (introduzione).  

### Logging (SLF4J/Logback)
- Configurazione di SLF4J con Logback.  
- **Livelli**: `INFO`, `DEBUG`, `ERROR`.  
- **Esempio**: registrare le query di Hibernate.  

### Concetti di Transazione (ACID)
- Atomicità, Consistenza, Isolamento, Durabilità.  
- Transazioni con JDBC (`commit`, `rollback`) e Hibernate (`@Transactional`).  

### Indici e Piani di Esecuzione
- **Indici**: primari, unici, compositi.  
- Uso di **EXPLAIN** per ottimizzare le query.  
- **Esempio**: creare un indice su una colonna frequentemente ricercata.  

### Manipolazione dei File (Opzionale)
- Lettura e scrittura con `Files`, `BufferedReader`.  
- **Esempio**: esportare un report di prodotti in CSV utilizzando Streams.  

### Test di Database (Introduzione)
- Test di integrazione con **H2** e **JUnit**.  
- **Esempio**: testare le operazioni CRUD con Hibernate.  

### Progetto Finale
**Sistema di Gestione Prodotti**  
- Database: tabelle **Product** e **Category** (relazione 1:N).  
- Java: classi con JPA (`Product`, `Category`), CRUD con Hibernate.  
- **Opzionale**: memorizzare i log delle modifiche dei prodotti in MongoDB.  
- **Opzionale**: memorizzare attributi dinamici dei prodotti (es. specifiche tecniche) in MongoDB.  
- Streams: filtrare/ordinare i prodotti (es. per prezzo o categoria).  
- Logging: monitorare le operazioni sul database.  
- Git: commit per ogni funzionalità (es. `feature/crud`, `feature/streams`).  
- Pubblicazione su GitHub con README esplicativo.  

### Risorse
- [SQLBolt](https://sqlbolt.com/)
- [PostgreSQL Official Docs](https://www.postgresql.org/docs/)  
- [Baeldung](https://www.baeldung.com/)  
- [Use The Index, Luke!](https://use-the-index-luke.com/)
- [Hibernate Official Docs](https://hibernate.org/orm/documentation/) 
- [Baeldung – Logging with SLF4J](https://www.baeldung.com/slf4j)
- [Flyway](https://flywaydb.org/)
- [MongoDB University](https://university.mongodb.com/)