# フェーズ 4 – フレームワークとウェブアプリケーション (3～4ヶ月)

### Spring Boot, Spring Core, Spring Data JPA
- **Spring Core**: Dependency Injection (`@Bean`, `@Autowired`), IoC Container.  
- **Spring Boot**: Auto-Configuration, Starters (`spring-boot-starter-web`, `spring-boot-starter-data-jpa`), `application.yml`.  
- **Spring Data JPA**: Repositories (`CrudRepository`, `JpaRepository`), `@Query`を使用したクエリ、ページネーション。  
- **例**: タスクアプリでタスクを管理するREST endpointsの作成（**CRUD**）。  

### Spring Security (JWT, OAuth2)
- **概念**: Authentication、Authorization、Security Filters。  
- **JWT**: トークンの作成と検証、`JwtAuthenticationFilter`の使用。  
- **OAuth2**: Resource Serverの設定、プロバイダ（例: Google）との統合。  
- **例**: JWTとロール（`ADMIN`, `USER`）でタスクのendpointsを保護。  

### ユニットテストとインテグレーションテスト
- **Unit Tests**: JUnit 5、Mockito（`@Mock`, `@InjectMocks`）、ビジネスロジックのテスト。  
- **Integration Tests**: `@SpringBootTest`, `@WebMvcTest`, テスト用の**H2**データベース。  
- **Testcontainers**: DockerコンテナでのPostgreSQLを使用したテスト。  
- **例**: タスクアプリのサービスとendpointsのテスト。  

### RESTful APIsとSwaggerによるドキュメンテーション
- **REST**: HTTPメソッド、ステータスコード、RESTful原則。  
- **Spring REST**: `@RestController`, `@RequestMapping`, `@PathVariable`。  
- **Swagger**: **springdoc-openapi**の設定、`@Operation`によるアノテーション。  
- **例**: **Swagger UI**でタスクアプリのendpointsをドキュメント化。  

### GraphQLの紹介
- **概念**: Queries、Mutations、Schema。  
- **Spring Boot with GraphQL**: spring-boot-starter-graphqlを使用したセットアップ。  
- **例**: ステータスごとのタスクをリストするGraphQL Queryの作成。  

### 基本的なフロントエンド統合
- **Thymeleaf**: Spring BootでHTMLページをレンダリングするためのテンプレート。  
- **例**: タスクの表示と作成のためのシンプルなウェブインターフェースの作成。  

### ビルドツール: MavenとGradle
- **Maven**: `pom.xml`の構造、依存関係、プラグイン。  
- **Gradle**: `build.gradle`ファイル、タスク、依存関係管理。  
- **例**: MavenとGradleでタスクアプリを設定。  

### プロジェクトのデプロイ
- **プラットフォーム**: Railway、Heroku、AWS（Elastic Beanstalk）。  
- **手順**: JARとしてパッケージ化、GitHub ActionsでCI/CDを設定。  
- **例**: PostgreSQLを使用してRailwayにタスクアプリをデプロイ。  

### 最終プロジェクト
**タスク管理システム**  
- データベース: `Task`（タイトル、説明、ステータス）と`User`テーブル（1:Nの関係）。  
- Java: Spring Boot、Spring Data JPAを使用したREST APIでCRUD。  
- セキュリティ: JWT Authentication、ロール（`ADMIN`, `USER`）。  
- テスト: ユニットテスト（サービス）とインテグレーションテスト（Testcontainersを使用したendpoints）。  
- ドキュメンテーション: endpointsの説明付きのSwagger UI。  
- **オプション**: タスクをリストするGraphQL Queryとインタラクション用のThymeleafインターフェースの追加。  
- Git: 機能ごとのcommit（例: `feature/rest-api`, `feature/security`）。  
- 公開: GitHubにREADME（セットアップ、endpoints、デプロイ）とともに公開。  

### リソース
- [Spring Boot Official Docs](https://spring.io/projects/spring-boot)  
- [Baeldung – Spring Boot Tutorials](https://www.baeldung.com/spring-boot)  
- [Spring Security Guide](https://spring.io/guides/topicals/spring-security-architecture)  
- [Testcontainers Official Docs](https://testcontainers.org/)  
- [Springdoc OpenAPI (Swagger)](https://springdoc.org/)  
- [AWS Free Tier Tutorials](https://aws.amazon.com/free/)  
- [GraphQL Official](https://graphql.org/learn/)  
- [Spring Boot with Thymeleaf](https://spring.io/guides/gs/serving-web-content/)  
- [Railway Documentation](https://docs.railway.app/)  
- [Heroku Dev Center](https://devcenter.heroku.com/)  
- [GitHub Actions Documentation](https://docs.github.com/en/actions)  