# フェーズ 3 – データ持続性とStreams (2～3ヶ月)

### 基本的なSQL
- **DDL**: `CREATE`, `ALTER`。  
- **DML**: `SELECT`, `INSERT`, `UPDATE`, `DELETE`。  
- **Joins**: `INNER`, `LEFT`, `RIGHT`。  
- **Keys**: プライマリキーと外部キー。  
- **正規化**: 1NF、2NF、3NF。  
- **例**: 製品とカテゴリーのテーブルを作成。  

### JDBCとConnection Pool
- **Classes**: `Connection`, `Statement`, `PreparedStatement`, `ResultSet`。  
- Connection Pool（**HikariCP**）の使用。  
- **ベストプラクティス**: `try-with-resources`、`SQLException`の処理。  

### Hibernate + JPAの実践
- **Annotations**: `@Entity`, `@Id`, `@ManyToOne`, `@OneToMany`。  
- **設定**: `persistence.xml`または`application.properties`。  
- `EntityManager`を使用した**CRUD**操作。  
- FlywayまたはLiquibaseによるデータベース移行の紹介。

### NoSQLデータベースの紹介
- **概念**: ドキュメント、コレクション、水平スケーラビリティ。  
- **MongoDB**: セットアップ、MongoRepositoryを使用したCRUD操作。  
- **Spring Data MongoDB**: Spring Bootとの統合。  
- **例**: MongoDBに製品のシステムアクティビティログを保存。

### StreamsとLambda Expressions
- **操作**: `filter`, `map`, `sorted`, `collect`, `forEach`, `reduce`。  
- **例**: 価格で製品をフィルタリングし、名前でソート。  

### OptionalとFunctional Interfaces
- `Optional`: `orElse`, `ifPresent`, `orElseThrow`。  
- **Functional Interfaces**: `Function`, `Predicate`, `Consumer`。  
- **例**: Streamsでデータをフィルタリングするために`Predicate`を使用。  

### 高度なCollections
- **LinkedList**: 効率的な挿入/削除。  
- **TreeMap**: 順序付けられたkey-valueペア。  
- **PriorityQueue**: 優先キュー。  
- **LinkedHashMap**と**Deque**（紹介）。  

### ロギング（SLF4J/Logback）
- SLF4JとLogbackの設定。  
- **レベル**: `INFO`, `DEBUG`, `ERROR`。  
- **例**: Hibernateクエリをログに記録。  

### トランザクションの概念（ACID）
- 原子性、一貫性、分離性、耐久性。  
- JDBC（`commit`, `rollback`）およびHibernate（`@Transactional`）を使用したトランザクション。  

### インデックスと実行計画
- **Indexes**: プライマリ、ユニーク、複合。  
- クエリオプティマイズのための**EXPLAIN**の使用。  
- **例**: 頻繁に検索される列にインデックスを作成。  

### ファイル操作（オプション）
- `Files`, `BufferedReader`を使用した読み書き。  
- **例**: Streamsを使用して製品レポートをCSVにエクスポート。  

### データベーステスト（紹介）
- **H2**と**JUnit**を使用したインテグレーションテスト。  
- **例**: Hibernateを使用したCRUD操作のテスト。  

### 最終プロジェクト
**製品管理システム**  
- データベース: **Product**と**Category**テーブル（1:Nの関係）。  
- Java: JPA（`Product`, `Category`）を使用したクラス、HibernateによるCRUD。  
- **オプション**: MongoDBに製品変更ログを保存。  
- **オプション**: MongoDBに動的な製品属性（例: 技術仕様）を保存。  
- Streams: 製品のフィルタリング/ソート（例: 価格またはカテゴリーによる）。  
- ロギング: データベース操作の監視。  
- Git: 機能ごとのcommit（例: `feature/crud`, `feature/streams`）。  
- GitHubに公開し、説明的なREADMEを付ける。  

### リソース
- [SQLBolt](https://sqlbolt.com/)
- [PostgreSQL Official Docs](https://www.postgresql.org/docs/)  
- [Baeldung](https://www.baeldung.com/)  
- [Use The Index, Luke!](https://use-the-index-luke.com/)
- [Hibernate Official Docs](https://hibernate.org/orm/documentation/) 
- [Baeldung – Logging with SLF4J](https://www.baeldung.com/slf4j)
- [Flyway](https://flywaydb.org/)
- [MongoDB University](https://university.mongodb.com/)