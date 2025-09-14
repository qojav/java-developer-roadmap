# Phase 5 – Architektur und Konkurrenz (2–3 Monate)

### Clean Code und SOLID-Prinzipien
- **Clean Code**: Klare Namensgebung, kurze Funktionen, hilfreiche Kommentare, konsistentes Format.  
- **SOLID**:  
  - SRP (Single Responsibility Principle)  
  - OCP (Open/Closed Principle)  
  - LSP (Liskov Substitution Principle)  
  - ISP (Interface Segregation Principle)  
  - DIP (Dependency Inversion Principle)  

**Beispiel:** Refaktorisierung eines Services im Task Manager, um SOLID-Prinzipien einzuhalten.  

### Design Patterns
- **Patterns**: Factory (Erstellung), Singleton (einzelne Instanz), Builder (Objektkonstruktion), Strategy (Verhalten), Observer (Ereignisse).  
- **Anwendung**: Auswahl von Patterns, die zum Projektkontext passen.  

**Beispiel:** Verwendung von Strategy für verschiedene Priorisierungsalgorithmen von Aufgaben.  

### Threads und Konkurrenz
- **Konzepte**: Thread, Runnable, ExecutorService, ForkJoinPool.  
- **Techniken**: Erstellen und Verwalten von Thread-Pools, asynchrone Aufgaben.  

**Beispiel:** Parallele Verarbeitung von Aufgabenberichten mit ExecutorService.  

### Synchronisation und Konkurrenzprobleme
- **Mechanismen**: `synchronized`, `Lock`, `ReentrantLock`, `ConcurrentHashMap`.  
- **Probleme**: Deadlock, Race Condition, Starvation.  

**Beispiel:** Implementierung eines sicheren Zugriffs auf eine gemeinsame Aufgabenliste.  

### Einführung in Microservices
- **Konzepte**: Microservices-Architektur, REST-Kommunikation, Service Discovery.  
- **Tools**: Spring Cloud (z. B. Eureka für Service Discovery).  

**Beispiel:** Aufteilung des Task Managers in Microservices (Aufgaben und Benutzer).  

### Grundlagen von Message Queues (optional)
- **Konzepte**: Publisher/Subscriber, Queues, Topics.  
- **RabbitMQ**: Einrichtung, Senden und Empfangen von Nachrichten.  

**Beispiel:** Benachrichtigung von Benutzern über Aufgabenaktualisierungen via RabbitMQ.  

### Performance-Optimierung
- **Caching**: Spring Cache mit Redis, um Datenbankzugriffe zu reduzieren.  
- **JVM Tuning**: Grundlegende Konzepte (Heap, Garbage Collection).  

**Beispiel:** Implementierung eines Caches für häufige Abfragen im Aufgabensystem.  

### Einführung in DevOps/Cloud: Docker und CI/CD
- **Docker**: Container, Images, Dockerfile, Docker Compose.  
- **CI/CD**: Konfiguration von Pipelines mit GitHub Actions für Build und Deployment.  

**Beispiel**: Erstellen eines Dockerfile für die Task-App und Deployment via GitHub Actions.  

### Observability
- **Tools**: Prometheus (Metriken), Grafana (Visualisierung), ELK Stack (Logs).  
- **Konzepte**: Performance-Überwachung, zentralisierte Logs, Alarme.  

**Beispiel**: Überwachung der API-Antwortzeit für Aufgaben mit Prometheus und Grafana.  

### Sicherheit: OWASP Top Ten
- **Konzepte**: Injection, Authentifizierungsfehler, Offenlegung sensibler Daten.  
- **Praktiken**: Eingabevalidierung, Sanitization, sichere Konfiguration.  

**Beispiel**: Schutz der Task-API gegen SQL Injection und XSS.  

### Abschlussprojekt
**Fortgeschrittenes Task-Management-System**  
- Backend: Erweiterung der Task-API (Phase 4) mit Microservices (Aufgaben und Benutzer).  
- Architektur: Refaktorisierung mit Clean Code, SOLID und Design Patterns (z. B. Strategy).  
- Konkurrenz: Parallele Verarbeitung von Berichten mit ExecutorService.  
- **Optional**: Hinzufügen von Kommunikation zwischen Microservices via RabbitMQ und Caching mit Redis für häufige Abfragen.  
- DevOps: Verpacken in Docker, Konfiguration von CI/CD mit GitHub Actions.  
- Observability: Hinzufügen von Prometheus und Grafana für Metriken.  
- Sicherheit: Implementierung von Schutzmaßnahmen gegen OWASP Top Ten.  
- Git: Commits pro Feature (z. B. `feature/microservices`, `feature/concurrency`).  
- Veröffentlichung: Auf GitHub mit detailliertem README (Setup, Architektur, Deployment).  

### Ressourcen
- *The Pragmatic Programmer* (Buch)  
- *Effective Java* (Buch)  
- *Java Concurrency in Practice* (Buch)  
- [Spring Cloud Documentation](https://spring.io/projects/spring-cloud)  
- [RabbitMQ Tutorials](https://www.rabbitmq.com/getstarted.html)  
- [Redis University](https://university.redis.com/)  
- [Docker Official Docs](https://docs.docker.com/)  
- [Prometheus Documentation](https://prometheus.io/docs/introduction/overview/)  
- [Grafana Documentation](https://grafana.com/docs/)  
- [ELK Stack Guide](https://www.elastic.co/what-is/elk-stack)  
- [OWASP Top Ten](https://owasp.org/www-project-top-ten/)  
- [GitHub Actions Documentation](https://docs.github.com/en/actions)  