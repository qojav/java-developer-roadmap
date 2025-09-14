# Faz 4 – Çerçeveler ve Web Uygulamaları (3–4 ay)

### Spring Boot, Spring Core ve Spring Data JPA
- **Spring Core**: Dependency injection (`@Bean`, `@Autowired`), IoC container.  
- **Spring Boot**: Otomatik konfigürasyon, starter’lar (`spring-boot-starter-web`, `spring-boot-starter-data-jpa`), `application.yml`.  
- **Spring Data JPA**: Repositories (`CrudRepository`, `JpaRepository`), `@Query` ile sorgular, sayfalama.  
- **Örnek**: Bir görev uygulamasında görevleri yönetmek için REST endpoint’leri oluşturma (**CRUD**).  

### Spring Security (JWT, OAuth2)
- **Kavramlar**: Kimlik doğrulama, yetkilendirme, güvenlik filtreleri.  
- **JWT**: Token oluşturma ve doğrulama, `JwtAuthenticationFilter` kullanımı.  
- **OAuth2**: Resource Server yapılandırma, bir sağlayıcı ile entegrasyon (ör. Google).  
- **Örnek**: Görev endpoint’lerini JWT ve rollerle (`ADMIN`, `USER`) koruma.  

### Birim ve Entegrasyon Testleri
- **Unit tests**: JUnit 5, Mockito (`@Mock`, `@InjectMocks`), iş mantığını test etme.  
- **Integration tests**: `@SpringBootTest`, `@WebMvcTest`, test için **H2** veritabanı.  
- **Testcontainers**: Docker konteynerlerinde PostgreSQL ile test.  
- **Örnek**: Görev uygulamasının servislerini ve endpoint’lerini test etme.  

### RESTful API’ler ve Swagger ile Dokümantasyon
- **REST**: HTTP metodları, durum kodları, RESTful prensipler.  
- **Spring REST**: `@RestController`, `@RequestMapping`, `@PathVariable`.  
- **Swagger**: **springdoc-openapi** yapılandırma, `@Operation` ile anotasyon.  
- **Örnek**: Görev uygulaması endpoint’lerini **Swagger UI** ile dokümante etme.  

### GraphQL’e Giriş
- **Kavramlar**: Sorgular, mutasyonlar, şema.  
- **Spring Boot ile GraphQL**: spring-boot-starter-graphql ile kurulum.  
- **Örnek**: Görevleri duruma göre listelemek için bir GraphQL sorgusu oluşturma.  

### Temel Frontend Entegrasyonu
- **Thymeleaf**: Spring Boot ile HTML sayfalarını oluşturmak için şablonlar.  
- **Örnek**: Görevleri görüntülemek ve oluşturmak için basit bir web arayüzü oluşturma.  

### Yapı Araçları: Maven ve Gradle
- **Maven**: `pom.xml` yapısı, bağımlılıklar, eklentiler.  
- **Gradle**: `build.gradle` dosyası, görevler, bağımlılık yönetimi.  
- **Örnek**: Görev uygulamasını Maven ve Gradle ile yapılandırma.  

### Proje Dağıtımı
- **Platformlar**: Railway, Heroku, AWS (Elastic Beanstalk).  
- **Adımlar**: JAR olarak paketleme, GitHub Actions ile CI/CD yapılandırma.  
- **Örnek**: Görev uygulamasını PostgreSQL ile Railway’e dağıtma.  

### Final Projesi
**Görev Yönetim Sistemi**  
- Veritabanı: `Task` (başlık, açıklama, durum) ve `User` tabloları (1:N ilişkisi).  
- Java: Spring Boot ile REST API, Spring Data JPA ile CRUD.  
- Güvenlik: JWT kimlik doğrulama, roller (`ADMIN`, `USER`).  
- Testler: Unit tests (servisler) ve integration tests (Testcontainers ile endpoint’ler).  
- Dokümantasyon: Endpoint açıklamaları ile Swagger UI.  
- **Opsiyonel**: Görevleri listelemek için GraphQL sorgusu ve etkileşim için Thymeleaf arayüzü ekleme.  
- Git: Özellik başına commit (ör. `feature/rest-api`, `feature/security`).  
- Yayın: GitHub’da README ile (kurulum, endpoint’ler, dağıtım).  

### Kaynaklar
- [Spring Boot Official Docs](https://spring.io/projects/spring-boot)  
- [Baeldung – Spring Boot Tutorials](https://www.baeldung.com/spring-boot)  
- [Spring Security Guide](https://spring.io/guides/topicals/spring-security-architecture)  
- [Testcontainers Official Docs](https://testcontainers.org/)  
- [Springdoc OpenAPI (Swagger)](https://springdoc.org/)  
- [AWS Free Tier Tutorials](https://aws.amazon.com/free/)  
- [GraphQL Official](https://graphql.org/learn/)  
- [Spring Boot with Thymeleaf](https://spring.io/guides/gs/serving-web-content/)  
- [Railway Documentation](https://docs.railway.app/)  
- [Heroku Dev Center](https://devcenter.heroku.com/)  
- [GitHub Actions Documentation](https://docs.github.com/en/actions)