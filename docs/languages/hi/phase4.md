# चरण 4 – फ्रेमवर्क्स और वेब एप्लिकेशन्स (3-4 महीने)

### Spring Boot, Spring Core, और Spring Data JPA
- **Spring Core**: Dependency Injection (`@Bean`, `@Autowired`), IoC Container.  
- **Spring Boot**: Auto-Configuration, Starters (`spring-boot-starter-web`, `spring-boot-starter-data-jpa`), `application.yml`.  
- **Spring Data JPA**: Repositories (`CrudRepository`, `JpaRepository`), `@Query` के साथ क्वेरीज़, पेजिनेशन।  
- **उदाहरण**: टास्क ऐप में टास्क प्रबंधन के लिए REST Endpoints बनाना (**CRUD**).  

### Spring Security (JWT, OAuth2)
- **अवधारणाएँ**: Authentication, Authorization, Security Filters.  
- **JWT**: टोकन बनाना और सत्यापित करना, `JwtAuthenticationFilter` का उपयोग।  
- **OAuth2**: Resource Server कॉन्फ़िगर करना, किसी प्रदाता (उदाहरण के लिए, Google) के साथ एकीकरण।  
- **उदाहरण**: JWT और roles (`ADMIN`, `USER`) के साथ टास्क endpoints को सुरक्षित करना।  

### यूनिट और इंटीग्रेशन टेस्टिंग
- **Unit Tests**: JUnit 5, Mockito (`@Mock`, `@InjectMocks`), बिजनेस लॉजिक का टेस्ट।  
- **Integration Tests**: `@SpringBootTest`, `@WebMvcTest`, टेस्टिंग के लिए **H2** डेटाबेस।  
- **Testcontainers**: Docker कंटेनर में PostgreSQL के साथ टेस्ट।  
- **उदाहरण**: टास्क ऐप के सर्विसेज और endpoints का टेस्ट करना।  

### RESTful APIs और Swagger के साथ डाक्यूमेंटेशन
- **REST**: HTTP मेथड्स, स्टेटस कोड्स, RESTful सिद्धांत।  
- **Spring REST**: `@RestController`, `@RequestMapping`, `@PathVariable`.  
- **Swagger**: **springdoc-openapi** कॉन्फ़िगर करना, `@Operation` के साथ एनोटेट करना।  
- **उदाहरण**: **Swagger UI** के साथ टास्क ऐप endpoints का डाक्यूमेंटेशन।  

### GraphQL का परिचय
- **अवधारणाएँ**: Queries, Mutations, Schema.  
- **Spring Boot with GraphQL**: spring-boot-starter-graphql के साथ सेटअप।  
- **उदाहरण**: स्टेटस के आधार पर टास्क लिस्ट करने के लिए GraphQL Query बनाना।  

### मूल फ्रंटएंड इंटीग्रेशन
- **Thymeleaf**: Spring Boot के साथ HTML पेज रेंडर करने के लिए टेम्पलेट्स।  
- **उदाहरण**: टास्क देखने और बनाने के लिए एक साधारण वेब इंटरफेस बनाना।  

### बिल्ड टूल्स: Maven और Gradle
- **Maven**: `pom.xml` की संरचना, डिपेंडेंसीज़, प्लगइन्स।  
- **Gradle**: `build.gradle` फ़ाइल, टास्क्स, डिपेंडेंसी मैनेजमेंट।  
- **उदाहरण**: Maven और Gradle के साथ टास्क ऐप कॉन्फ़िगर करना।  

### प्रोजेक्ट डिप्लॉयमेंट
- **प्लेटफॉर्म्स**: Railway, Heroku, AWS (Elastic Beanstalk).  
- **चरण**: JAR के रूप में पैकेजिंग, GitHub Actions के साथ CI/CD कॉन्फ़िगर करना।  
- **उदाहरण**: PostgreSQL के साथ Railway पर टास्क ऐप डिप्लॉय करना।  

### अंतिम प्रोजेक्ट
**टास्क मैनेजमेंट सिस्टम**  
- डेटाबेस: `Task` (शीर्षक, विवरण, स्टेटस) और `User` टेबल्स (1:N संबंध)।  
- Java: Spring Boot, Spring Data JPA के साथ REST API बनाना और CRUD।  
- सिक्योरिटी: JWT Authentication, roles (`ADMIN`, `USER`).  
- टेस्ट्स: यूनिट टेस्ट्स (सर्विसेज) और इंटीग्रेशन टेस्ट्स (Testcontainers के साथ endpoints)।  
- डाक्यूमेंटेशन: endpoints के विवरण के साथ Swagger UI।  
- **वैकल्पिक**: टास्क लिस्ट करने के लिए GraphQL Query और इंटरैक्शन के लिए Thymeleaf इंटरफेस जोड़ना।  
- Git: प्रत्येक फीचर के लिए commit (उदाहरण के लिए, `feature/rest-api`, `feature/security`)।  
- प्रकाशन: GitHub पर README के साथ (सेटअप, endpoints, डिप्लॉयमेंट)।  

### संसाधन
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