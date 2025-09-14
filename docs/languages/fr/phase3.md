# Phase 3 – Persistance des Données et Streams (2–3 mois)

### SQL de Base
- **DDL** : `CREATE`, `ALTER`.  
- **DML** : `SELECT`, `INSERT`, `UPDATE`, `DELETE`.  
- **Joins** : `INNER`, `LEFT`, `RIGHT`.  
- **Keys** : clés primaires et étrangères.  
- **Normalization** : 1NF, 2NF, 3NF.  
- **Exemple** : créer des tables pour les produits et les catégories.  

### JDBC et Connection Pool
- **Classes** : `Connection`, `Statement`, `PreparedStatement`, `ResultSet`.  
- Utilisation de Connection Pool (**HikariCP**).  
- **Meilleures pratiques** : `try-with-resources`, gestion des `SQLException`.  

### Hibernate + JPA en Pratique
- **Annotations** : `@Entity`, `@Id`, `@ManyToOne`, `@OneToMany`.  
- **Configuration** : `persistence.xml` ou `application.properties`.  
- Opérations **CRUD** avec `EntityManager`.  
- Introduction aux migrations de base de données avec Flyway ou Liquibase.

### Introduction aux Bases de Données NoSQL
- **Concepts** : documents, collections, scalabilité horizontale.  
- **MongoDB** : configuration, opérations CRUD avec MongoRepository.  
- **Spring Data MongoDB** : intégration avec Spring Boot.  
- **Exemple** : stocker les journaux d’activité du système pour les produits dans MongoDB.

### Streams et Lambda Expressions
- **Opérations** : `filter`, `map`, `sorted`, `collect`, `forEach`, `reduce`.  
- **Exemple** : filtrer les produits par prix, trier par nom.  

### Optional et Functional Interfaces
- `Optional` : `orElse`, `ifPresent`, `orElseThrow`.  
- **Functional interfaces** : `Function`, `Predicate`, `Consumer`.  
- **Exemple** : utiliser `Predicate` dans Streams pour filtrer des données.  

### Collections Avancées
- **LinkedList** : insertion/suppression efficace.  
- **TreeMap** : paires clé-valeur ordonnées.  
- **PriorityQueue** : file de priorité.  
- **LinkedHashMap** et **Deque** (introduction).  

### Logging (SLF4J/Logback)
- Configuration de SLF4J avec Logback.  
- **Niveaux** : `INFO`, `DEBUG`, `ERROR`.  
- **Exemple** : enregistrer les queries Hibernate.  

### Concepts de Transactions (ACID)
- Atomicité, Cohérence, Isolation, Durabilité.  
- Transactions avec JDBC (`commit`, `rollback`) et Hibernate (`@Transactional`).  

### Index et Plans d’Exécution
- **Indexes** : primaires, uniques, composites.  
- Utilisation de **EXPLAIN** pour optimiser les queries.  
- **Exemple** : créer un index sur une colonne fréquemment recherchée.  

### Manipulation de Fichiers (Optionnel)
- Lecture et écriture avec `Files`, `BufferedReader`.  
- **Exemple** : exporter un rapport de produits au format CSV en utilisant Streams.  

### Tests de Base de Données (Introduction)
- Tests d’intégration avec **H2** et **JUnit**.  
- **Exemple** : tester les opérations CRUD avec Hibernate.  

### Projet Final
**Système de Gestion de Produits**  
- Base de données : tables **Product** et **Category** (relation 1:N).  
- Java : classes avec JPA (`Product`, `Category`), CRUD avec Hibernate.  
- **Optionnel** : stocker les journaux de modifications des produits dans MongoDB.  
- **Optionnel** : stocker les attributs dynamiques des produits (par exemple, spécifications techniques) dans MongoDB.  
- Streams : filtrer/trier les produits (par exemple, par prix ou catégorie).  
- Logging : surveiller les opérations de base de données.  
- Git : commit par fonctionnalité (par exemple, `feature/crud`, `feature/streams`).  
- Publier sur GitHub avec un README explicatif.  

### Ressources
- [SQLBolt](https://sqlbolt.com/)
- [PostgreSQL Official Docs](https://www.postgresql.org/docs/)  
- [Baeldung](https://www.baeldung.com/)  
- [Use The Index, Luke!](https://use-the-index-luke.com/)
- [Hibernate Official Docs](https://hibernate.org/orm/documentation/) 
- [Baeldung – Logging with SLF4J](https://www.baeldung.com/slf4j)
- [Flyway](https://flywaydb.org/)
- [MongoDB University](https://university.mongodb.com/)