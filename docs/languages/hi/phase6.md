# चरण 6 – अंतिम प्रोजेक्ट्स (चल रहे)

### प्रोजेक्ट 1: पूर्ण CRUD के साथ ऑथेंटिकेशन
- **उद्देश्य**: सुरक्षित ऑथेंटिकेशन और टेस्टिंग के साथ एक मजबूत RESTful API बनाना।  
- **टेक्नोलॉजीज**: Spring Boot, Spring Data JPA (PostgreSQL), Spring Security (JWT), JUnit 5, Testcontainers।  
- **फीचर्स**: एंटिटीज (उदाहरण के लिए, टास्क्स, यूजर्स) के लिए CRUD, roles (ADMIN, USER) के साथ ऑथेंटिकेशन, Swagger के साथ डाक्यूमेंटेशन।  
- **वैकल्पिक**: टास्क्स देखने/प्रबंधन के लिए Thymeleaf इंटरफेस जोड़ना।  
- **उदाहरण**: प्रोजेक्ट्स प्रबंधन के लिए API (एंटिटीज: `Project`, `Task`, `User`) सुरक्षित endpoints के साथ।  

### प्रोजेक्ट 2: फाइल अपलोड
- **उद्देश्य**: प्रोजेक्ट 1 की API में फाइल अपलोड फंक्शनैलिटी जोड़ना।  
- **टेक्नोलॉजीज**: Spring Boot (`MultipartFile`), Amazon S3 या लोकल स्टोरेज, फाइल वैलिडेशन।  
- **फीचर्स**: टास्क्स से संबंधित इमेज/डॉक्यूमेंट्स अपलोड करना, टाइप/साइज़ वैलिडेशन।  
- **उदाहरण**: API में टास्क्स के लिए अटैचमेंट्स (उदाहरण के लिए, PDF, PNG) अपलोड करने की अनुमति देना।  

### प्रोजेक्ट 3: क्लाउड डिप्लॉयमेंट
- **उद्देश्य**: CI/CD के साथ क्लाउड प्लेटफॉर्म पर API डिप्लॉय करना।  
- **टेक्नोलॉजीज**: Railway, Heroku, या AWS (Elastic Beanstalk), GitHub Actions, Docker।  
- **फीचर्स**: JAR/Docker के रूप में पैकेजिंग, पर्यावरण चर कॉन्फ़िगर करना, स्वचालित डिप्लॉयमेंट।  
- **वैकल्पिक**: बार-बार होने वाली क्वेरीज़ को अनुकूलित करने के लिए Redis के साथ कैशिंग लागू करना।  
- **उदाहरण**: PostgreSQL और CI/CD के साथ Railway पर प्रोजेक्ट API डिप्लॉय करना।  

### प्रोजेक्ट 4: माइक्रोसर्विसेज़
- **उद्देश्य**: प्रोजेक्ट 1 की API को ऑर्केस्ट्रेटेड माइक्रोसर्विसेज़ में विभाजित करना।  
- **टेक्नोलॉजीज**: Spring Cloud (Eureka, Gateway), Docker Compose, REST के लिए कम्युनिकेशन।  
- **फीचर्स**: `Tasks` और `Users` के लिए माइक्रोसर्विसेज़, सर्विस डिस्कवरी के साथ।  
- **वैकल्पिक**: माइक्रोसर्विसेज़ के बीच एसिंक्रोनस कम्युनिकेशन के लिए RabbitMQ का उपयोग।  
- **उदाहरण**: टास्क और यूजर लॉजिक को दो सर्विसेज में अलग करना, Docker के साथ ऑर्केस्ट्रेटेड।  

### प्रोजेक्ट 5: एक्सटर्नल API इंटीग्रेशन
- **उद्देश्य**: कार्यक्षमता बढ़ाने के लिए एक एक्सटर्नल API का उपयोग करना।  
- **टेक्नोलॉजीज**: Spring RestTemplate या WebClient, API ऑथेंटिकेशन (उदाहरण के लिए, OAuth2)।  
- **फीचर्स**: एक पब्लिक API के साथ एकीकरण (उदाहरण के लिए, SendGrid के माध्यम से ईमेल नोटिफिकेशन्स भेजना)।  
- **वैकल्पिक**: टास्क्स/यूजर्स को रिट्रीव करने के लिए GraphQL Query जोड़ना और MongoDB में मेटाडेटा स्टोर करना।  
- **उदाहरण**: टास्क पूर्ण होने के लिए ईमेल नोटिफिकेशन्स जोड़ना।  

### पोर्टफोलियो सर्वोत्तम अभ्यास
- **Git**: प्रत्येक फीचर के लिए commit (उदाहरण के लिए, `feature/crud`, `feature/upload`), स्पष्ट ब्रांचेस।  
- **डाक्यूमेंटेशन**: विवरण, सेटअप, endpoints, डिप्लॉयमेंट, और स्क्रीनशॉट्स के साथ README।  
- **प्रकाशन**: GitHub पर ओपन-सोर्स लाइसेंस (उदाहरण के लिए, MIT) के साथ होस्ट करना।  

### संसाधन
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