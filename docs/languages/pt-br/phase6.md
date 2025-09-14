# Fase 6 – Projetos Finais (Contínuo)

### Projeto 1: CRUD Completo com Autenticação
- **Objetivo:** Criar uma API RESTful robusta com autenticação segura e testes.  
- **Tecnologias:** Spring Boot, Spring Data JPA (PostgreSQL), Spring Security (JWT), JUnit 5, Testcontainers.  
- **Funcionalidades:** CRUD para entidades (ex.: tarefas, usuários), autenticação com papéis (ADMIN, USER), documentação com Swagger.  
- **Opcional**: adicionar uma interface Thymeleaf para visualizar/gerenciar tarefas.
- **Exemplo:** API para gerenciar projetos (entidades: `Project`, `Task`, `User`) com endpoints protegidos.  

### Projeto 2: Upload de Arquivos
- **Objetivo:** Adicionar funcionalidade de upload de arquivos à API do Projeto 1.  
- **Tecnologias:** Spring Boot (`MultipartFile`), Amazon S3 ou armazenamento local, validação de arquivos.  
- **Funcionalidades:** Upload de imagens/documentos associados a tarefas, validação de tipo/tamanho.  
- **Exemplo:** Permitir upload de anexos (ex.: PDF, PNG) para tarefas na API.  

### Projeto 3: Deploy em Nuvem
- **Objetivo:** Publicar a API em uma plataforma de nuvem com CI/CD.  
- **Tecnologias:** Railway, Heroku ou AWS (Elastic Beanstalk), GitHub Actions, Docker.  
- **Funcionalidades:** Empacotar como JAR/Docker, configurar variáveis de ambiente, automatizar deploy. 
- **Opcional**: implementar caching com Redis para otimizar consultas frequentes. 
- **Exemplo:** Deploy da API de projetos no Railway com PostgreSQL e CI/CD.  

### Projeto 4: Microsserviços
- **Objetivo:** Dividir a API do Projeto 1 em microsserviços orquestrados.  
- **Tecnologias:** Spring Cloud (Eureka, Gateway), Docker Compose, REST para comunicação.  
- **Funcionalidades:** Microsserviços para `Tasks` e `Users`, com descoberta de serviços.  
- **Opcional**: usar RabbitMQ para comunicação assíncrona entre microsserviços.
- **Exemplo:** Separar a lógica de tarefas e usuários em dois serviços, orquestrados com Docker.  

### Projeto 5: Integração com API Externa
- **Objetivo:** Consumir uma API externa para enriquecer a funcionalidade.  
- **Tecnologias:** Spring RestTemplate ou WebClient, autenticação de API (ex.: OAuth2).  
- **Funcionalidades:** Integrar com API pública (ex.: enviar notificações via e-mail com SendGrid). 
- **Opcional**: adicionar uma query GraphQL para consultar tarefas/usuários e armazenar metadados em MongoDB. 
- **Exemplo:** Adicionar envio de e-mails para notificar conclusão de tarefas.  

### Boas Práticas de Portfólio
- **Git:** Commits por funcionalidade (ex.: `feature/crud`, `feature/upload`), branches claras.  
- **Documentação:** README com descrição, setup, endpoints, deploy e capturas de tela.  
- **Publicar:** Hospedar no GitHub com licença open-source (ex.: MIT).  

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