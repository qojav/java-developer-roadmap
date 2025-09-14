# Faz 3 – Veri Kalıcılığı ve Akışlar (2–3 ay)

### Temel SQL
- **DDL**: `CREATE`, `ALTER`.  
- **DML**: `SELECT`, `INSERT`, `UPDATE`, `DELETE`.  
- **Joins**: `INNER`, `LEFT`, `RIGHT`.  
- **Keys**: primary ve foreign keys.  
- **Normalization**: 1NF, 2NF, 3NF.  
- **Örnek**: ürünler ve kategoriler için tablolar oluşturma.  

### JDBC ve Connection Pool
- **Sınıflar**: `Connection`, `Statement`, `PreparedStatement`, `ResultSet`.  
- Connection Pool kullanımı (**HikariCP**).  
- **En iyi uygulamalar**: `try-with-resources`, `SQLException` yönetimi.  

### Hibernate + JPA Uygulamada
- **Annotations**: `@Entity`, `@Id`, `@ManyToOne`, `@OneToMany`.  
- **Konfigürasyon**: `persistence.xml` veya `application.properties`.  
- **CRUD** işlemleri `EntityManager` ile.  
- Flyway veya Liquibase ile veritabanı göçlerine giriş.

### NoSQL Veritabanlarına Giriş
- **Kavramlar**: belgeler, koleksiyonlar, yatay ölçeklenebilirlik.  
- **MongoDB**: kurulum, MongoRepository ile CRUD işlemleri.  
- **Spring Data MongoDB**: Spring Boot ile entegrasyon.  
- **Örnek**: ürünlerle ilgili sistem etkinlik günlüklerini MongoDB’de saklama.

### Akışlar ve Lambda İfadeleri
- **İşlemler**: `filter`, `map`, `sorted`, `collect`, `forEach`, `reduce`.  
- **Örnek**: ürünleri fiyata göre filtreleme, isme göre sıralama.  

### Optional ve Fonksiyonel Arayüzler
- `Optional`: `orElse`, `ifPresent`, `orElseThrow`.  
- **Fonksiyonel arayüzler**: `Function`, `Predicate`, `Consumer`.  
- **Örnek**: verileri filtrelemek için Streams’te `Predicate` kullanma.  

### Gelişmiş Koleksiyonlar
- **LinkedList**: verimli ekleme/çıkarma.  
- **TreeMap**: sıralı anahtar-değer çiftleri.  
- **PriorityQueue**: öncelik kuyruğu.  
- **LinkedHashMap** ve **Deque** (giriş).  

### Günlük Kaydı (SLF4J/Logback)
- SLF4J ve Logback konfigürasyonu.  
- **Seviyeler**: `INFO`, `DEBUG`, `ERROR`.  
- **Örnek**: Hibernate sorgularını günlüğe kaydetme.  

### İşlem Kavramları (ACID)
- Atomiklik, Tutarlılık, İzolasyon, Dayanıklılık.  
- JDBC ile işlemler (`commit`, `rollback`) ve Hibernate ile (`@Transactional`).  

### İndeksler ve Yürütme Planları
- **İndeksler**: primary, unique, composite.  
- Sorguları optimize etmek için **EXPLAIN** kullanımı.  
- **Örnek**: sık aranan bir sütunda indeks oluşturma.  

### Dosya Manipülasyonu (Opsiyonel)
- `Files`, `BufferedReader` ile okuma ve yazma.  
- **Örnek**: Streams kullanarak ürün raporunu CSV’ye dışa aktarma.  

### Veritabanı Testi (Giriş)
- **H2** ve **JUnit** ile entegrasyon testleri.  
- **Örnek**: Hibernate ile CRUD işlemlerini test etme.  

### Final Projesi
**Ürün Yönetim Sistemi**  
- Veritabanı: **Product** ve **Category** tabloları (1:N ilişkisi).  
- Java: JPA ile sınıflar (`Product`, `Category`), Hibernate ile CRUD.  
- **Opsiyonel**: ürün değişim günlüklerini MongoDB’de saklama.  
- **Opsiyonel**: dinamik ürün özelliklerini (ör. teknik özellikler) MongoDB’de saklama.  
- Streams: ürünleri filtreleme/sıralama (ör. fiyat veya kategori bazında).  
- Logging: veritabanı işlemlerini izleme.  
- Git: özellik başına commit (ör. `feature/crud`, `feature/streams`).  
- Açıklayıcı README ile GitHub’da yayınla.  

### Kaynaklar
- [SQLBolt](https://sqlbolt.com/)
- [PostgreSQL Official Docs](https://www.postgresql.org/docs/)  
- [Baeldung](https://www.baeldung.com/)  
- [Use The Index, Luke!](https://use-the-index-luke.com/)
- [Hibernate Official Docs](https://hibernate.org/orm/documentation/) 
- [Baeldung – Logging with SLF4J](https://www.baeldung.com/slf4j)
- [Flyway](https://flywaydb.org/)
- [MongoDB University](https://university.mongodb.com/)