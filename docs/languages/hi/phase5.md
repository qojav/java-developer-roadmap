# चरण 5 – आर्किटेक्चर और कनकरेंसी (2-3 महीने)

### Clean Code और SOLID सिद्धांत
- **Clean Code**: स्पष्ट नामकरण, छोटे फंक्शन्स, उपयोगी टिप्पणियाँ, सुसंगत फॉर्मेटिंग।  
- **SOLID**:  
  - SRP (Single Responsibility Principle)  
  - OCP (Open/Closed Principle)  
  - LSP (Liskov Substitution Principle)  
  - ISP (Interface Segregation Principle)  
  - DIP (Dependency Inversion Principle)  

**उदाहरण**: टास्क मैनेजर में एक सर्विस को SOLID सिद्धांतों के अनुसार रिफैक्टर करना।  

### डिज़ाइन पैटर्न्स
- **पैटर्न्स**: Factory (निर्माण), Singleton (एकल इंस्टैंस), Builder (ऑब्जेक्ट निर्माण), Strategy (व्यवहार), Observer (इवेंट्स)।  
- **एप्लिकेशन**: प्रोजेक्ट संदर्भ के लिए उपयुक्त पैटर्न्स का चयन।  

**उदाहरण**: विभिन्न टास्क प्रायोरिटाइजेशन एल्गोरिदम के लिए Strategy का उपयोग।  

### थ्रेड्स और कनकरेंसी
- **अवधारणाएँ**: Thread, Runnable, ExecutorService, ForkJoinPool।  
- **तकनीकें**: थ्रेड पूल बनाना और प्रबंधन, एसिंक्रोनस टास्क्स।  

**उदाहरण**: ExecutorService के साथ टास्क रिपोर्ट्स को समानांतर में प्रोसेस करना।  

### सिंक्रोनाइज़ेशन और कनकरेंसी समस्याएँ
- **मैकेनिज़्म्स**: `synchronized`, `Lock`, `ReentrantLock`, `ConcurrentHashMap`।  
- **समस्याएँ**: Deadlock, Race Condition, Starvation।  

**उदाहरण**: साझा टास्क लिस्ट में सुरक्षित पहुँच लागू करना।  

### माइक्रोसर्विसेज़ का परिचय
- **अवधारणाएँ**: माइक्रोसर्विसेज़ आर्किटेक्चर, REST कम्युनिकेशन, सर्विस डिस्कवरी।  
- **टूल्स**: Spring Cloud (उदाहरण के लिए, Eureka for service discovery)।  

**उदाहरण**: टास्क मैनेजर को माइक्रोसर्विसेज़ (टास्क्स और यूजर्स) में विभाजित करना।  

### मेसेज क्यू फंडामेंटल्स (वैकल्पिक)
- **अवधारणाएँ**: Publisher/Subscriber, Queues, Topics।  
- **RabbitMQ**: सेटअप, मेसेज भेजना और उपभोग करना।  

**उदाहरण**: RabbitMQ के माध्यम से यूजर्स को टास्क अपडेट्स के बारे में सूचित करना।  

### परफॉर्मेंस ऑप्टिमाइज़ेशन
- **Caching**: Spring Cache के साथ Redis का उपयोग डेटाबेस एक्सेस को कम करने के लिए।  
- **JVM Tuning**: मूल अवधारणाएँ (Heap, Garbage Collection)।  

**उदाहरण**: टास्क सिस्टम में बार-बार होने वाली क्वेरीज़ के लिए कैश लागू करना।  

### DevOps/Cloud का परिचय: Docker और CI/CD
- **Docker**: कंटेनर्स, इमेजेस, Dockerfile, Docker Compose।  
- **CI/CD**: GitHub Actions के साथ बिल्ड और डिप्लॉय के लिए पाइपलाइन कॉन्फ़िगर करना।  

**उदाहरण**: टास्क ऐप के लिए Dockerfile बनाना और GitHub Actions के माध्यम से डिप्लॉय करना।  

### ऑब्जर्वेबिलिटी
- **टूल्स**: Prometheus (मेट्रिक्स), Grafana (विज़ुअलाइज़ेशन), ELK Stack (लॉग्स)।  
- **अवधारणाएँ**: परफॉर्मेंस मॉनिटरिंग, सेंट्रलाइज़्ड लॉग्स, अलर्ट्स।  

**उदाहरण**: Prometheus और Grafana के साथ टास्क्स के लिए API रिस्पॉन्स टाइम की निगरानी।  

### सिक्योरिटी: OWASP Top Ten
- **अवधारणाएँ**: Injection, Authentication Failures, संवेदनशील डेटा एक्सपोज़र।  
- **अभ्यास**: इनपुट वैलिडेशन, सैनिटाइज़ेशन, सुरक्षित कॉन्फ़िगरेशन।  

**उदाहरण**: टास्क API को SQL Injection और XSS से सुरक्षित करना।  

### अंतिम प्रोजेक्ट
**उन्नत टास्क मैनेजमेंट सिस्टम**  
- बैकएंड: चरण 4 की टास्क API को माइक्रोसर्विसेज़ (टास्क्स और यूजर्स) के साथ बढ़ाना।  
- आर्किटेक्चर: Clean Code, SOLID, और Design Patterns (उदाहरण के लिए, Strategy) के साथ रिफैक्टर करना।  
- कनकरेंसी: ExecutorService के साथ रिपोर्ट्स को समानांतर में प्रोसेस करना।  
- **वैकल्पिक**: RabbitMQ के माध्यम से माइक्रोसर्विसेज़ के बीच कम्युनिकेशन और बार-बार होने वाली क्वेरीज़ के लिए Redis के साथ कैशिंग जोड़ना।  
- DevOps: Docker में पैकेजिंग, GitHub Actions के साथ CI/CD कॉन्फ़िगर करना।  
- ऑब्जर्वेबिलिटी: मेट्रिक्स के लिए Prometheus और Grafana जोड़ना।  
- सिक्योरिटी: OWASP Top Ten के खिलाफ सुरक्षा लागू करना।  
- Git: प्रत्येक फीचर के लिए commit (उदाहरण के लिए, `feature/microservices`, `feature/concurrency`)।  
- प्रकाशन: GitHub पर विस्तृत README के साथ (सेटअप, आर्किटेक्चर, डिप्लॉयमेंट)।  

### संसाधन
- *The Pragmatic Programmer* (पुस्तक)  
- *Effective Java* (पुस्तक)  
- *Java Concurrency in Practice* (पुस्तक)  
- [Spring Cloud Documentation](https://spring.io/projects/spring-cloud)  
- [RabbitMQ Tutorials](https://www.rabbitmq.com/getstarted.html)  
- [Redis University](https://university.redis.com/)  
- [Docker Official Docs](https://docs.docker.com/)  
- [Prometheus Documentation](https://prometheus.io/docs/introduction/overview/)  
- [Grafana Documentation](https://grafana.com/docs/)  
- [ELK Stack Guide](https://www.elastic.co/what-is/elk-stack)  
- [OWASP Top Ten](https://owasp.org/www-project-top-ten/)  
- [GitHub Actions Documentation](https://docs.github.com/en/actions)  