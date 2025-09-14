# Phase 6 – Abschlussprojekte (laufend)

### Projekt 1: Vollständiges CRUD mit Authentifizierung
- **Ziel**: Erstellen einer robusten RESTful API mit sicherer Authentifizierung und Tests.  
- **Technologien**: Spring Boot, Spring Data JPA (PostgreSQL), Spring Security (JWT), JUnit 5, Testcontainers.  
- **Features**: CRUD für Entitäten (z. B. Aufgaben, Benutzer), Authentifizierung mit Rollen (ADMIN, USER), Dokumentation mit Swagger.  
- **Optional**: Hinzufügen einer Thymeleaf-Oberfläche zum Anzeigen/Verwalten von Aufgaben.  
- **Beispiel**: API zur Verwaltung von Projekten (Entitäten: `Project`, `Task`, `User`) mit geschützten Endpoints.  

### Projekt 2: Datei-Upload
- **Ziel**: Hinzufügen einer Datei-Upload-Funktion zur API aus Projekt 1.  
- **Technologien**: Spring Boot (`MultipartFile`), Amazon S3 oder lokaler Speicher, Dateivalidierung.  
- **Features**: Hochladen von Bildern/Dokumenten, die mit Aufgaben verknüpft sind, Validierung von Typ/Größe.  
- **Beispiel**: Ermöglichen des Hochladens von Anhängen (z. B. PDF, PNG) für Aufgaben in der API.  

### Projekt 3: Cloud-Bereitstellung
- **Ziel**: Bereitstellung der API auf einer Cloud-Plattform mit CI/CD.  
- **Technologien**: Railway, Heroku oder AWS (Elastic Beanstalk), GitHub Actions, Docker.  
- **Features**: Verpacken als JAR/Docker, Konfiguration von Umgebungsvariablen, automatisierte Bereitstellung.  
- **Optional**: Implementierung von Caching mit Redis zur Optimierung häufiger Abfragen.  
- **Beispiel**: Bereitstellung der Projekt-API auf Railway mit PostgreSQL und CI/CD.  

### Projekt 4: Microservices
- **Ziel**: Aufteilung der API aus Projekt 1 in orchestrierte Microservices.  
- **Technologien**: Spring Cloud (Eureka, Gateway), Docker Compose, REST für Kommunikation.  
- **Features**: Microservices für `Tasks` und `Users`, mit Service Discovery.  
- **Optional**: Verwendung von RabbitMQ für asynchrone Kommunikation zwischen Microservices.  
- **Beispiel**: Trennung der Logik für Aufgaben und Benutzer in zwei Services, orchestriert mit Docker.  

### Projekt 5: Integration externer APIs
- **Ziel**: Nutzung einer externen API zur Erweiterung der Funktionalität.  
- **Technologien**: Spring RestTemplate oder WebClient, API-Authentifizierung (z. B. OAuth2).  
- **Features**: Integration mit einer öffentlichen API (z. B. Senden von Benachrichtigungen per E-Mail mit SendGrid).  
- **Optional**: Hinzufügen einer GraphQL Query zum Abrufen von Aufgaben/Benutzern und Speichern von Metadaten in MongoDB.  
- **Beispiel**: Hinzufügen von E-Mail-Benachrichtigungen bei Abschluss von Aufgaben.  

### Best Practices für das Portfolio
- **Git**: Commits pro Feature (z. B. `feature/crud`, `feature/upload`), klare Branches.  
- **Dokumentation**: README mit Beschreibung, Setup, Endpoints, Bereitstellung und Screenshots.  
- **Veröffentlichung**: Hosting auf GitHub mit einer Open-Source-Lizenz (z. B. MIT).  

### Ressourcen
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