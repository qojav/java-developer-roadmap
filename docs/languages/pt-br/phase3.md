# Fase 3 – Persistência de Dados e Streams (2–3 meses)

### SQL Básico
- **DDL**: `CREATE`, `ALTER`.  
- **DML**: `SELECT`, `INSERT`, `UPDATE`, `DELETE`.  
- **Joins**: `INNER`, `LEFT`, `RIGHT`.  
- **Chaves**: primárias e estrangeiras.  
- **Normalização**: 1NF, 2NF, 3NF.  
- **Exemplo**: criar tabelas para produtos e categorias.  

### JDBC e Connection Pool
- **Classes**: `Connection`, `Statement`, `PreparedStatement`, `ResultSet`.  
- Uso de Connection Pool (**HikariCP**).  
- **Boas práticas**: `try-with-resources`, tratamento de `SQLException`.  

### Hibernate + JPA na Prática
- **Anotações**: `@Entity`, `@Id`, `@ManyToOne`, `@OneToMany`.  
- **Configuração**: `persistence.xml` ou `application.properties`.  
- Operações **CRUD** com `EntityManager`.  
- Introdução a migrações de banco com Flyway ou Liquibase

### Introdução a Bancos NoSQL
- **Conceitos**: documentos, coleções, escalabilidade horizontal.
- **MongoDB**: configuração, operações CRUD com MongoRepository.
- **Spring Data MongoDB**: integração com Spring Boot.
- **Exemplo**: armazenar logs de atividades do sistema de produtos em MongoDB.

### Streams e Lambda Expressions
- **Operações**: `filter`, `map`, `sorted`, `collect`, `forEach`, `reduce`.  
- **Exemplo**: filtrar produtos por preço, ordenar por nome.  

### Optional e Functional Interfaces
- `Optional`: `orElse`, `ifPresent`, `orElseThrow`.  
- **Interfaces funcionais**: `Function`, `Predicate`, `Consumer`.  
- **Exemplo**: usar `Predicate` em Streams para filtrar dados.  

### Collections Avançadas
- **LinkedList**: inserção/remoção eficiente.  
- **TreeMap**: chave-valor ordenado.  
- **PriorityQueue**: fila de prioridade.  
- **LinkedHashMap** e **Deque** (introdução).  

### Logging (SLF4J/Logback)
- Configuração de SLF4J com Logback.  
- **Níveis**: `INFO`, `DEBUG`, `ERROR`.  
- **Exemplo**: log de queries do Hibernate.  

### Conceitos de Transações (ACID)
- Atomicidade, Consistência, Isolamento, Durabilidade.  
- Transações com JDBC (`commit`, `rollback`) e Hibernate (`@Transactional`).  

### Índices e Planos de Execução
- **Índices**: primários, únicos, compostos.  
- Uso de **EXPLAIN** para otimizar queries.  
- **Exemplo**: criar índice em coluna de busca frequente.  

### Manipulação de Arquivos (Opcional)
- Leitura e escrita com `Files`, `BufferedReader`.  
- **Exemplo**: exportar relatório de produtos para CSV usando Streams.  

### Testes com Banco de Dados (Introdução)
- Testes de integração com **H2** e **JUnit**.  
- **Exemplo**: testar operação CRUD com Hibernate.  

### Projeto Final
**Sistema de Gerenciamento de Produtos**  
- Banco: tabelas **Produto** e **Categoria** (relacionamento 1:N).  
- Java: classes com JPA (`Produto`, `Categoria`), CRUD com Hibernate. 
- **Opcional**: armazenar logs de alterações de produtos em MongoDB. 
- **Opcional**: armazenar atributos dinâmicos de produtos (ex.: especificações técnicas) em MongoDB.
- Streams: filtrar/ordenar produtos (ex.: por preço ou categoria).  
- Logging: monitorar operações no banco.  
- Git: commit por funcionalidade (ex.: `feature/crud`, `feature/streams`).  
- Publicar no GitHub com README explicativo.  

### Recursos
- [SQLBolt](https://sqlbolt.com/)
- [PostgreSQL Official Docs](https://www.postgresql.org/docs/)  
- [Baeldung](https://www.baeldung.com/)  
- [Use The Index, Luke!](https://use-the-index-luke.com/)
- [Hibernate Official Docs](https://hibernate.org/orm/documentation/) 
- [Baeldung – Logging com SLF4J](https://www.baeldung.com/slf4j)
- [Flyway](https://flywaydb.org/)
- [MongoDB University](https://university.mongodb.com/)