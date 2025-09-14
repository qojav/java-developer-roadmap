# ফেজ ৬ – চূড়ান্ত প্রকল্প (চলমান)

### প্রকল্প ১: সম্পূর্ণ CRUD সহ অথেনটিকেশন
- **উদ্দেশ্য**: নিরাপদ অথেনটিকেশন এবং টেস্টিং সহ একটি শক্তিশালী RESTful API তৈরি।  
- **টেকনোলজি**: Spring Boot, Spring Data JPA (PostgreSQL), Spring Security (JWT), JUnit 5, Testcontainers.  
- **ফিচার**: এনটিটি (যেমন, টাস্ক, ইউজার) এর জন্য CRUD, roles (ADMIN, USER) সহ অথেনটিকেশন, Swagger দিয়ে ডকুমেন্টেশন।  
- **ঐচ্ছিক**: টাস্ক দেখতে/পরিচালনার জন্য Thymeleaf ইন্টারফেস যোগ করা।  
- **উদাহরণ**: প্রোজেক্ট পরিচালনার জন্য API (এনটিটি: `Project`, `Task`, `User`) সুরক্ষিত endpoints সহ।  

### প্রকল্প ২: ফাইল আপলোড
- **উদ্দেশ্য**: প্রকল্প ১-এর API-তে ফাইল আপলোড ফাংশনালিটি যোগ করা।  
- **টেকনোলজি**: Spring Boot (`MultipartFile`), Amazon S3 বা লোকাল স্টোরেজ, ফাইল ভ্যালিডেশন।  
- **ফিচার**: টাস্কের সাথে সম্পর্কিত ইমেজ/ডকুমেন্ট আপলোড, টাইপ/সাইজ ভ্যালিডেশন।  
- **উদাহরণ**: API-তে টাস্কের জন্য অ্যাটাচমেন্ট (যেমন, PDF, PNG) আপলোডের অনুমতি দেওয়া।  

### প্রকল্প ৩: ক্লাউড ডিপ্লয়মেন্ট
- **উদ্দেশ্য**: CI/CD সহ ক্লাউড প্ল্যাটফর্মে API ডিপ্লয় করা।  
- **টেকনোলজি**: Railway, Heroku, বা AWS (Elastic Beanstalk), GitHub Actions, Docker.  
- **ফিচার**: JAR/Docker হিসেবে প্যাকেজিং, এনভায়রনমেন্ট ভেরিয়েবল কনফিগার, অটোমেটেড ডিপ্লয়মেন্ট।  
- **ঐচ্ছিক**: ঘন ঘন কোয়েরি অপটিমাইজ করতে Redis দিয়ে ক্যাশিং বাস্তবায়ন।  
- **উদাহরণ**: PostgreSQL এবং CI/CD সহ Railway-তে প্রকল্প API ডিপ্লয়।  

### প্রকল্প ৪: মাইক্রোসার্ভিস
- **উদ্দেশ্য**: প্রকল্প ১-এর API-কে অর্কেস্ট্রেটেড মাইক্রোসার্ভিসে বিভক্ত করা।  
- **টেকনোলজি**: Spring Cloud (Eureka, Gateway), Docker Compose, REST কমিউনিকেশন।  
- **ফিচার**: `Tasks` এবং `Users`-এর জন্য মাইক্রোসার্ভিস, সার্ভিস ডিসকভারি সহ।  
- **ঐচ্ছিক**: মাইক্রোসার্ভিসগুলোর মধ্যে অ্যাসিনক্রোনাস কমিউনিকেশনের জন্য RabbitMQ ব্যবহার।  
- **উদাহরণ**: টাস্ক এবং ইউজার লজিক দুটি সার্ভিসে বিভক্ত করা, Docker দিয়ে অর্কেস্ট্রেটেড।  

### প্রকল্প ৫: এক্সটার্নাল API ইন্টিগ্রেশন
- **উদ্দেশ্য**: ফাংশনালিটি উন্নত করতে এক্সটার্নাল API ব্যবহার।  
- **টেকনোলজি**: Spring RestTemplate বা WebClient, API অথেনটিকেশন (যেমন, OAuth2).  
- **ফিচার**: পাবলিক API-এর সাথে ইন্টিগ্রেশন (যেমন, SendGrid দিয়ে ইমেল নোটিফিকেশন পাঠানো)।  
- **ঐচ্ছিক**: টাস্ক/ইউজার পুনরুদ্ধারের জন্য GraphQL query যোগ করা এবং MongoDB-তে মেটাডেটা সংরক্ষণ।  
- **উদাহরণ**: টাস্ক সম্পন্ন হওয়ার জন্য ইমেল নোটিফিকেশন যোগ করা।  

### পোর্টফোলিওর সর্বোত্তম অনুশীলন
- **Git**: প্রতিটি ফিচারের জন্য commit (যেমন, `feature/crud`, `feature/upload`), স্পষ্ট ব্রাঞ্চ।  
- **ডকুমেন্টেশন**: বর্ণনা, সেটআপ, endpoints, ডিপ্লয়মেন্ট, এবং স্ক্রিনশট সহ README।  
- **প্রকাশ**: ওপেন-সোর্স লাইসেন্স (যেমন, MIT) সহ GitHub-এ হোস্টিং।  

### রিসোর্স
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