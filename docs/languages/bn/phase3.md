# ফেজ ৩ – ডেটা পারসিস্টেন্স এবং স্ট্রিম (২-৩ মাস)

### মৌলিক SQL
- **DDL**: `CREATE`, `ALTER`.  
- **DML**: `SELECT`, `INSERT`, `UPDATE`, `DELETE`.  
- **Joins**: `INNER`, `LEFT`, `RIGHT`.  
- **Keys**: প্রাইমারি এবং ফরেন কী.  
- **Normalization**: 1NF, 2NF, 3NF.  
- **উদাহরণ**: প্রোডাক্ট এবং ক্যাটাগরির জন্য টেবিল তৈরি করা।  

### JDBC এবং Connection Pool
- **Classes**: `Connection`, `Statement`, `PreparedStatement`, `ResultSet`.  
- Connection Pool (**HikariCP**) এর ব্যবহার।  
- **সর্বোত্তম অনুশীলন**: `try-with-resources`, `SQLException` হ্যান্ডলিং।  

### Hibernate + JPA ব্যবহারিক প্রয়োগ
- **Annotations**: `@Entity`, `@Id`, `@ManyToOne`, `@OneToMany`.  
- **Configuration**: `persistence.xml` বা `application.properties`.  
- **CRUD** অপারেশন `EntityManager` দিয়ে।  
- Flyway বা Liquibase দিয়ে ডাটাবেস মাইগ্রেশনের পরিচিতি।

### NoSQL ডাটাবেসের পরিচিতি
- **ধারণা**: ডকুমেন্ট, কালেকশন, হরিজন্টাল স্কেলাবিলিটি।  
- **MongoDB**: সেটআপ, MongoRepository দিয়ে CRUD অপারেশন।  
- **Spring Data MongoDB**: Spring Boot এর সাথে ইন্টিগ্রেশন।  
- **উদাহরণ**: MongoDB-তে প্রোডাক্টের জন্য সিস্টেম অ্যাক্টিভিটি লগ সংরক্ষণ।

### Streams এবং Lambda Expressions
- **অপারেশন**: `filter`, `map`, `sorted`, `collect`, `forEach`, `reduce`.  
- **উদাহরণ**: দাম অনুযায়ী প্রোডাক্ট ফিল্টার করা, নাম অনুযায়ী সাজানো।  

### Optional এবং Functional Interfaces
- `Optional`: `orElse`, `ifPresent`, `orElseThrow`.  
- **Functional interfaces**: `Function`, `Predicate`, `Consumer`.  
- **উদাহরণ**: Streams-এ ডেটা ফিল্টার করতে `Predicate` ব্যবহার।  

### উন্নত কালেকশন
- **LinkedList**: দক্ষ ইনসার্শন/রিমুভাল।  
- **TreeMap**: সাজানো key-value পেয়ার।  
- **PriorityQueue**: প্রায়োরিটি কিউ।  
- **LinkedHashMap** এবং **Deque** (পরিচিতি)।  

### Logging (SLF4J/Logback)
- SLF4J এর সাথে Logback কনফিগারেশন।  
- **লেভেল**: `INFO`, `DEBUG`, `ERROR`.  
- **উদাহরণ**: Hibernate queries লগ করা।  

### ট্রানজাকশন ধারণা (ACID)
- অ্যাটমিসিটি, কনসিস্টেন্সি, আইসোলেশন, ডিউরাবিলিটি।  
- JDBC (`commit`, `rollback`) এবং Hibernate (`@Transactional`) দিয়ে ট্রানজাকশন।  

### ইনডেক্স এবং এক্সিকিউশন প্ল্যান
- **Indexes**: প্রাইমারি, ইউনিক, কম্পোজিট।  
- Queries অপটিমাইজ করতে **EXPLAIN** ব্যবহার।  
- **উদাহরণ**: ঘন ঘন সার্চ করা কলামে ইনডেক্স তৈরি করা।  

### ফাইল ম্যানিপুলেশন (ঐচ্ছিক)
- `Files`, `BufferedReader` দিয়ে পড়া এবং লেখা।  
- **উদাহরণ**: Streams ব্যবহার করে CSV ফরম্যাটে প্রোডাক্ট রিপোর্ট এক্সপোর্ট করা।  

### ডাটাবেস টেস্টিং (পরিচিতি)
- **H2** এবং **JUnit** দিয়ে ইন্টিগ্রেশন টেস্ট।  
- **উদাহরণ**: Hibernate দিয়ে CRUD অপারেশন টেস্ট করা।  

### চূড়ান্ত প্রকল্প
**প্রোডাক্ট ম্যানেজমেন্ট সিস্টেম**  
- ডাটাবেস: **Product** এবং **Category** টেবিল (1:N সম্পর্ক)।  
- Java: JPA (`Product`, `Category`) দিয়ে ক্লাস, Hibernate দিয়ে CRUD।  
- **ঐচ্ছিক**: MongoDB-তে প্রোডাক্ট পরিবর্তনের লগ সংরক্ষণ।  
- **ঐচ্ছিক**: MongoDB-তে প্রোডাক্টের ডায়নামিক অ্যাট্রিবিউট সংরক্ষণ (যেমন, টেকনিক্যাল স্পেসিফিকেশন)।  
- Streams: প্রোডাক্ট ফিল্টার/সর্ট করা (যেমন, দাম বা ক্যাটাগরি অনুযায়ী)।  
- Logging: ডাটাবেস অপারেশন পর্যবেক্ষণ।  
- Git: প্রতিটি ফিচারের জন্য commit (যেমন, `feature/crud`, `feature/streams`)।  
- GitHub-এ প্রকাশ সহ ব্যাখ্যামূলক README।  

### রিসোর্স
- [SQLBolt](https://sqlbolt.com/)
- [PostgreSQL Official Docs](https://www.postgresql.org/docs/)  
- [Baeldung](https://www.baeldung.com/)  
- [Use The Index, Luke!](https://use-the-index-luke.com/)
- [Hibernate Official Docs](https://hibernate.org/orm/documentation/) 
- [Baeldung – Logging with SLF4J](https://www.baeldung.com/slf4j)
- [Flyway](https://flywaydb.org/)
- [MongoDB University](https://university.mongodb.com/)