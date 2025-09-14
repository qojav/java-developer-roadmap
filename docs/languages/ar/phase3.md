# المرحلة 3 – استمرارية البيانات و Streams (2-3 أشهر)

### SQL الأساسي
- **DDL**: `CREATE`, `ALTER`.  
- **DML**: `SELECT`, `INSERT`, `UPDATE`, `DELETE`.  
- **Joins**: `INNER`, `LEFT`, `RIGHT`.  
- **Keys**: المفاتيح الأساسية والأجنبية.  
- **Normalization**: 1NF, 2NF, 3NF.  
- **مثال**: إنشاء جداول للمنتجات والفئات.  

### JDBC و Connection Pool
- **Classes**: `Connection`, `Statement`, `PreparedStatement`, `ResultSet`.  
- استخدام Connection Pool (**HikariCP**).  
- **أفضل الممارسات**: `try-with-resources`, التعامل مع `SQLException`.  

### Hibernate + JPA في التطبيق العملي
- **Annotations**: `@Entity`, `@Id`, `@ManyToOne`, `@OneToMany`.  
- **Configuration**: `persistence.xml` أو `application.properties`.  
- عمليات **CRUD** باستخدام `EntityManager`.  
- مقدمة إلى هجرة قواعد البيانات باستخدام Flyway أو Liquibase.

### مقدمة إلى قواعد البيانات NoSQL
- **المفاهيم**: المستندات، المجموعات، القابلية للتوسع الأفقي.  
- **MongoDB**: الإعداد، عمليات CRUD باستخدام MongoRepository.  
- **Spring Data MongoDB**: التكامل مع Spring Boot.  
- **مثال**: تخزين سجلات نشاط النظام للمنتجات في MongoDB.

### Streams و Lambda Expressions
- **العمليات**: `filter`, `map`, `sorted`, `collect`, `forEach`, `reduce`.  
- **مثال**: تصفية المنتجات حسب السعر، الفرز حسب الاسم.  

### Optional و Functional Interfaces
- `Optional`: `orElse`, `ifPresent`, `orElseThrow`.  
- **Functional interfaces**: `Function`, `Predicate`, `Consumer`.  
- **مثال**: استخدام `Predicate` في Streams لتصفية البيانات.  

### المجموعات المتقدمة
- **LinkedList**: الإدراج/الحذف بكفاءة.  
- **TreeMap**: أزواج مفتاح-قيمة مرتبة.  
- **PriorityQueue**: قائمة انتظار ذات أولوية.  
- **LinkedHashMap** و **Deque** (مقدمة).  

### Logging (SLF4J/Logback)
- تهيئة SLF4J مع Logback.  
- **المستويات**: `INFO`, `DEBUG`, `ERROR`.  
- **مثال**: تسجيل queries Hibernate.  

### مفاهيم المعاملات (ACID)
- الذرية، الاتساق، العزلة، المتانة.  
- المعاملات مع JDBC (`commit`, `rollback`) و Hibernate (`@Transactional`).  

### الفهارس وخطط التنفيذ
- **Indexes**: أساسي، فريد، مركب.  
- استخدام **EXPLAIN** لتحسين queries.  
- **مثال**: إنشاء فهرس على عمود يتم البحث فيه بشكل متكرر.  

### التعامل مع الملفات (اختياري)
- القراءة والكتابة باستخدام `Files`, `BufferedReader`.  
- **مثال**: تصدير تقرير المنتجات إلى CSV باستخدام Streams.  

### اختبار قواعد البيانات (مقدمة)
- اختبارات التكامل مع **H2** و **JUnit**.  
- **مثال**: اختبار عمليات CRUD مع Hibernate.  

### المشروع النهائي
**نظام إدارة المنتجات**  
- قاعدة البيانات: جداول **Product** و **Category** (علاقة 1:N).  
- Java: فئات مع JPA (`Product`, `Category`), CRUD مع Hibernate.  
- **اختياري**: تخزين سجلات تغييرات المنتجات في MongoDB.  
- **اختياري**: تخزين السمات الديناميكية للمنتجات (مثل المواصفات الفنية) في MongoDB.  
- Streams: تصفية/فرز المنتجات (مثل حسب السعر أو الفئة).  
- Logging: مراقبة عمليات قاعدة البيانات.  
- Git: commit لكل ميزة (مثال: `feature/crud`, `feature/streams`).  
- النشر على GitHub مع README توضيحي.  

### الموارد
- [SQLBolt](https://sqlbolt.com/)
- [PostgreSQL Official Docs](https://www.postgresql.org/docs/)  
- [Baeldung](https://www.baeldung.com/)  
- [Use The Index, Luke!](https://use-the-index-luke.com/)
- [Hibernate Official Docs](https://hibernate.org/orm/documentation/) 
- [Baeldung – Logging with SLF4J](https://www.baeldung.com/slf4j)
- [Flyway](https://flywaydb.org/)
- [MongoDB University](https://university.mongodb.com/)