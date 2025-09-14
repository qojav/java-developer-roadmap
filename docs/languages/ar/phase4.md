# المرحلة 4 – الإطارات وتطبيقات الويب (3-4 أشهر)

### Spring Boot، Spring Core، و Spring Data JPA
- **Spring Core**: حقن التبعيات (`@Bean`, `@Autowired`)، حاوية IoC.  
- **Spring Boot**: الإعداد التلقائي، starters (`spring-boot-starter-web`, `spring-boot-starter-data-jpa`)، `application.yml`.  
- **Spring Data JPA**: المستودعات (`CrudRepository`, `JpaRepository`)، الاستعلامات باستخدام `@Query`، التصفح.  
- **مثال**: إنشاء endpoints REST لإدارة المهام (**CRUD**) في تطبيق المهام.  

### Spring Security (JWT, OAuth2)
- **المفاهيم**: المصادقة، التفويض، مرشحات الأمان.  
- **JWT**: إنشاء والتحقق من tokens، استخدام `JwtAuthenticationFilter`.  
- **OAuth2**: تهيئة Resource Server، التكامل مع مزود (مثل Google).  
- **مثال**: حماية endpoints المهام باستخدام JWT و roles (`ADMIN`, `USER`).  

### الاختبارات الوحدية والتكاملية
- **Unit tests**: JUnit 5، Mockito (`@Mock`, `@InjectMocks`)، اختبار المنطق التجاري.  
- **Integration tests**: `@SpringBootTest`, `@WebMvcTest`, قاعدة بيانات **H2** للاختبار.  
- **Testcontainers**: الاختبار باستخدام PostgreSQL في حاويات Docker.  
- **مثال**: اختبار الخدمات و endpoints تطبيق المهام.  

### RESTful APIs وتوثيق باستخدام Swagger
- **REST**: طرق HTTP، أكواد الحالة، مبادئ RESTful.  
- **Spring REST**: `@RestController`, `@RequestMapping`, `@PathVariable`.  
- **Swagger**: تهيئة **springdoc-openapi**، التعليق باستخدام `@Operation`.  
- **مثال**: توثيق endpoints تطبيق المهام باستخدام **Swagger UI**.  

### مقدمة إلى GraphQL
- **المفاهيم**: Queries، mutations، schema.  
- **Spring Boot مع GraphQL**: الإعداد باستخدام spring-boot-starter-graphql.  
- **مثال**: إنشاء query GraphQL لسرد المهام حسب الحالة.  

### التكامل الأمامي الأساسي
- **Thymeleaf**: قوالب لعرض صفحات HTML مع Spring Boot.  
- **مثال**: إنشاء واجهة ويب بسيطة لعرض وإنشاء المهام.  

### أدوات البناء: Maven و Gradle
- **Maven**: هيكلية `pom.xml`، التبعيات، الإضافات.  
- **Gradle**: ملف `build.gradle`، المهام، إدارة التبعيات.  
- **مثال**: تهيئة تطبيق المهام باستخدام Maven و Gradle.  

### نشر المشروع
- **المنصات**: Railway، Heroku، AWS (Elastic Beanstalk).  
- **الخطوات**: التعبئة كـ JAR، تهيئة CI/CD باستخدام GitHub Actions.  
- **مثال**: نشر تطبيق المهام على Railway مع PostgreSQL.  

### المشروع النهائي
**نظام إدارة المهام**  
- قاعدة البيانات: جداول `Task` (العنوان، الوصف، الحالة) و `User` (علاقة 1:N).  
- Java: API REST مع Spring Boot، Spring Data JPA لـ CRUD.  
- الأمان: المصادقة باستخدام JWT، roles (`ADMIN`, `USER`).  
- الاختبارات: اختبارات وحدية (الخدمات) واختبارات تكاملية (endpoints باستخدام Testcontainers).  
- التوثيق: Swagger UI مع وصف endpoints.  
- **اختياري**: إضافة query GraphQL لسرد المهام وواجهة Thymeleaf للتفاعل.  
- Git: commit لكل ميزة (مثال: `feature/rest-api`, `feature/security`).  
- النشر: على GitHub مع README (الإعداد، endpoints، النشر).  

### الموارد
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