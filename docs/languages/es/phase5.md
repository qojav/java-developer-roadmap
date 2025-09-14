# Fase 5 – Arquitectura y Concurrencia (2–3 meses)

### Clean Code y Principios SOLID
- **Clean Code**: Nomenclatura clara, funciones cortas, comentarios útiles, formato consistente.  
- **SOLID**:  
  - SRP (Single Responsibility Principle)  
  - OCP (Open/Closed Principle)  
  - LSP (Liskov Substitution Principle)  
  - ISP (Interface Segregation Principle)  
  - DIP (Dependency Inversion Principle)  

**Ejemplo**: Refactorizar un servicio del Gestor de Tareas para seguir los principios SOLID.  

### Design Patterns
- **Patrones**: Factory (creación), Singleton (instancia única), Builder (construcción de objetos), Strategy (comportamiento), Observer (eventos).  
- **Aplicación**: Elegir patrones adecuados al contexto del proyecto.  

**Ejemplo**: Usar Strategy para diferentes algoritmos de priorización de tareas.  

### Threads y Concurrencia
- **Conceptos**: Thread, Runnable, ExecutorService, ForkJoinPool.  
- **Técnicas**: Crear y gestionar pools de threads, tareas asíncronas.  

**Ejemplo**: Procesar informes de tareas en paralelo con ExecutorService.  

### Sincronización y Problemas de Concurrencia
- **Mecanismos**: `synchronized`, `Lock`, `ReentrantLock`, `ConcurrentHashMap`.  
- **Problemas**: Deadlock, race condition, starvation.  

**Ejemplo**: Implementar acceso seguro a una lista de tareas compartida.  

### Introducción a Microservicios
- **Conceptos**: Arquitectura de microservicios, comunicación vía REST, descubrimiento de servicios.  
- **Herramientas**: Spring Cloud (por ejemplo, Eureka para descubrimiento de servicios).  

**Ejemplo**: Dividir el Gestor de Tareas en microservicios (tareas y usuarios).  

### Fundamentos de Colas de Mensajes (Opcional)
- **Conceptos**: Publisher/subscriber, colas, tópicos.  
- **RabbitMQ**: Configuración, envío y consumo de mensajes.  

**Ejemplo**: Notificar a usuarios sobre actualizaciones de tareas vía RabbitMQ.  

### Optimización de Rendimiento
- **Caching**: Spring Cache con Redis para reducir accesos a la base de datos.  
- **JVM Tuning**: Conceptos básicos (heap, garbage collection).  

**Ejemplo**: Implementar cache para consultas frecuentes en el sistema de tareas.  

### Introducción a DevOps/Cloud: Docker y CI/CD
- **Docker**: Contenedores, imágenes, Dockerfile, Docker Compose.  
- **CI/CD**: Configurar pipelines con GitHub Actions para construcción y despliegue.  

**Ejemplo**: Crear un Dockerfile para la aplicación de tareas y desplegar vía GitHub Actions.  

### Observabilidad
- **Herramientas**: Prometheus (métricas), Grafana (visualización), ELK Stack (logs).  
- **Conceptos**: Monitoreo de rendimiento, logs centralizados, alertas.  

**Ejemplo**: Monitorear el tiempo de respuesta de la API de tareas con Prometheus y Grafana.  

### Seguridad: OWASP Top Ten
- **Conceptos**: Inyección, fallos de autenticación, exposición de datos sensibles.  
- **Prácticas**: Validación de entrada, sanitización, configuración segura.  

**Ejemplo**: Proteger la API de tareas contra inyección SQL y XSS.  

### Proyecto Final
**Sistema Avanzado de Gestión de Tareas**  
- Backend: Mejorar la API de tareas (Fase 4) con microservicios (tareas y usuarios).  
- Arquitectura: Refactorizar con Clean Code, SOLID y design patterns (por ejemplo, Strategy).  
- Concurrencia: Procesar informes en paralelo con ExecutorService.  
- **Opcional**: Agregar comunicación entre microservicios vía RabbitMQ y caching con Redis para consultas frecuentes.  
- DevOps: Empaquetar en Docker, configurar CI/CD con GitHub Actions.  
- Observabilidad: Agregar Prometheus y Grafana para métricas.  
- Seguridad: Implementar protecciones contra OWASP Top Ten.  
- Git: Commits por funcionalidad (por ejemplo, `feature/microservices`, `feature/concurrency`).  
- Publicar: En GitHub con README detallado (configuración, arquitectura, despliegue).  

### Recursos
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