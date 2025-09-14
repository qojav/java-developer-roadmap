# ফেজ ৫ – আর্কিটেকচার এবং কনকারেন্সি (২-৩ মাস)

### Clean Code এবং SOLID নীতি
- **Clean Code**: স্পষ্ট নামকরণ, সংক্ষিপ্ত ফাংশন, সহায়ক মন্তব্য, সামঞ্জস্যপূর্ণ ফরম্যাটিং।  
- **SOLID**:  
  - SRP (Single Responsibility Principle)  
  - OCP (Open/Closed Principle)  
  - LSP (Liskov Substitution Principle)  
  - ISP (Interface Segregation Principle)  
  - DIP (Dependency Inversion Principle)  

**উদাহরণ**: SOLID নীতি অনুসরণ করতে টাস্ক ম্যানেজারের একটি সার্ভিস রিফ্যাক্টর করা।  

### ডিজাইন প্যাটার্ন
- **প্যাটার্ন**: Factory (সৃষ্টি), Singleton (একক ইনস্ট্যান্স), Builder (অবজেক্ট নির্মাণ), Strategy (আচরণ), Observer (ইভেন্ট)।  
- **প্রয়োগ**: প্রকল্পের প্রেক্ষাপটের জন্য উপযুক্ত প্যাটার্ন নির্বাচন।  

**উদাহরণ**: বিভিন্ন টাস্ক প্রায়োরিটাইজেশন অ্যালগরিদমের জন্য Strategy ব্যবহার।  

### থ্রেড এবং কনকারেন্সি
- **ধারণা**: Thread, Runnable, ExecutorService, ForkJoinPool.  
- **টেকনিক**: থ্রেড পুল তৈরি এবং পরিচালনা, অ্যাসিনক্রোনাস টাস্ক।  

**উদাহরণ**: ExecutorService দিয়ে টাস্ক রিপোর্ট সমান্তরালভাবে প্রক্রিয়াকরণ।  

### সিনক্রোনাইজেশন এবং কনকারেন্সি সমস্যা
- **মেকানিজম**: `synchronized`, `Lock`, `ReentrantLock`, `ConcurrentHashMap`.  
- **সমস্যা**: Deadlock, race condition, starvation.  

**উদাহরণ**: শেয়ারড টাস্ক লিস্টে নিরাপদ অ্যাক্সেস বাস্তবায়ন।  

### মাইক্রোসার্ভিসের পরিচিতি
- **ধারণা**: মাইক্রোসার্ভিস আর্কিটেকচার, REST কমিউনিকেশন, সার্ভিস ডিসকভারি।  
- **টুল**: Spring Cloud (যেমন, Eureka ফর service discovery).  

**উদাহরণ**: টাস্ক ম্যানেজারকে মাইক্রোসার্ভিসে বিভক্ত করা (টাস্ক এবং ইউজার)।  

### মেসেজ কিউ ফান্ডামেন্টাল (ঐচ্ছিক)
- **ধারণা**: Publisher/subscriber, queues, topics.  
- **RabbitMQ**: সেটআপ, মেসেজ পাঠানো এবং গ্রহণ।  

**উদাহরণ**: RabbitMQ দিয়ে টাস্ক আপডেট সম্পর্কে ইউজারদের নোটিফাই করা।  

### পারফরম্যান্স অপটিমাইজেশন
- **Caching**: Spring Cache সহ Redis দিয়ে ডাটাবেস অ্যাক্সেস কমানো।  
- **JVM Tuning**: মৌলিক ধারণা (heap, garbage collection).  

**উদাহরণ**: টাস্ক সিস্টেমে ঘন ঘন কোয়েরির জন্য ক্যাশ বাস্তবায়ন।  

### DevOps/Cloud পরিচিতি: Docker এবং CI/CD
- **Docker**: কনটেইনার, ইমেজ, Dockerfile, Docker Compose.  
- **CI/CD**: GitHub Actions দিয়ে বিল্ড এবং ডিপ্লয়ের জন্য পাইপলাইন কনফিগার।  

**উদাহরণ**: টাস্ক অ্যাপের জন্য Dockerfile তৈরি এবং GitHub Actions দিয়ে ডিপ্লয়।  

### অবজারভেবিলিটি
- **টুল**: Prometheus (মেট্রিক্স), Grafana (ভিজ্যুয়ালাইজেশন), ELK Stack (লগ)।  
- **ধারণা**: পারফরম্যান্স মনিটরিং, সেন্ট্রালাইজড লগ, অ্যালার্ট।  

**উদাহরণ**: Prometheus এবং Grafana দিয়ে টাস্ক API-এর রেসপন্স টাইম মনিটরিং।  

### সিকিউরিটি: OWASP Top Ten
- **ধারণা**: ইনজেকশন, অথেনটিকেশন ফেইলিওর, সংবেদনশীল ডেটা এক্সপোজার।  
- **অনুশীলন**: ইনপুট ভ্যালিডেশন, স্যানিটাইজেশন, সিকিউর কনফিগারেশন।  

**উদাহরণ**: SQL injection এবং XSS থেকে টাস্ক API সুরক্ষিত করা।  

### চূড়ান্ত প্রকল্প
**অ্যাডভান্সড টাস্ক ম্যানেজমেন্ট সিস্টেম**  
- ব্যাকএন্ড: ফেজ ৪-এর টাস্ক API উন্নত করা মাইক্রোসার্ভিস দিয়ে (টাস্ক এবং ইউজার)।  
- আর্কিটেকচার: Clean Code, SOLID, এবং design patterns (যেমন, Strategy) দিয়ে রিফ্যাক্টর।  
- কনকারেন্সি: ExecutorService দিয়ে রিপোর্ট সমান্তরালভাবে প্রক্রিয়াকরণ।  
- **ঐচ্ছিক**: RabbitMQ দিয়ে মাইক্রোসার্ভিসগুলোর মধ্যে যোগাযোগ এবং ঘন ঘন কোয়েরির জন্য Redis দিয়ে ক্যাশিং।  
- DevOps: Docker-এ প্যাকেজিং, GitHub Actions দিয়ে CI/CD কনফিগার।  
- অবজারভেবিলিটি: মেট্রিক্সের জন্য Prometheus এবং Grafana যোগ করা।  
- সিকিউরিটি: OWASP Top Ten-এর বিরুদ্ধে সুরক্ষা বাস্তবায়ন।  
- Git: প্রতিটি ফিচারের জন্য commit (যেমন, `feature/microservices`, `feature/concurrency`).  
- প্রকাশ: GitHub-এ বিস্তারিত README সহ (সেটআপ, আর্কিটেকচার, ডিপ্লয়মেন্ট)।  

### রিসোর্স
- *The Pragmatic Programmer* (বই)  
- *Effective Java* (বই)  
- *Java Concurrency in Practice* (বই)  
- [Spring Cloud Documentation](https://spring.io/projects/spring-cloud)  
- [RabbitMQ Tutorials](https://www.rabbitmq.com/getstarted.html)  
- [Redis University](https://university.redis.com/)  
- [Docker Official Docs](https://docs.docker.com/)  
- [Prometheus Documentation](https://prometheus.io/docs/introduction/overview/)  
- [Grafana Documentation](https://grafana.com/docs/)  
- [ELK Stack Guide](https://www.elastic.co/what-is/elk-stack)  
- [OWASP Top Ten](https://owasp.org/www-project-top-ten/)  
- [GitHub Actions Documentation](https://docs.github.com/en/actions)  