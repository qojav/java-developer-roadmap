# Phase 6 – Final Projects (Ongoing)

### Project 1: Complete CRUD with Authentication
- **Objective**: Build a robust RESTful API with secure authentication and testing.  
- **Technologies**: Spring Boot, Spring Data JPA (PostgreSQL), Spring Security (JWT), JUnit 5, Testcontainers.  
- **Features**: CRUD for entities (e.g., tasks, users), authentication with roles (ADMIN, USER), documentation with Swagger.  
- **Optional**: Add a Thymeleaf interface to view/manage tasks.  
- **Example**: API to manage projects (entities: `Project`, `Task`, `User`) with protected endpoints.  

### Project 2: File Upload
- **Objective**: Add file upload functionality to the API from Project 1.  
- **Technologies**: Spring Boot (`MultipartFile`), Amazon S3 or local storage, file validation.  
- **Features**: Upload images/documents associated with tasks, validate type/size.  
- **Example**: Allow uploading attachments (e.g., PDF, PNG) for tasks in the API.  

### Project 3: Cloud Deployment
- **Objective**: Deploy the API to a cloud platform with CI/CD.  
- **Technologies**: Railway, Heroku, or AWS (Elastic Beanstalk), GitHub Actions, Docker.  
- **Features**: Package as JAR/Docker, configure environment variables, automate deployment.  
- **Optional**: Implement caching with Redis to optimize frequent queries.  
- **Example**: Deploy the project API on Railway with PostgreSQL and CI/CD.  

### Project 4: Microservices
- **Objective**: Split the API from Project 1 into orchestrated microservices.  
- **Technologies**: Spring Cloud (Eureka, Gateway), Docker Compose, REST for communication.  
- **Features**: Microservices for `Tasks` and `Users`, with service discovery.  
- **Optional**: Use RabbitMQ for asynchronous communication between microservices.  
- **Example**: Separate task and user logic into two services, orchestrated with Docker.  

### Project 5: External API Integration
- **Objective**: Consume an external API to enhance functionality.  
- **Technologies**: Spring RestTemplate or WebClient, API authentication (e.g., OAuth2).  
- **Features**: Integrate with a public API (e.g., send notifications via email with SendGrid).  
- **Optional**: Add a GraphQL query to retrieve tasks/users and store metadata in MongoDB.  
- **Example**: Add email notifications for task completion.  

### Portfolio Best Practices
- **Git**: Commits per feature (e.g., `feature/crud`, `feature/upload`), clear branches.  
- **Documentation**: README with description, setup, endpoints, deployment, and screenshots.  
- **Publish**: Host on GitHub with an open-source license (e.g., MIT).  

### Resources
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