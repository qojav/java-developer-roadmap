# Fase 5 – Architettura e Concorrenza (2–3 mesi)

### Clean Code e Principi SOLID
- **Clean Code**: Nomenclatura chiara, funzioni brevi, commenti utili, formattazione coerente.  
- **SOLID**:  
  - SRP (Single Responsibility Principle)  
  - OCP (Open/Closed Principle)  
  - LSP (Liskov Substitution Principle)  
  - ISP (Interface Segregation Principle)  
  - DIP (Dependency Inversion Principle)  

**Esempio:** Rifattorizzare un servizio nel Task Manager per seguire i principi SOLID.  

### Design Patterns
- **Pattern**: Factory (creazione), Singleton (istanza unica), Builder (costruzione oggetti), Strategy (comportamento), Observer (eventi).  
- **Applicazione**: Scegliere pattern adeguati al contesto del progetto.  

**Esempio:** Utilizzare Strategy per diversi algoritmi di prioritizzazione delle attività.  

### Thread e Concorrenza
- **Concetti**: Thread, Runnable, ExecutorService, ForkJoinPool.  
- **Tecniche**: Creare e gestire pool di thread, attività asincrone.  

**Esempio:** Elaborare report di attività in parallelo con ExecutorService.  

### Sincronizzazione e Problemi di Concorrenza
- **Meccanismi**: `synchronized`, `Lock`, `ReentrantLock`, `ConcurrentHashMap`.  
- **Problemi**: Deadlock, race condition, starvation.  

**Esempio:** Implementare l'accesso sicuro a una lista di attività condivisa.  

### Introduzione ai Microservizi
- **Concetti**: Architettura dei microservizi, comunicazione REST, scoperta dei servizi.  
- **Strumenti**: Spring Cloud (es. Eureka per la scoperta dei servizi).  

**Esempio:** Dividere il Task Manager in microservizi (attività e utenti).  

### Fondamenti di Code di Messaggi (Opzionale)
- **Concetti**: Publisher/subscriber, code, topic.  
- **RabbitMQ**: Configurazione, invio e ricezione di messaggi.  

**Esempio:** Notificare agli utenti gli aggiornamenti delle attività tramite RabbitMQ.  

### Ottimizzazione delle Prestazioni
- **Caching**: Spring Cache con Redis per ridurre l'accesso al database.  
- **Tuning JVM**: Concetti di base (heap, garbage collection).  

**Esempio:** Implementare cache per query frequenti nel sistema di attività.  

### Introduzione a DevOps/Cloud: Docker e CI/CD
- **Docker**: Container, immagini, Dockerfile, Docker Compose.  
- **CI/CD**: Configurare pipeline con GitHub Actions per build e deploy.  

**Esempio:** Creare un Dockerfile per l'app di attività e distribuirla tramite GitHub Actions.  

### Osservabilità
- **Strumenti**: Prometheus (metriche), Grafana (visualizzazione), ELK Stack (log).  
- **Concetti**: Monitoraggio delle prestazioni, log centralizzati, avvisi.  

**Esempio:** Monitorare il tempo di risposta dell'API delle attività con Prometheus e Grafana.  

### Sicurezza: OWASP Top Ten
- **Concetti**: Injection, fallimenti di autenticazione, esposizione di dati sensibili.  
- **Pratiche**: Validazione dell'input, sanitizzazione, configurazione sicura.  

**Esempio:** Proteggere l'API delle attività da SQL injection e XSS.  

### Progetto Finale
**Sistema Avanzato di Gestione delle Attività**  
- Backend: Migliorare l'API delle attività (Fase 4) con microservizi (attività e utenti).  
- Architettura: Rifattorizzare con Clean Code, SOLID e design patterns (es. Strategy).  
- Concorrenza: Elaborare report in parallelo con ExecutorService.  
- **Opzionale**: Aggiungere comunicazione tra microservizi tramite RabbitMQ e caching con Redis per query frequenti.  
- DevOps: Pacchettizzare in Docker, configurare CI/CD con GitHub Actions.  
- Osservabilità: Aggiungere Prometheus e Grafana per le metriche.  
- Sicurezza: Implementare protezioni contro OWASP Top Ten.  
- Git: Commit per ogni funzionalità (es. `feature/microservices`, `feature/concurrency`).  
- Pubblicazione: Su GitHub con README dettagliato (configurazione, architettura, distribuzione).  

### Risorse
- *The Pragmatic Programmer* (Libro)  
- *Effective Java* (Libro)  
- *Java Concurrency in Practice* (Libro)  
- [Spring Cloud Documentation](https://spring.io/projects/spring-cloud)  
- [RabbitMQ Tutorials](https://www.rabbitmq.com/getstarted.html)  
- [Redis University](https://university.redis.com/)  
- [Docker Official Docs](https://docs.docker.com/)  
- [Prometheus Documentation](https://prometheus.io/docs/introduction/overview/)  
- [Grafana Documentation](https://grafana.com/docs/)  
- [ELK Stack Guide](https://www.elastic.co/what-is/elk-stack)  
- [OWASP Top Ten](https://owasp.org/www-project-top-ten/)  
- [GitHub Actions Documentation](https://docs.github.com/en/actions)