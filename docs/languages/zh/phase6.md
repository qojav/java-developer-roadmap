# 第六阶段 – 最终项目（持续进行）

### 项目 1: 带认证的完整 CRUD
- **目标**: 构建一个稳健的 RESTful API，具备安全认证和测试。  
- **技术**: Spring Boot, Spring Data JPA (PostgreSQL), Spring Security (JWT), JUnit 5, Testcontainers。  
- **功能**: 对实体（例如任务、用户）进行 CRUD 操作，带 roles (ADMIN, USER) 的认证，使用 Swagger 进行文档化。  
- **可选**: 添加 Thymeleaf 界面以查看/管理任务。  
- **示例**: 用于管理项目的 API（实体：`Project`, `Task`, `User`），带受保护的 endpoints。  

### 项目 2: 文件上传
- **目标**: 为项目 1 的 API 添加文件上传功能。  
- **技术**: Spring Boot (`MultipartFile`), Amazon S3 或本地存储，文件验证。  
- **功能**: 上传与任务相关的图片/文档，验证类型/大小。  
- **示例**: 允许在 API 中为任务上传附件（例如 PDF, PNG）。  

### 项目 3: 云部署
- **目标**: 将 API 部署到云平台并实现 CI/CD。  
- **技术**: Railway, Heroku 或 AWS (Elastic Beanstalk), GitHub Actions, Docker。  
- **功能**: 打包为 JAR/Docker，配置环境变量，自动化部署。  
- **可选**: 使用 Redis 实现缓存以优化频繁查询。  
- **示例**: 在 Railway 上部署项目 API，结合 PostgreSQL 和 CI/CD。  

### 项目 4: 微服务
- **目标**: 将项目 1 的 API 拆分为编排的微服务。  
- **技术**: Spring Cloud (Eureka, Gateway), Docker Compose, REST 通信。  
- **功能**: 为 `Tasks` 和 `Users` 创建微服务，带服务发现。  
- **可选**: 使用 RabbitMQ 实现微服务间的异步通信。  
- **示例**: 将任务和用户逻辑分为两个服务，使用 Docker 进行编排。  

### 项目 5: 外部 API 集成
- **目标**: 消费外部 API 以增强功能。  
- **技术**: Spring RestTemplate 或 WebClient, API 认证（例如 OAuth2）。  
- **功能**: 集成公共 API（例如，通过 SendGrid 发送电子邮件通知）。  
- **可选**: 添加 GraphQL query 以检索任务/用户，并将元数据存储在 MongoDB 中。  
- **示例**: 添加任务完成时的电子邮件通知。  

### 作品集最佳实践
- **Git**: 按功能提交（例如，`feature/crud`, `feature/upload`），清晰的分支。  
- **文档**: README 包含描述、设置、endpoints、部署和截图。  
- **发布**: 在 GitHub 上托管，带 open-source 许可证（例如 MIT）。  

### 资源
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