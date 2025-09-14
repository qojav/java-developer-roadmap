# 6단계 – 최종 프로젝트 (진행 중)

### 프로젝트 1: 인증을 포함한 완전한 CRUD
- **목표**: 안전한 인증과 테스트를 포함한 견고한 RESTful API 구축.  
- **기술**: Spring Boot, Spring Data JPA (PostgreSQL), Spring Security (JWT), JUnit 5, Testcontainers.  
- **기능**: 엔티티(예: 태스크, 사용자)에 대한 CRUD, 롤(ADMIN, USER)을 사용한 인증, Swagger로 문서화.  
- **선택 사항**: 태스크 보기/관리를 위한 Thymeleaf 인터페이스 추가.  
- **예제**: 프로젝트 관리 API (엔티티: `Project`, `Task`, `User`)를 보호된 endpoints로 구축.  

### 프로젝트 2: 파일 업로드
- **목표**: 프로젝트 1의 API에 파일 업로드 기능 추가.  
- **기술**: Spring Boot (`MultipartFile`), Amazon S3 또는 로컬 스토리지, 파일 검증.  
- **기능**: 태스크와 관련된 이미지/문서 업로드, 타입/크기 검증.  
- **예제**: API에서 태스크를 위한 첨부 파일(예: PDF, PNG) 업로드 허용.  

### 프로젝트 3: 클라우드 배포
- **목표**: CI/CD를 사용하여 클라우드 플랫폼에 API 배포.  
- **기술**: Railway, Heroku, 또는 AWS (Elastic Beanstalk), GitHub Actions, Docker.  
- **기능**: JAR/Docker로 패키징, 환경 변수 설정, 배포 자동화.  
- **선택 사항**: 빈번한 쿼리 최적화를 위해 Redis로 캐싱 구현.  
- **예제**: PostgreSQL과 CI/CD를 사용하여 Railway에 프로젝트 API 배포.  

### 프로젝트 4: 마이크로서비스
- **목표**: 프로젝트 1의 API를 오케스트레이션된 마이크로서비스로 분할.  
- **기술**: Spring Cloud (Eureka, Gateway), Docker Compose, REST 통신.  
- **기능**: `Tasks`와 `Users`를 위한 마이크로서비스, 서비스 디스커버리 포함.  
- **선택 사항**: 마이크로서비스 간 비동기 통신을 위해 RabbitMQ 사용.  
- **예제**: 태스크와 사용자 로직을 두 개의 서비스로 분리하고 Docker로 오케스트레이션.  

### 프로젝트 5: 외부 API 통합
- **목표**: 외부 API를 소비하여 기능 강화.  
- **기술**: Spring RestTemplate 또는 WebClient, API 인증(예: OAuth2).  
- **기능**: 공개 API와 통합(예: SendGrid를 통해 이메일 알림 전송).  
- **선택 사항**: 태스크/사용자를 검색하는 GraphQL Query 추가 및 MongoDB에 메타데이터 저장.  
- **예제**: 태스크 완료를 위한 이메일 알림 추가.  

### 포트폴리오 모범 사례
- **Git**: 기능별 commit (예: `feature/crud`, `feature/upload`), 명확한 브랜치.  
- **문서화**: 설명, 설정, endpoints, 배포, 스크린샷이 포함된 README.  
- **공개**: GitHub에 오픈소스 라이선스(예: MIT)로 호스팅.  

### 리소스
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