# Fase 5 – Arquitetura e Concorrência (2–3 meses)

### Clean Code e Princípios SOLID
- **Clean Code**: Nomenclatura clara, funções curtas, comentários úteis, formatação consistente.  
- **SOLID**:  
  - SRP (Responsabilidade Única)  
  - OCP (Aberto/Fechado)  
  - LSP (Substituição de Liskov)  
  - ISP (Segregação de Interfaces)  
  - DIP (Inversão de Dependência)  

**Exemplo:** Refatorar um serviço do Gerenciador de Tarefas para seguir SOLID.  

### Design Patterns
- **Padrões**: Factory (criação), Singleton (instância única), Builder (construção de objetos), Strategy (comportamento), Observer (eventos).  
- **Aplicação**: Escolher padrões adequados ao contexto do projeto.  

**Exemplo:** Usar Strategy para diferentes algoritmos de priorização de tarefas.  

### Threads e Concorrência
- **Conceitos**: Thread, Runnable, ExecutorService, ForkJoinPool.  
- **Técnicas**: Criar e gerenciar pools de threads, tarefas assíncronas.  

**Exemplo:** Processar relatórios de tarefas em paralelo com ExecutorService.  

### Sincronização e Problemas de Concorrência
- **Mecanismos**: `synchronized`, `Lock`, `ReentrantLock`, `ConcurrentHashMap`.  
- **Problemas**: Deadlock, race condition, starvation.  

**Exemplo:** Implementar acesso seguro a uma lista de tarefas compartilhada.  

### Introdução a Microsserviços
- **Conceitos**: Arquitetura de microsserviços, comunicação via REST, descoberta de serviços.  
- **Ferramentas**: Spring Cloud (ex.: Eureka para descoberta de serviços).  

**Exemplo:** Dividir o Gerenciador de Tarefas em microsserviços (tarefas e usuários).  

### Fundamentos de Filas de Mensagens (Opcional)
- **Conceitos**: publicador/subscriber, filas, tópicos.
- **RabbitMQ**: configuração, envio e consumo de mensagens.

- **Exemplo**: notificar usuários sobre atualizações de tarefas via RabbitMQ.

### Otimização de Performance
- **Caching**: Spring Cache com Redis para reduzir acesso ao banco.
- **JVM Tuning**: conceitos básicos (heap, garbage collection).

- **Exemplo**: implementar cache para consultas frequentes no sistema de tarefas.

### Introdução a DevOps/Cloud: Docker e CI/CD
- **Docker**: Containers, imagens, Dockerfile, Docker Compose.  
- **CI/CD**: Configurar pipelines com GitHub Actions para build e deploy.  

**Exemplo:** Criar um Dockerfile para o app de tarefas e deploy via GitHub Actions.  

### Observabilidade
- **Ferramentas**: Prometheus (métricas), Grafana (visualização), ELK Stack (logs).  
- **Conceitos**: Monitoramento de performance, logs centralizados, alertas.  

**Exemplo:** Monitorar tempo de resposta da API de tarefas com Prometheus e Grafana.  

### Segurança: OWASP Top Ten
- **Conceitos**: Injeção, falhas de autenticação, exposição de dados sensíveis.  
- **Práticas**: Validação de entrada, sanitização, configuração segura.  

**Exemplo:** Proteger a API de tarefas contra injeção SQL e XSS.  

### Projeto Final
**Sistema de Gerenciamento de Tarefas Avançado**  
- Backend: Melhorar a API de tarefas (Fase 4) com microsserviços (tarefas e usuários).  
- Arquitetura: Refatorar com Clean Code, SOLID e padrões de design (ex.: Strategy).  
- Concorrência: Processar relatórios em paralelo com ExecutorService.  
- **Opcional**: adicionar comunicação entre microsserviços via RabbitMQ e caching com Redis para consultas frequentes.
- DevOps: Empacotar em Docker, configurar CI/CD com GitHub Actions.  
- Observabilidade: Adicionar Prometheus e Grafana para métricas.  
- Segurança: Implementar proteções contra OWASP Top Ten.  
- Git: Commits por funcionalidade (ex.: feature/microservices, feature/concurrency).  
- Publicar: No GitHub com README detalhado (setup, arquitetura, deploy).  

### Recursos
- *The Pragmatic Programmer* (Livro)
- *Effective Java* (Livro)
- *Java Concurrency in Practice* (Livro) 
- [Spring Cloud Documentation](https://spring.io/projects/spring-cloud)  
- [RabbitMQ Tutorials](https://www.rabbitmq.com/getstarted.html)
- [Redis University](https://university.redis.com/)
- [Docker Official Docs](https://docs.docker.com/)  
- [Prometheus Documentation](https://prometheus.io/docs/introduction/overview/)  
- [Grafana Documentation](https://grafana.com/docs/)  
- [ELK Stack Guide](https://www.elastic.co/what-is/elk-stack)  
- [OWASP Top Ten](https://owasp.org/www-project-top-ten/)  
- [GitHub Actions Documentation](https://docs.github.com/en/actions)  
