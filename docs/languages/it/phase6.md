# Fase 6 – Progetti Finali (In Corso)

### Progetto 1: CRUD Completo con Autenticazione
- **Obiettivo**: Costruire un'API RESTful robusta con autenticazione sicura e test.  
- **Tecnologie**: Spring Boot, Spring Data JPA (PostgreSQL), Spring Security (JWT), JUnit 5, Testcontainers.  
- **Funzionalità**: CRUD per entità (es. attività, utenti), autenticazione con ruoli (ADMIN, USER), documentazione con Swagger.  
- **Opzionale**: Aggiungere un'interfaccia Thymeleaf per visualizzare/gestire le attività.  
- **Esempio**: API per gestire progetti (entità: `Project`, `Task`, `User`) con endpoint protetti.  

### Progetto 2: Caricamento File
- **Obiettivo**: Aggiungere funzionalità di caricamento file all'API del Progetto 1.  
- **Tecnologie**: Spring Boot (`MultipartFile`), Amazon S3 o storage locale, validazione dei file.  
- **Funzionalità**: Caricare immagini/documenti associati alle attività, validare tipo/dimensione.  
- **Esempio**: Consentire il caricamento di allegati (es. PDF, PNG) per le attività nell'API.  

### Progetto 3: Distribuzione su Cloud
- **Obiettivo**: Distribuire l'API su una piattaforma cloud con CI/CD.  
- **Tecnologie**: Railway, Heroku o AWS (Elastic Beanstalk), GitHub Actions, Docker.  
- **Funzionalità**: Pacchettizzare come JAR/Docker, configurare variabili d'ambiente, automatizzare la distribuzione.  
- **Opzionale**: Implementare caching con Redis per ottimizzare query frequenti.  
- **Esempio**: Distribuire l'API del progetto su Railway con PostgreSQL e CI/CD.  

### Progetto 4: Microservizi
- **Obiettivo**: Dividere l'API del Progetto 1 in microservizi orchestrati.  
- **Tecnologie**: Spring Cloud (Eureka, Gateway), Docker Compose, REST per la comunicazione.  
- **Funzionalità**: Microservizi per `Tasks` e `Users`, con service discovery.  
- **Opzionale**: Usare RabbitMQ per la comunicazione asincrona tra microservizi.  
- **Esempio**: Separare la logica di attività e utenti in due servizi, orchestrati con Docker.  

### Progetto 5: Integrazione con API Esterne
- **Obiettivo**: Consumare un'API esterna per migliorare le funzionalità.  
- **Tecnologie**: Spring RestTemplate o WebClient, autenticazione API (es. OAuth2).  
- **Funzionalità**: Integrare con un'API pubblica (es. inviare notifiche via email con SendGrid).  
- **Opzionale**: Aggiungere una query GraphQL per recuperare attività/utenti e memorizzare metadati in MongoDB.  
- **Esempio**: Aggiungere notifiche email per il completamento delle attività.  

### Best Practices per il Portfolio
- **Git**: Commit per funzionalità (es. `feature/crud`, `feature/upload`), branch chiari.  
- **Documentazione**: README con descrizione, configurazione, endpoint, distribuzione e screenshot.  
- **Pubblicazione**: Ospitare su GitHub con licenza open-source (es. MIT).  

### Risorse
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