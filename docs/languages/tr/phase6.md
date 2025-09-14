# Faz 6 – Final Projeleri (Devam Ediyor)

### Proje 1: Kimlik Doğrulama ile Tam CRUD
- **Amaç**: Güvenli kimlik doğrulama ve test ile sağlam bir RESTful API oluşturma.  
- **Teknolojiler**: Spring Boot, Spring Data JPA (PostgreSQL), Spring Security (JWT), JUnit 5, Testcontainers.  
- **Özellikler**: Varlıklar için CRUD (ör. görevler, kullanıcılar), rollerle kimlik doğrulama (ADMIN, USER), Swagger ile dokümantasyon.  
- **Opsiyonel**: Görevleri görüntülemek/yönetmek için Thymeleaf arayüzü ekleme.  
- **Örnek**: Projeleri yönetmek için API (varlıklar: `Project`, `Task`, `User`) korumalı endpoint’lerle.  

### Proje 2: Dosya Yükleme
- **Amaç**: Proje 1’deki API’ye dosya yükleme işlevselliği ekleme.  
- **Teknolojiler**: Spring Boot (`MultipartFile`), Amazon S3 veya yerel depolama, dosya doğrulama.  
- **Özellikler**: Görevlerle ilişkilendirilmiş resim/belge yükleme, tip/boyut doğrulama.  
- **Örnek**: API’deki görevler için ek yükleme izni (ör. PDF, PNG).  

### Proje 3: Bulut Dağıtımı
- **Amaç**: API’yi CI/CD ile bir bulut platformuna dağıtma.  
- **Teknolojiler**: Railway, Heroku veya AWS (Elastic Beanstalk), GitHub Actions, Docker.  
- **Özellikler**: JAR/Docker olarak paketleme, çevre değişkenlerini yapılandırma, dağıtımı otomatikleştirme.  
- **Opsiyonel**: Sık sorguları optimize etmek için Redis ile önbellek uygulama.  
- **Örnek**: Proje API’sini PostgreSQL ve CI/CD ile Railway’e dağıtma.  

### Proje 4: Mikroservisler
- **Amaç**: Proje 1’deki API’yi orkestre edilmiş mikroservislere ayırma.  
- **Teknolojiler**: Spring Cloud (Eureka, Gateway), Docker Compose, iletişim için REST.  
- **Özellikler**: `Tasks` ve `Users` için mikroservisler, servis keşfi ile.  
- **Opsiyonel**: Mikroservisler arası asenkron iletişim için RabbitMQ kullanma.  
- **Örnek**: Görev ve kullanıcı mantığını iki servise ayırma, Docker ile orkestrasyon.  

### Proje 5: Harici API Entegrasyonu
- **Amaç**: İşlevselliği artırmak için harici bir API tüketme.  
- **Teknolojiler**: Spring RestTemplate veya WebClient, API kimlik doğrulaması (ör. OAuth2).  
- **Özellikler**: Genel bir API ile entegrasyon (ör. SendGrid ile e-posta bildirimleri gönderme).  
- **Opsiyonel**: Görevleri/kullanıcıları almak ve meta verileri MongoDB’de saklamak için GraphQL sorgusu ekleme.  
- **Örnek**: Görev tamamlanması için e-posta bildirimleri ekleme.  

### Portföy En İyi Uygulamaları
- **Git**: Özellik başına commit (ör. `feature/crud`, `feature/upload`), açık dallar.  
- **Dokümantasyon**: Açıklama, kurulum, endpoint’ler, dağıtım ve ekran görüntüleri içeren README.  
- **Yayın**: GitHub’da açık kaynak lisansı ile barındırma (ör. MIT).  

### Kaynaklar
- [GitHub Guides](https://guides.github.com)  
- [Spring Boot Official Docs](https://spring.io/projects/spring-boot)  
- [Baeldung – Spring Boot Tutorials](https://www.baeldung.com)  
- [Spring Cloud Documentation](https://spring.io/projects/spring-cloud)  
- [Docker Official Docs](https://docs.docker.com)  
- [Railway Documentation](https://docs.railway.app)  
- [Heroku Dev Center](https://devcenter.heroku.com)  
- [AWS Elastic Beanstalk](https://docs.aws.amazon.com/elasticbeanstalk)  
- [SendGrid API Docs](https://docs.sendgrid.com)  
- [Awesome Open Source](https://awesomeopensource.com)  
- [Practical MongoDB Aggregations](https://university.mongodb.com/courses/MongoDB-Aggregations)