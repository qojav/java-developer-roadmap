# المرحلة 5 – الهندسة المعمارية والتزامن (2-3 أشهر)

### Clean Code ومبادئ SOLID
- **Clean Code**: تسمية واضحة، دوال قصيرة، تعليقات مفيدة، تنسيق متسق.  
- **SOLID**:  
  - SRP (Single Responsibility Principle)  
  - OCP (Open/Closed Principle)  
  - LSP (Liskov Substitution Principle)  
  - ISP (Interface Segregation Principle)  
  - DIP (Dependency Inversion Principle)  

**مثال**: إعادة هيكلة خدمة في مدير المهام لتتبع مبادئ SOLID.  

### أنماط التصميم
- **الأنماط**: Factory (إنشاء)، Singleton (مثيل واحد)، Builder (بناء الكائنات)، Strategy (السلوك)، Observer (الأحداث).  
- **التطبيق**: اختيار أنماط مناسبة لسياق المشروع.  

**مثال**: استخدام Strategy لخوارزميات مختلفة لتحديد أولويات المهام.  

### الخيوط والتزامن
- **المفاهيم**: Thread, Runnable, ExecutorService, ForkJoinPool.  
- **التقنيات**: إنشاء وإدارة مجموعات الخيوط، المهام غير المتزامنة.  

**مثال**: معالجة تقارير المهام بالتوازي باستخدام ExecutorService.  

### التزامن ومشاكل التزامن
- **الآليات**: `synchronized`, `Lock`, `ReentrantLock`, `ConcurrentHashMap`.  
- **المشاكل**: Deadlock, race condition, starvation.  

**مثال**: تنفيذ الوصول الآمن إلى قائمة مهام مشتركة.  

### مقدمة إلى الخدمات الدقيقة
- **المفاهيم**: هندسة الخدمات الدقيقة، التواصل عبر REST، اكتشاف الخدمات.  
- **الأدوات**: Spring Cloud (مثل Eureka لاكتشاف الخدمات).  

**مثال**: تقسيم مدير المهام إلى خدمات دقيقة (المهام والمستخدمين).  

### أساسيات قوائم الرسائل (اختياري)
- **المفاهيم**: Publisher/subscriber، القوائم، المواضيع.  
- **RabbitMQ**: الإعداد، إرسال واستهلاك الرسائل.  

**مثال**: إخطار المستخدمين بتحديثات المهام عبر RabbitMQ.  

### تحسين الأداء
- **Caching**: Spring Cache مع Redis لتقليل الوصول إلى قاعدة البيانات.  
- **JVM Tuning**: المفاهيم الأساسية (heap, garbage collection).  

**مثال**: تنفيذ التخزين المؤقت للاستعلامات المتكررة في نظام المهام.  

### مقدمة إلى DevOps/Cloud: Docker و CI/CD
- **Docker**: الحاويات، الصور، Dockerfile، Docker Compose.  
- **CI/CD**: تهيئة الأنابيب باستخدام GitHub Actions للبناء والنشر.  

**مثال**: إنشاء Dockerfile لتطبيق المهام والنشر عبر GitHub Actions.  

### القابلية للمراقبة
- **الأدوات**: Prometheus (المقاييس)، Grafana (التصور)، ELK Stack (السجلات).  
- **المفاهيم**: مراقبة الأداء، السجلات المركزية، التنبيهات.  

**مثال**: مراقبة وقت استجابة API للمهام باستخدام Prometheus و Grafana.  

### الأمان: OWASP Top Ten
- **المفاهيم**: الحقن، فشل المصادقة، تعريض البيانات الحساسة.  
- **الممارسات**: التحقق من المدخلات، التنظيف، التهيئة الآمنة.  

**مثال**: حماية API المهام من الحقن SQL و XSS.  

### المشروع النهائي
**نظام إدارة المهام المتقدم**  
- الواجهة الخلفية: تحسين API المهام (المرحلة 4) باستخدام الخدمات الدقيقة (المهام والمستخدمين).  
- الهندسة المعمارية: إعادة هيكلة باستخدام Clean Code، SOLID، و design patterns (مثل Strategy).  
- التزامن: معالجة التقارير بالتوازي باستخدام ExecutorService.  
- **اختياري**: إضافة تواصل بين الخدمات الدقيقة عبر RabbitMQ والتخزين المؤقت باستخدام Redis للاستعلامات المتكررة.  
- DevOps: التعبئة في Docker، تهيئة CI/CD باستخدام GitHub Actions.  
- القابلية للمراقبة: إضافة Prometheus و Grafana للمقاييس.  
- الأمان: تنفيذ الحماية ضد OWASP Top Ten.  
- Git: commit لكل ميزة (مثال: `feature/microservices`, `feature/concurrency`).  
- النشر: على GitHub مع README مفصل (الإعداد، الهندسة المعمارية، النشر).  

### الموارد
- *The Pragmatic Programmer* (كتاب)  
- *Effective Java* (كتاب)  
- *Java Concurrency in Practice* (كتاب)  
- [Spring Cloud Documentation](https://spring.io/projects/spring-cloud)  
- [RabbitMQ Tutorials](https://www.rabbitmq.com/getstarted.html)  
- [Redis University](https://university.redis.com/)  
- [Docker Official Docs](https://docs.docker.com/)  
- [Prometheus Documentation](https://prometheus.io/docs/introduction/overview/)  
- [Grafana Documentation](https://grafana.com/docs/)  
- [ELK Stack Guide](https://www.elastic.co/what-is/elk-stack)  
- [OWASP Top Ten](https://owasp.org/www-project-top-ten/)  
- [GitHub Actions Documentation](https://docs.github.com/en/actions)  