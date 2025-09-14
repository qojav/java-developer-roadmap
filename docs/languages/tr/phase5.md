# Faz 5 – Mimari ve Eşzamanlılık (2–3 ay)

### Temiz Kod ve SOLID Prensipleri
- **Clean Code**: Açık isimlendirme, kısa fonksiyonlar, faydalı yorumlar, tutarlı formatlama.  
- **SOLID**:  
  - SRP (Single Responsibility Principle)  
  - OCP (Open/Closed Principle)  
  - LSP (Liskov Substitution Principle)  
  - ISP (Interface Segregation Principle)  
  - DIP (Dependency Inversion Principle)  

**Örnek:** Görev Yöneticisi’nde bir servisi SOLID prensiplerine uygun olarak yeniden düzenleme.  

### Tasarım Kalıpları
- **Kalıplar**: Factory (yaratma), Singleton (tek örnek), Builder (nesne oluşturma), Strategy (davranış), Observer (olaylar).  
- **Uygulama**: Proje bağlamına uygun kalıpları seçme.  

**Örnek:** Farklı görev önceliklendirme algoritmaları için Strategy kullanma.  

### İş Parçacıkları ve Eşzamanlılık
- **Kavramlar**: Thread, Runnable, ExecutorService, ForkJoinPool.  
- **Teknikler**: İş parçacığı havuzları oluşturma ve yönetme, asenkron görevler.  

**Örnek:** Görev raporlarını ExecutorService ile paralel işleme.  

### Senkronizasyon ve Eşzamanlılık Sorunları
- **Mekanizmalar**: `synchronized`, `Lock`, `ReentrantLock`, `ConcurrentHashMap`.  
- **Sorunlar**: Deadlock, race condition, starvation.  

**Örnek:** Paylaşılan bir görev listesine güvenli erişim sağlama.  

### Mikroservislere Giriş
- **Kavramlar**: Mikroservis mimarisi, REST iletişimi, servis keşfi.  
- **Araçlar**: Spring Cloud (ör. servis keşfi için Eureka).  

**Örnek:** Görev Yöneticisi’ni mikroservisler (görevler ve kullanıcılar) olarak ayırma.  

### Mesaj Kuyruğu Temelleri (Opsiyonel)
- **Kavramlar**: Yayıncı/abone, kuyruklar, konular.  
- **RabbitMQ**: Kurulum, mesaj gönderme ve tüketme.  

**Örnek:** Görev güncellemeleri için kullanıcıları RabbitMQ aracılığıyla bilgilendirme.  

### Performans Optimizasyonu
- **Caching**: Veritabanı erişimini azaltmak için Spring Cache ile Redis.  
- **JVM Tuning**: Temel kavramlar (heap, garbage collection).  

**Örnek:** Görev sisteminde sık yapılan sorgular için önbellek uygulama.  

### DevOps/Cloud’a Giriş: Docker ve CI/CD
- **Docker**: Konteynerler, görüntüler, Dockerfile, Docker Compose.  
- **CI/CD**: GitHub Actions ile derleme ve dağıtım için pipeline yapılandırma.  

**Örnek:** Görev uygulaması için Dockerfile oluşturma ve GitHub Actions ile dağıtım.  

### Gözlemlenebilirlik
- **Araçlar**: Prometheus (metrikler), Grafana (görselleştirme), ELK Stack (günlükler).  
- **Kavramlar**: Performans izleme, merkezi günlükler, uyarılar.  

**Örnek:** Görevler için API yanıt süresini Prometheus ve Grafana ile izleme.  

### Güvenlik: OWASP Top Ten
- **Kavramlar**: Enjeksiyon, kimlik doğrulama hataları, hassas veri ifşası.  
- **Uygulamalar**: Girdi doğrulama, temizleme, güvenli konfigürasyon.  

**Örnek:** Görev API’sini SQL injection ve XSS saldırılarına karşı koruma.  

### Final Projesi
**Gelişmiş Görev Yönetim Sistemi**  
- Backend: Görev API’sini (Faz 4) mikroservislerle (görevler ve kullanıcılar) geliştirme.  
- Mimari: Clean Code, SOLID ve tasarım kalıplarıyla (ör. Strategy) yeniden düzenleme.  
- Eşzamanlılık: Raporları ExecutorService ile paralel işleme.  
- **Opsiyonel**: Mikroservisler arası iletişim için RabbitMQ ve sık sorgular için Redis ile önbellek ekleme.  
- DevOps: Docker ile paketleme, GitHub Actions ile CI/CD yapılandırma.  
- Gözlemlenebilirlik: Metrikler için Prometheus ve Grafana ekleme.  
- Güvenlik: OWASP Top Ten’e karşı korumalar uygulama.  
- Git: Özellik başına commit (ör. `feature/microservices`, `feature/concurrency`).  
- Yayın: GitHub’da detaylı README ile (kurulum, mimari, dağıtım).  

### Kaynaklar
- *The Pragmatic Programmer* (Kitap)  
- *Effective Java* (Kitap)  
- *Java Concurrency in Practice* (Kitap)  
- [Spring Cloud Documentation](https://spring.io/projects/spring-cloud)  
- [RabbitMQ Tutorials](https://www.rabbitmq.com/getstarted.html)  
- [Redis University](https://university.redis.com/)  
- [Docker Official Docs](https://docs.docker.com/)  
- [Prometheus Documentation](https://prometheus.io/docs/introduction/overview/)  
- [Grafana Documentation](https://grafana.com/docs/)  
- [ELK Stack Guide](https://www.elastic.co/what-is/elk-stack)  
- [OWASP Top Ten](https://owasp.org/www-project-top-ten/)  
- [GitHub Actions Documentation](https://docs.github.com/en/actions)