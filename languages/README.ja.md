## フェーズ1 – Javaの基礎（1～2ヶ月）
言語の基礎

プリミティブデータ型

制御構造（if/else、switch）

ループ（for、while、do-while）

メソッドと変数のスコープ

配列と基本的なコレクションの紹介

例外処理の紹介（try/catch、throws、カスタム例外）

Git/GitHub（基本的なバージョン管理）

📚 リソース：
* Oracle Java Tutorials: https://docs.oracle.com/javase/tutorial/
* Exercism.io: https://exercism.org/tracks/java
* Java Programming MOOC by the University of Helsinki: https://java-programming.mooc.fi/
* Git - The Simple Guide: https://rogerdudler.github.io/git-guide/
* GitHub Docs: https://docs.github.com/en/get-started
* Beecrowd: https://www.beecrowd.com.br

## フェーズ2 – オブジェクト指向プログラミング（2～3ヶ月）
クラスとオブジェクト（修飾子、属性、メソッド）

インターフェース

抽象化

カプセル化

継承

ポリモーフィズム

データ構造の紹介（リスト、キュー、スタック、マップ）

基本的なアルゴリズム（検索、ソート、再帰）

LeetCode/HackerRankでデータ構造とアルゴリズム（DSA）の問題を解く

📚 リソース：
* Oracle Java Tutorials (OOP): https://docs.oracle.com/javase/tutorial/java/concepts/
* Baeldung (Java OOP): https://www.baeldung.com/java-oop
* LeetCode: https://leetcode.com/
* HackerRank (Java Track): https://www.hackerrank.com/domains/java
* Khan Academy (Algorithms): https://www.khanacademy.org/computing/computer-science/algorithms
* Head First Java (Book)

## フェーズ3 – 主要なフレームワーク（3～4ヶ月）
Spring Boot

Spring Data JPA

Spring Security（認証/認可、JWT、OAuth2）

Hibernate（ORM）

MavenとGradle（ビルドおよび依存関係管理）

JUnit + Mockito（単体テストおよび統合テスト）

Testcontainers（実際のデータベースを使用したテスト）

少なくとも1つの完全なプロジェクトをAWSにデプロイ（またはRailway/Heroku、ただしAWSの方が重要）

📚 リソース：
* Spring Boot Official Documentation: https://spring.io/projects/spring-boot
* Spring Guides: https://spring.io/guides
* Baeldung (Spring Boot): https://www.baeldung.com/spring-boot
* JUnit: https://junit.org/junit5/
* Mockito: https://site.mockito.org/
* Maven: https://maven.apache.org/
* Gradle: https://gradle.org/
* Testcontainers: https://testcontainers.org/
* AWS Free Tier Tutorials: https://aws.amazon.com/free/
* Railway.app: https://railway.app/

## フェーズ4 – データベース（2ヶ月）
SQLの基礎

PostgreSQLおよびMySQL（リレーショナル）

Hibernate + JPAの実践

データベース移行（Flyway/Liquibase）

MongoDBおよびSpring Data Mongo（NoSQL）

インメモリキャッシュとRedis

メッセージング統合（Kafka/RabbitMQ – 任意だが非常に評価される）

GraphQLの学習（グローバル企業での強いトレンド）

インデックス作成とクエリ最適化の学習

📚 リソース：
* SQLBolt: https://sqlbolt.com/
* Mode SQL Tutorial: https://mode.com/sql-tutorial/
* PostgreSQL Official Docs: https://www.postgresql.org/docs/
* MySQL Official Docs: https://dev.mysql.com/doc/
* Flyway: https://flywaydb.org/
* Liquibase: https://www.liquibase.org/
* MongoDB University: https://learn.mongodb.com/
* Practical MongoDB Aggregations (Free eBook)
* Redis University: https://university.redis.com/
* Apache Kafka: https://kafka.apache.org/documentation/
* RabbitMQ: https://www.rabbitmq.com/tutorials/
* GraphQL Official: https://graphql.org/
* Use The Index, Luke! (SQL Indexing): https://use-the-index-luke.com/

## フェーズ5 – システムアーキテクチャ（3ヶ月）
クリーンコードの原則を適用したプロジェクト

Javaで一般的に使用されるデザインパターン（ファクトリ、シングルトン、ビルダー、ストラテジー、オブザーバーなど）

SOLIDおよびコーディングのベストプラクティス

クリーンアーキテクチャ

テストケースおよびTDD

Swaggerを使用したAPIドキュメンテーション

外部APIとの統合（例：Spring OpenAI）

DevOps/クラウドの紹介：

DockerおよびDocker Compose

AWSまたはGCPへのデプロイ

GitHub Actionsを使用したCI/CD

システム設計の学習（スケーラビリティ、高可用性、サービス間通信）

Kubernetesの基礎を学ぶ

📚 リソース：
* Refactoring Guru (Design Patterns): https://refactoring.guru/design-patterns/java
* MartinFowler.com (Architecture): https://martinfowler.com/
* Docker Official Docs: https://docs.docker.com/
* GitHub Actions: https://docs.github.com/en/actions
* Kubernetes Official Docs: https://kubernetes.io/docs/
* Prometheus: https://prometheus.io/docs/
* Grafana: https://grafana.com/docs/
* Elastic Docs: https://www.elastic.co/guide/
* System Design Primer: https://github.com/donnemartin/system-design-primer
* Clean Architecture (Book, Robert C. Martin)
* Designing Data-Intensive Applications (Book, Martin Kleppmann)


最終プロジェクト（学習の定着）
認証付きの完全なCRUD

独立した認証モジュール（JWT + OAuth2）

ファイルおよび画像のアップロード

データベース間のデータレプリケーション

Swaggerを使用したAPIドキュメンテーション

クラウドへのデプロイ（例：AWSまたはRailway）

（ボーナス）Spring Cloudを使用したマイクロサービスアーキテクチャ

例：

CRUD + 認証 → CI/CDパイプラインを使用してAWSにデプロイ

ファイルおよび画像のアップロード → AWS S3を使用

データレプリケーション → PostgreSQL + MongoDB

ドキュメント化されたAPI（Swagger + README）

## 追加トピック（自信がある場合）
String、StringBuilder、StringBufferの使用

Stream APIおよびOptional

SLF4J/Logbackを使用したロギング

Spring Boot Profiles + Actuator

トランザクションの概念（ACID）

インデックスおよび実行計画（EXPLAIN）

ヘキサゴナルアーキテクチャ

オブザーバビリティの紹介：集中型メトリクスおよびログ（Prometheus、Grafana、またはELK）

レジリエンス：サーキットブレーカー（Resilience4j）

セキュリティ：OWASPトップ10（SQLインジェクション、XSS、CSRFなど）およびその防止方法

📚 リソース：
* Oracle Documentation (Stream API, Optional): https://docs.oracle.com/javase/8/docs/api/
* SLF4J: https://www.slf4j.org/
* Resilience4j: https://resilience4j.readme.io/
* OWASP Top Ten: https://owasp.org/www-project-top-ten/
* Loiane Groner: https://www.youtube.com/@LoianeGroner
* DevDojo: https://www.youtube.com/@DevDojo