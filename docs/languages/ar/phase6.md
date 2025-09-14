# المرحلة 6 – المشاريع النهائية (مستمرة)

### المشروع 1: CRUD كامل مع المصادقة
- **الهدف**: بناء API RESTful قوية مع مصادقة آمنة واختبارات.  
- **التقنيات**: Spring Boot, Spring Data JPA (PostgreSQL), Spring Security (JWT), JUnit 5, Testcontainers.  
- **الميزات**: CRUD للكيانات (مثل المهام، المستخدمين)، المصادقة مع roles (ADMIN, USER)، التوثيق باستخدام Swagger.  
- **اختياري**: إضافة واجهة Thymeleaf لعرض/إدارة المهام.  
- **مثال**: API لإدارة المشاريع (الكيانات: `Project`, `Task`, `User`) مع endpoints محمية.  

### المشروع 2: رفع الملفات
- **الهدف**: إضافة وظيفة رفع الملفات إلى API المشروع 1.  
- **التقنيات**: Spring Boot (`MultipartFile`), Amazon S3 أو التخزين المحلي، التحقق من الملفات.  
- **الميزات**: رفع الصور/المستندات المرتبطة بالمهام، التحقق من النوع/الحجم.  
- **مثال**: السماح برفع المرفقات (مثل PDF, PNG) للمهام في API.  

### المشروع 3: النشر السحابي
- **الهدف**: نشر API على منصة سحابية مع CI/CD.  
- **التقنيات**: Railway, Heroku, أو AWS (Elastic Beanstalk), GitHub Actions, Docker.  
- **الميزات**: التعبئة كـ JAR/Docker، تهيئة متغيرات البيئة، أتمتة النشر.  
- **اختياري**: تنفيذ التخزين المؤقت باستخدام Redis لتحسين الاستعلامات المتكررة.  
- **مثال**: نشر API المشروع على Railway مع PostgreSQL و CI/CD.  

### المشروع 4: الخدمات الدقيقة
- **الهدف**: تقسيم API المشروع 1 إلى خدمات دقيقة منسقة.  
- **التقنيات**: Spring Cloud (Eureka, Gateway), Docker Compose, REST للتواصل.  
- **الميزات**: خدمات دقيقة لـ `Tasks` و `Users`، مع اكتشاف الخدمات.  
- **اختياري**: استخدام RabbitMQ للتواصل غير المتزامن بين الخدمات الدقيقة.  
- **مثال**: فصل منطق المهام والمستخدمين إلى خدمتين، منسقتين باستخدام Docker.  

### المشروع 5: التكامل مع API خارجية
- **الهدف**: استهلاك API خارجية لتعزيز الوظائف.  
- **التقنيات**: Spring RestTemplate أو WebClient، مصادقة API (مثل OAuth2).  
- **الميزات**: التكامل مع API عامة (مثل إرسال إشعارات عبر البريد الإلكتروني باستخدام SendGrid).  
- **اختياري**: إضافة query GraphQL لاسترداد المهام/المستخدمين وتخزين البيانات الوصفية في MongoDB.  
- **مثال**: إضافة إشعارات بريد إلكتروني عند اكتمال المهام.  

### أفضل ممارسات المحفظة
- **Git**: commit لكل ميزة (مثال: `feature/crud`, `feature/upload`)، فروع واضحة.  
- **التوثيق**: README يحتوي على الوصف، الإعداد، endpoints، النشر، ولقطات الشاشة.  
- **النشر**: استضافة على GitHub مع رخصة مفتوحة المصدر (مثل MIT).  

### الموارد
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