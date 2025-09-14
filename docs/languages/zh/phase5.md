# 第五阶段 – 架构与并发（2-3个月）

### Clean Code 与 SOLID 原则
- **Clean Code**: 清晰的命名，短小的函数，有用的注释，一致的格式。  
- **SOLID**:  
  - SRP (Single Responsibility Principle)  
  - OCP (Open/Closed Principle)  
  - LSP (Liskov Substitution Principle)  
  - ISP (Interface Segregation Principle)  
  - DIP (Dependency Inversion Principle)  

**示例**: 重构任务管理器中的服务以遵循 SOLID 原则。  

### 设计模式
- **模式**: Factory（创建），Singleton（单一实例），Builder（对象构建），Strategy（行为），Observer（事件）。  
- **应用**: 选择适合项目上下文的模式。  

**示例**: 使用 Strategy 实现不同的任务优先级算法。  

### 线程与并发
- **概念**: Thread, Runnable, ExecutorService, ForkJoinPool。  
- **技术**: 创建和管理线程池，异步任务。  

**示例**: 使用 ExecutorService 并行处理任务报告。  

### 同步与并发问题
- **机制**: `synchronized`, `Lock`, `ReentrantLock`, `ConcurrentHashMap`。  
- **问题**: Deadlock, race condition, starvation。  

**示例**: 实现对共享任务列表的安全访问。  

### 微服务介绍
- **概念**: 微服务架构，REST 通信，服务发现。  
- **工具**: Spring Cloud（例如，Eureka 用于服务发现）。  

**示例**: 将任务管理器拆分为微服务（任务和用户）。  

### 消息队列基础（可选）
- **概念**: Publisher/subscriber，队列，主题。  
- **RabbitMQ**: 设置，发送和消费消息。  

**示例**: 通过 RabbitMQ 通知用户任务更新。  

### 性能优化
- **Caching**: 使用 Redis 的 Spring Cache 减少数据库访问。  
- **JVM Tuning**: 基本概念（heap, garbage collection）。  

**示例**: 为任务系统中的频繁查询实现缓存。  

### DevOps/Cloud 介绍：Docker 与 CI/CD
- **Docker**: 容器，镜像，Dockerfile，Docker Compose。  
- **CI/CD**: 使用 GitHub Actions 配置构建和部署管道。  

**示例**: 为任务应用创建 Dockerfile 并通过 GitHub Actions 部署。  

### 可观测性
- **工具**: Prometheus（指标），Grafana（可视化），ELK Stack（日志）。  
- **概念**: 性能监控，集中式日志，警报。  

**示例**: 使用 Prometheus 和 Grafana 监控任务 API 的响应时间。  

### 安全：OWASP Top Ten
- **概念**: 注入，认证失败，敏感数据暴露。  
- **实践**: 输入验证，数据清理，安全配置。  

**示例**: 保护任务 API 免受 SQL 注入和 XSS 攻击。  

### 最终项目
**高级任务管理系统**  
- 后端: 增强第四阶段的任务 API，使用微服务（任务和用户）。  
- 架构: 使用 Clean Code、SOLID 和 design patterns（例如 Strategy）重构。  
- 并发: 使用 ExecutorService 并行处理报告。  
- **可选**: 通过 RabbitMQ 实现微服务间通信，并使用 Redis 为频繁查询实现缓存。  
- DevOps: 使用 Docker 打包，配置 GitHub Actions 的 CI/CD。  
- 可观测性: 添加 Prometheus 和 Grafana 用于指标监控。  
- 安全: 实现针对 OWASP Top Ten 的保护措施。  
- Git: 按功能提交（例如，`feature/microservices`, `feature/concurrency`）。  
- 发布: 在 GitHub 上发布，附带详细的 README（设置、架构、部署）。  

### 资源
- *The Pragmatic Programmer*（书籍）  
- *Effective Java*（书籍）  
- *Java Concurrency in Practice*（书籍）  
- [Spring Cloud Documentation](https://spring.io/projects/spring-cloud)  
- [RabbitMQ Tutorials](https://www.rabbitmq.com/getstarted.html)  
- [Redis University](https://university.redis.com/)  
- [Docker Official Docs](https://docs.docker.com/)  
- [Prometheus Documentation](https://prometheus.io/docs/introduction/overview/)  
- [Grafana Documentation](https://grafana.com/docs/)  
- [ELK Stack Guide](https://www.elastic.co/what-is/elk-stack)  
- [OWASP Top Ten](https://owasp.org/www-project-top-ten/)  
- [GitHub Actions Documentation](https://docs.github.com/en/actions)  