# 5단계 – 아키텍처와 동시성 (2~3개월)

### Clean Code와 SOLID 원칙
- **Clean Code**: 명확한 명명, 짧은 함수, 유용한 주석, 일관된 포맷팅.  
- **SOLID**:  
  - SRP (Single Responsibility Principle)  
  - OCP (Open/Closed Principle)  
  - LSP (Liskov Substitution Principle)  
  - ISP (Interface Segregation Principle)  
  - DIP (Dependency Inversion Principle)  

**예제**: 태스크 매니저의 서비스를 SOLID 원칙에 따라 리팩토링.  

### Design Patterns
- **패턴**: Factory (생성), Singleton (단일 인스턴스), Builder (객체 구성), Strategy (행동), Observer (이벤트).  
- **적용**: 프로젝트 컨텍스트에 적합한 패턴 선택.  

**예제**: 다양한 태스크 우선순위 알고리즘에 Strategy 사용.  

### Threads와 동시성
- **개념**: Thread, Runnable, ExecutorService, ForkJoinPool.  
- **기술**: 스레드 풀 생성 및 관리, 비동기 태스크.  

**예제**: ExecutorService로 태스크 보고서를 병렬 처리.  

### 동기화와 동시성 문제
- **메커니즘**: `synchronized`, `Lock`, `ReentrantLock`, `ConcurrentHashMap`.  
- **문제**: Deadlock, Race Condition, Starvation.  

**예제**: 공유 태스크 리스트에 안전한 접근 구현.  

### 마이크로서비스 소개
- **개념**: 마이크로서비스 아키텍처, REST 통신, 서비스 디스커버리.  
- **도구**: Spring Cloud (예: Eureka for service discovery).  

**예제**: 태스크 매니저를 마이크로서비스(태스크와 사용자)로 분할.  

### 메시지 큐 기초 (선택 사항)
- **개념**: Publisher/Subscriber, 큐, 토픽.  
- **RabbitMQ**: 설정, 메시지 송수신.  

**예제**: RabbitMQ를 통해 사용자에게 태스크 업데이트 알림.  

### 성능 최적화
- **Caching**: 데이터베이스 접근을 줄이기 위해 Redis를 사용한 Spring Cache.  
- **JVM Tuning**: 기본 개념 (Heap, Garbage Collection).  

**예제**: 태스크 시스템의 빈번한 쿼리에 캐시 구현.  

### DevOps/클라우드 소개: Docker와 CI/CD
- **Docker**: 컨테이너, 이미지, Dockerfile, Docker Compose.  
- **CI/CD**: GitHub Actions로 빌드 및 배포 파이프라인 설정.  

**예제**: 태스크 앱의 Dockerfile 생성 및 GitHub Actions로 배포.  

### 관찰 가능성
- **도구**: Prometheus (메트릭), Grafana (시각화), ELK Stack (로그).  
- **개념**: 성능 모니터링, 중앙화된 로그, 알림.  

**예제**: Prometheus와 Grafana로 태스크의 API 응답 시간 모니터링.  

### 보안: OWASP Top Ten
- **개념**: Injection, 인증 실패, 민감 데이터 노출.  
- **실습**: 입력 검증, 정화, 안전한 설정.  

**예제**: 태스크 API를 SQL Injection과 XSS로부터 보호.  

### 최종 프로젝트
**고급 태스크 관리 시스템**  
- 백엔드: 4단계 태스크 API를 마이크로서비스(태스크와 사용자)로 강화.  
- 아키텍처: Clean Code, SOLID, Design Patterns(예: Strategy)로 리팩토링.  
- 동시성: ExecutorService로 보고서를 병렬 처리.  
- **선택 사항**: RabbitMQ를 통한 마이크로서비스 간 통신 및 빈번한 쿼리를 위한 Redis 캐싱 추가.  
- DevOps: Docker로 패키징, GitHub Actions로 CI/CD 설정.  
- 관찰 가능성: 메트릭을 위해 Prometheus와 Grafana 추가.  
- 보안: OWASP Top Ten에 대한 보호 구현.  
- Git: 기능별 commit (예: `feature/microservices`, `feature/concurrency`).  
- 공개: GitHub에 자세한 README(설정, 아키텍처, 배포)와 함께 공개.  

### 리소스
- *The Pragmatic Programmer* (책)  
- *Effective Java* (책)  
- *Java Concurrency in Practice* (책)  
- [Spring Cloud Documentation](https://spring.io/projects/spring-cloud)  
- [RabbitMQ Tutorials](https://www.rabbitmq.com/getstarted.html)  
- [Redis University](https://university.redis.com/)  
- [Docker Official Docs](https://docs.docker.com/)  
- [Prometheus Documentation](https://prometheus.io/docs/introduction/overview/)  
- [Grafana Documentation](https://grafana.com/docs/)  
- [ELK Stack Guide](https://www.elastic.co/what-is/elk-stack)  
- [OWASP Top Ten](https://owasp.org/www-project-top-ten/)  
- [GitHub Actions Documentation](https://docs.github.com/en/actions)  