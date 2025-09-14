# ফেজ ৪ – ফ্রেমওয়ার্ক এবং ওয়েব অ্যাপ্লিকেশন (৩-৪ মাস)

### Spring Boot, Spring Core, এবং Spring Data JPA
- **Spring Core**: Dependency injection (`@Bean`, `@Autowired`), IoC container.  
- **Spring Boot**: Auto-configuration, starters (`spring-boot-starter-web`, `spring-boot-starter-data-jpa`), `application.yml`.  
- **Spring Data JPA**: Repositories (`CrudRepository`, `JpaRepository`), `@Query` দিয়ে কোয়েরি, পেজিনেশন।  
- **উদাহরণ**: টাস্ক অ্যাপে টাস্ক পরিচালনার জন্য REST endpoints তৈরি (**CRUD**).  

### Spring Security (JWT, OAuth2)
- **ধারণা**: Authentication, authorization, security filters.  
- **JWT**: টোকেন তৈরি এবং যাচাই, `JwtAuthenticationFilter` ব্যবহার।  
- **OAuth2**: Resource Server কনফিগার, কোনো প্রোভাইডারের সাথে ইন্টিগ্রেশন (যেমন, Google).  
- **উদাহরণ**: JWT এবং roles (`ADMIN`, `USER`) দিয়ে টাস্ক endpoints সুরক্ষিত করা।  

### ইউনিট এবং ইন্টিগ্রেশন টেস্টিং
- **Unit tests**: JUnit 5, Mockito (`@Mock`, `@InjectMocks`), বিজনেস লজিক টেস্ট।  
- **Integration tests**: `@SpringBootTest`, `@WebMvcTest`, টেস্টিংয়ের জন্য **H2** ডাটাবেস।  
- **Testcontainers**: Docker কনটেইনারে PostgreSQL দিয়ে টেস্ট।  
- **উদাহরণ**: টাস্ক অ্যাপের সার্ভিস এবং endpoints টেস্ট করা।  

### RESTful APIs এবং Swagger দিয়ে ডকুমেন্টেশন
- **REST**: HTTP মেথড, স্ট্যাটাস কোড, RESTful নীতি।  
- **Spring REST**: `@RestController`, `@RequestMapping`, `@PathVariable`.  
- **Swagger**: **springdoc-openapi** কনফিগার, `@Operation` দিয়ে টীকা।  
- **উদাহরণ**: **Swagger UI** দিয়ে টাস্ক অ্যাপের endpoints ডকুমেন্ট করা।  

### GraphQL-এর পরিচিতি
- **ধারণা**: Queries, mutations, schema.  
- **Spring Boot with GraphQL**: spring-boot-starter-graphql দিয়ে সেটআপ।  
- **উদাহরণ**: স্ট্যাটাস অনুযায়ী টাস্ক তালিকাভুক্ত করতে GraphQL query তৈরি।  

### মৌলিক ফ্রন্টএন্ড ইন্টিগ্রেশন
- **Thymeleaf**: Spring Boot-এর সাথে HTML পেজ রেন্ডারিংয়ের জন্য টেমপ্লেট।  
- **উদাহরণ**: টাস্ক দেখতে এবং তৈরি করতে একটি সাধারণ ওয়েব ইন্টারফেস তৈরি।  

### বিল্ড টুল: Maven এবং Gradle
- **Maven**: `pom.xml` এর গঠন, ডিপেন্ডেন্সি, প্লাগিন।  
- **Gradle**: `build.gradle` ফাইল, টাস্ক, ডিপেন্ডেন্সি ম্যানেজমেন্ট।  
- **উদাহরণ**: Maven এবং Gradle দিয়ে টাস্ক অ্যাপ কনফিগার করা।  

### প্রকল্প ডিপ্লয়মেন্ট
- **প্ল্যাটফর্ম**: Railway, Heroku, AWS (Elastic Beanstalk).  
- **ধাপ**: JAR হিসেবে প্যাকেজিং, GitHub Actions দিয়ে CI/CD কনফিগার।  
- **উদাহরণ**: PostgreSQL সহ Railway-তে টাস্ক অ্যাপ ডিপ্লয় করা।  

### চূড়ান্ত প্রকল্প
**টাস্ক ম্যানেজমেন্ট সিস্টেম**  
- ডাটাবেস: `Task` (শিরোনাম, বিবরণ, স্ট্যাটাস) এবং `User` টেবিল (1:N সম্পর্ক)।  
- Java: Spring Boot, Spring Data JPA দিয়ে REST API তৈরি এবং CRUD।  
- সিকিউরিটি: JWT authentication, roles (`ADMIN`, `USER`).  
- টেস্ট: সার্ভিসের জন্য ইউনিট টেস্ট এবং Testcontainers দিয়ে endpoints-এর ইন্টিগ্রেশন টেস্ট।  
- ডকুমেন্টেশন: endpoints-এর বিবরণ সহ Swagger UI।  
- **ঐচ্ছিক**: টাস্ক তালিকাভুক্ত করতে GraphQL query এবং ইন্টারঅ্যাকশনের জন্য Thymeleaf ইন্টারফেস যোগ করা।  
- Git: প্রতিটি ফিচারের জন্য commit (যেমন, `feature/rest-api`, `feature/security`).  
- প্রকাশ: GitHub-এ README সহ (সেটআপ, endpoints, ডিপ্লয়মেন্ট)।  

### রিসোর্স
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