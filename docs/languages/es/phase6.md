# Fase 6 – Proyectos Finales (Continuo)

### Proyecto 1: CRUD Completo con Autenticación
- **Objetivo**: Construir una API RESTful robusta con autenticación segura y pruebas.  
- **Tecnologías**: Spring Boot, Spring Data JPA (PostgreSQL), Spring Security (JWT), JUnit 5, Testcontainers.  
- **Funcionalidades**: CRUD para entidades (por ejemplo, tareas, usuarios), autenticación con roles (ADMIN, USER), documentación con Swagger.  
- **Opcional**: Agregar una interfaz Thymeleaf para visualizar/gestionar tareas.  
- **Ejemplo**: API para gestionar proyectos (entidades: `Project`, `Task`, `User`) con endpoints protegidos.  

### Proyecto 2: Carga de Archivos
- **Objetivo**: Agregar funcionalidad de carga de archivos a la API del Proyecto 1.  
- **Tecnologías**: Spring Boot (`MultipartFile`), Amazon S3 o almacenamiento local, validación de archivos.  
- **Funcionalidades**: Carga de imágenes/documentos asociados a tareas, validación de tipo/tamaño.  
- **Ejemplo**: Permitir la carga de anexos (por ejemplo, PDF, PNG) para tareas en la API.  

### Proyecto 3: Despliegue en la Nube
- **Objetivo**: Desplegar la API en una plataforma en la nube con CI/CD.  
- **Tecnologías**: Railway, Heroku o AWS (Elastic Beanstalk), GitHub Actions, Docker.  
- **Funcionalidades**: Empaquetar como JAR/Docker, configurar variables de entorno, automatizar el despliegue.  
- **Opcional**: Implementar caching con Redis para optimizar consultas frecuentes.  
- **Ejemplo**: Desplegar la API de proyectos en Railway con PostgreSQL y CI/CD.  

### Proyecto 4: Microservicios
- **Objetivo**: Dividir la API del Proyecto 1 en microservicios orquestados.  
- **Tecnologías**: Spring Cloud (Eureka, Gateway), Docker Compose, REST para comunicación.  
- **Funcionalidades**: Microservicios para `Tasks` y `Users`, con descubrimiento de servicios.  
- **Opcional**: Usar RabbitMQ para comunicación asíncrona entre microservicios.  
- **Ejemplo**: Separar la lógica de tareas y usuarios en dos servicios, orquestados con Docker.  

### Proyecto 5: Integración con API Externa
- **Objetivo**: Consumir una API externa para enriquecer la funcionalidad.  
- **Tecnologías**: Spring RestTemplate o WebClient, autenticación de API (por ejemplo, OAuth2).  
- **Funcionalidades**: Integrar con una API pública (por ejemplo, enviar notificaciones por correo con SendGrid).  
- **Opcional**: Agregar una query GraphQL para consultar tareas/usuarios y almacenar metadatos en MongoDB.  
- **Ejemplo**: Agregar notificaciones por correo electrónico para la finalización de tareas.  

### Mejores Prácticas de Portafolio
- **Git**: Commits por funcionalidad (por ejemplo, `feature/crud`, `feature/upload`), ramas claras.  
- **Documentación**: README con descripción, configuración, endpoints, despliegue y capturas de pantalla.  
- **Publicar**: Hospedar en GitHub con una licencia open-source (por ejemplo, MIT).  

### Recursos
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