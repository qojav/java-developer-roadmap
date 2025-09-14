# चरण 3 – डेटा पर्सिस्टेंस और स्ट्रीम्स (2-3 महीने)

### मूल SQL
- **DDL**: `CREATE`, `ALTER`.  
- **DML**: `SELECT`, `INSERT`, `UPDATE`, `DELETE`.  
- **Joins**: `INNER`, `LEFT`, `RIGHT`.  
- **Keys**: प्राइमरी और फॉरेन कीज़।  
- **नॉर्मलाइजेशन**: 1NF, 2NF, 3NF।  
- **उदाहरण**: प्रोडक्ट्स और कैटेगरीज के लिए टेबल बनाना।  

### JDBC और Connection Pool
- **Classes**: `Connection`, `Statement`, `PreparedStatement`, `ResultSet`.  
- Connection Pool (**HikariCP**) का उपयोग।  
- **सर्वोत्तम अभ्यास**: `try-with-resources`, `SQLException` का प्रबंधन।  

### Hibernate + JPA व्यवहार में
- **Annotations**: `@Entity`, `@Id`, `@ManyToOne`, `@OneToMany`.  
- **कॉन्फ़िगरेशन**: `persistence.xml` या `application.properties`.  
- `EntityManager` के साथ **CRUD** ऑपरेशन्स।  
- Flyway या Liquibase के साथ डेटाबेस माइग्रेशन्स का परिचय।

### NoSQL डेटाबेस का परिचय
- **अवधारणाएँ**: दस्तावेज़, कलेक्शन्स, हॉरिजॉन्टल स्केलेबिलिटी।  
- **MongoDB**: सेटअप, MongoRepository के साथ CRUD ऑपरेशन्स।  
- **Spring Data MongoDB**: Spring Boot के साथ एकीकरण।  
- **उदाहरण**: MongoDB में प्रोडक्ट्स के लिए सिस्टम गतिविधि लॉग्स स्टोर करना।

### स्ट्रीम्स और लैम्ब्डा एक्सप्रेशन्स
- **ऑपरेशन्स**: `filter`, `map`, `sorted`, `collect`, `forEach`, `reduce`.  
- **उदाहरण**: कीमत के आधार पर प्रोडक्ट्स को फ़िल्टर करना, नाम के आधार पर सॉर्ट करना।  

### Optional और Functional Interfaces
- `Optional`: `orElse`, `ifPresent`, `orElseThrow`.  
- **Functional Interfaces**: `Function`, `Predicate`, `Consumer`.  
- **उदाहरण**: स्ट्रीम्स में डेटा फ़िल्टर करने के लिए `Predicate` का उपयोग।  

### उन्नत कलेक्शन्स
- **LinkedList**: कुशलतापूर्वक जोड़ना/हटाना।  
- **TreeMap**: क्रमबद्ध key-value जोड़े।  
- **PriorityQueue**: प्रायोरिटी क्यू।  
- **LinkedHashMap** और **Deque** (परिचय)।  

### लॉगिंग (SLF4J/Logback)
- SLF4J के साथ Logback का कॉन्फ़िगरेशन।  
- **लेवल्स**: `INFO`, `DEBUG`, `ERROR`.  
- **उदाहरण**: Hibernate क्वेरीज़ को लॉग करना।  

### ट्रांजेक्शन अवधारणाएँ (ACID)
- परमाणुकता, संगतता, अलगाव, स्थायित्व।  
- JDBC (`commit`, `rollback`) और Hibernate (`@Transactional`) के साथ ट्रांजेक्शन्स।  

### इंडेक्स और एक्जीक्यूशन प्लान्स
- **Indexes**: प्राइमरी, यूनिक, कम्पोजिट।  
- क्वेरीज़ को अनुकूलित करने के लिए **EXPLAIN** का उपयोग।  
- **उदाहरण**: बार-बार खोजी जाने वाली कॉलम पर इंडेक्स बनाना।  

### फाइल मैनिपुलेशन (वैकल्पिक)
- `Files`, `BufferedReader` के साथ पढ़ना और लिखना।  
- **उदाहरण**: स्ट्रीम्स का उपयोग करके CSV में प्रोडक्ट रिपोर्ट निर्यात करना।  

### डेटाबेस टेस्टिंग (परिचय)
- **H2** और **JUnit** के साथ इंटीग्रेशन टेस्ट्स।  
- **उदाहरण**: Hibernate के साथ CRUD ऑपरेशन्स का टेस्ट करना।  

### अंतिम प्रोजेक्ट
**प्रोडक्ट मैनेजमेंट सिस्टम**  
- डेटाबेस: **Product** और **Category** टेबल्स (1:N संबंध)।  
- Java: JPA (`Product`, `Category`) के साथ क्लासेस, Hibernate के साथ CRUD।  
- **वैकल्पिक**: MongoDB में प्रोडक्ट परिवर्तन लॉग्स स्टोर करना।  
- **वैकल्पिक**: MongoDB में डायनामिक प्रोडक्ट विशेषताएँ (उदाहरण के लिए, तकनीकी विनिर्देश) स्टोर करना।  
- स्ट्रीम्स: प्रोडक्ट्स को फ़िल्टर/सॉर्ट करना (उदाहरण के लिए, कीमत या कैटेगरी के आधार पर)।  
- लॉगिंग: डेटाबेस ऑपरेशन्स की निगरानी।  
- Git: प्रत्येक फीचर के लिए commit (उदाहरण के लिए, `feature/crud`, `feature/streams`)।  
- GitHub पर प्रकाशन के साथ व्याख्यात्मक README।  

### संसाधन
- [SQLBolt](https://sqlbolt.com/)
- [PostgreSQL Official Docs](https://www.postgresql.org/docs/)  
- [Baeldung](https://www.baeldung.com/)  
- [Use The Index, Luke!](https://use-the-index-luke.com/)
- [Hibernate Official Docs](https://hibernate.org/orm/documentation/) 
- [Baeldung – Logging with SLF4J](https://www.baeldung.com/slf4j)
- [Flyway](https://flywaydb.org/)
- [MongoDB University](https://university.mongodb.com/)