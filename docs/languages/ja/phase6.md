# フェーズ 6 – 最終プロジェクト (継続中)

### プロジェクト 1: 認証付き完全なCRUD
- **目的**: 安全な認証とテストを備えた堅牢なRESTful APIを構築する。  
- **技術**: Spring Boot、Spring Data JPA (PostgreSQL)、Spring Security (JWT)、JUnit 5、Testcontainers。  
- **機能**: エンティティ（例: タスク、ユーザー）のCRUD、ロール（ADMIN、USER）による認証、Swaggerによるドキュメンテーション。  
- **オプション**: タスクの表示/管理のためのThymeleafインターフェースを追加。  
- **例**: プロジェクトを管理するAPI（エンティティ: `Project`, `Task`, `User`）を保護されたendpointsで構築。  

### プロジェクト 2: ファイルアップロード
- **目的**: プロジェクト1のAPIにファイルアップロード機能を追加する。  
- **技術**: Spring Boot（`MultipartFile`）、Amazon S3またはローカルストレージ、ファイル検証。  
- **機能**: タスクに関連する画像/ドキュメントのアップロード、タイプ/サイズの検証。  
- **例**: APIでタスクのための添付ファイル（例: PDF、PNG）のアップロードを許可。  

### プロジェクト 3: クラウドデプロイ
- **目的**: CI/CDを使用してクラウドプラットフォームにAPIをデプロイする。  
- **技術**: Railway、Heroku、またはAWS (Elastic Beanstalk)、GitHub Actions、Docker。  
- **機能**: JAR/Dockerとしてパッケージ化、環境変数の設定、自動デプロイ。  
- **オプション**: 頻繁なクエリを最適化するためにRedisでキャッシュを実装。  
- **例**: PostgreSQLとCI/CDを使用してRailwayにプロジェクトAPIをデプロイ。  

### プロジェクト 4: マイクロサービス
- **目的**: プロジェクト1のAPIをオーケストレーションされたマイクロサービスに分割する。  
- **技術**: Spring Cloud (Eureka, Gateway)、Docker Compose、RESTによる通信。  
- **機能**: `Tasks`と`Users`のマイクロサービス、サービスディスカバリ付き。  
- **オプション**: マイクロサービス間の非同期通信にRabbitMQを使用。  
- **例**: タスクとユーザーロジックを2つのサービスに分け、Dockerでオーケストレーション。  

### プロジェクト 5: 外部API統合
- **目的**: 外部APIを利用して機能を強化する。  
- **技術**: Spring RestTemplateまたはWebClient、API認証（例: OAuth2）。  
- **機能**: 公開APIとの統合（例: SendGridを介してメール通知を送信）。  
- **オプション**: タスク/ユーザーを取得するGraphQL Queryを追加し、MongoDBにメタデータを保存。  
- **例**: タスク完了のためのメール通知を追加。  

### ポートフォリオのベストプラクティス
- **Git**: 機能ごとのcommit（例: `feature/crud`, `feature/upload`）、明確なブランチ。  
- **ドキュメンテーション**: 説明、セットアップ、endpoints、デプロイ、スクリーンショットを含むREADME。  
- **公開**: GitHubにオープンソースライセンス（例: MIT）でホスト。  

### リソース
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