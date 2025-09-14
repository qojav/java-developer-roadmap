# Phase 5 – Architecture and Concurrency (2–3 months)

### Clean Code and SOLID Principles
- **Clean Code**: Clear naming, short functions, helpful comments, consistent formatting.  
- **SOLID**:  
  - SRP (Single Responsibility Principle)  
  - OCP (Open/Closed Principle)  
  - LSP (Liskov Substitution Principle)  
  - ISP (Interface Segregation Principle)  
  - DIP (Dependency Inversion Principle)  

**Example:** Refactor a service in the Task Manager to follow SOLID principles.  

### Design Patterns
- **Patterns**: Factory (creation), Singleton (single instance), Builder (object construction), Strategy (behavior), Observer (events).  
- **Application**: Choose patterns suitable for the project context.  

**Example:** Use Strategy for different task prioritization algorithms.  

### Threads and Concurrency
- **Concepts**: Thread, Runnable, ExecutorService, ForkJoinPool.  
- **Techniques**: Create and manage thread pools, asynchronous tasks.  

**Example:** Process task reports in parallel with ExecutorService.  

### Synchronization and Concurrency Issues
- **Mechanisms**: `synchronized`, `Lock`, `ReentrantLock`, `ConcurrentHashMap`.  
- **Issues**: Deadlock, race condition, starvation.  

**Example:** Implement safe access to a shared task list.  

### Introduction to Microservices
- **Concepts**: Microservices architecture, REST communication, service discovery.  
- **Tools**: Spring Cloud (e.g., Eureka for service discovery).  

**Example:** Split the Task Manager into microservices (tasks and users).  

### Message Queue Fundamentals (Optional)
- **Concepts**: Publisher/subscriber, queues, topics.  
- **RabbitMQ**: Setup, sending and consuming messages.  

**Example:** Notify users about task updates via RabbitMQ.  

### Performance Optimization
- **Caching**: Spring Cache with Redis to reduce database access.  
- **JVM Tuning**: Basic concepts (heap, garbage collection).  

**Example:** Implement cache for frequent queries in the task system.  

### Introduction to DevOps/Cloud: Docker and CI/CD
- **Docker**: Containers, images, Dockerfile, Docker Compose.  
- **CI/CD**: Configure pipelines with GitHub Actions for build and deploy.  

**Example:** Create a Dockerfile for the task app and deploy via GitHub Actions.  

### Observability
- **Tools**: Prometheus (metrics), Grafana (visualization), ELK Stack (logs).  
- **Concepts**: Performance monitoring, centralized logs, alerts.  

**Example:** Monitor API response time for tasks with Prometheus and Grafana.  

### Security: OWASP Top Ten
- **Concepts**: Injection, authentication failures, sensitive data exposure.  
- **Practices**: Input validation, sanitization, secure configuration.  

**Example:** Protect the task API against SQL injection and XSS.  

### Final Project
**Advanced Task Management System**  
- Backend: Enhance the task API (Phase 4) with microservices (tasks and users).  
- Architecture: Refactor with Clean Code, SOLID, and design patterns (e.g., Strategy).  
- Concurrency: Process reports in parallel with ExecutorService.  
- **Optional**: Add communication between microservices via RabbitMQ and caching with Redis for frequent queries.  
- DevOps: Package in Docker, configure CI/CD with GitHub Actions.  
- Observability: Add Prometheus and Grafana for metrics.  
- Security: Implement protections against OWASP Top Ten.  
- Git: Commits per feature (e.g., `feature/microservices`, `feature/concurrency`).  
- Publish: On GitHub with detailed README (setup, architecture, deployment).  

### Resources
- *The Pragmatic Programmer* (Book)  
- *Effective Java* (Book)  
- *Java Concurrency in Practice* (Book)  
- [Spring Cloud Documentation](https://spring.io/projects/spring-cloud)  
- [RabbitMQ Tutorials](https://www.rabbitmq.com/getstarted.html)  
- [Redis University](https://university.redis.com/)  
- [Docker Official Docs](https://docs.docker.com/)  
- [Prometheus Documentation](https://prometheus.io/docs/introduction/overview/)  
- [Grafana Documentation](https://grafana.com/docs/)  
- [ELK Stack Guide](https://www.elastic.co/what-is/elk-stack)  
- [OWASP Top Ten](https://owasp.org/www-project-top-ten/)  
- [GitHub Actions Documentation](https://docs.github.com/en/actions)  