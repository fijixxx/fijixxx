# プロフィール

## 概要

- AWS 環境におけるエンジニアリング全般に強みがあります
  - AWS 認定ソリューションアーキテクト - アソシエイト 取得済み
  - EC2 に Linux 系 OS の Web サーバーを立てて作る系が特に得意です
- 業務で Docker を使う知見をためたいです
- JavaScript が好きです。あまり業務では使えてないのですが・・・
- 人生で一番書いている言語は PHP です

## スキル

### 言語

- JavaScript(Node.js, React, Next.js, Angular, Vue.js, Jest)
- Python(Unittest)
- PHP(5, 7, ZendFramework, Smarty, WordPress)
- Java(8, Struts2, Tomcat)
- Ruby(RubyOnRails4, Minitest)
- HTML/CSS(Sass, Stylus, Gulp)
- Shell(Bash, Zsh)
- Vim

### DB

- PostgreSQL, MySQL, Oracle, SQLServer, DynamoDB

### クラウド

- AWS(EC2, VPC, Route53, API Gateway, ECS, CodeCommit, CodePipeline, CodeBuild, CodeDeploy, S3, IAM, Cognito, Lambda, Cloud Formation, Cloud Watch, Cloud Trail)

### その他

- Docker, GitLab, GitHub, Heroku, Apache, Nginx, Amazon Linux2, CentOS

### 保有資格など

#### AWS

- AWS 認定 ソリューションアーキテクト - プロフェッショナル
- AWS 認定 DevOps エンジニア - プロフェッショナル
- AWS 認定 ソリューションアーキテクト - アソシエイト
- AWS 認定 デベロッパー - アソシエイト
- AWS 認定 SysOps アドミニストレーター - アソシエイト

---

## 業務経歴書

### サーバレス業務システム開発【JavaScript, Vue.js, Python, AWS】（2020）

#### 案件概要:

社会保険系法人様の業務システムの運用コスト削減のため、運用プラットフォームの AWS 移行、サービスのサーバレス化、および運用の自動化を目標とした開発を行う

#### 担当:

プロトタイプ作成と同時に発足したテストチームにおいて、上記の観点を実現するテスト手法（自動化やコード化）や CI/CD 手法の PoC（概念実証）とテスト実施を担当

#### 作業実績:

- Selenium(Python)を使用した 結合テスト自動化/ コード化 の提案とテストコード作成時の git フロー導入とテストコード作成
- AWS Lambda(Python) で動作するバックエンドコードに対する 単体テスト自動化/ モック化 手法の提案とサンプルとなるテストコード作成（Unittest/ Nose）
- Vue.js/ Vuex で動作するフロントエンドコードに対する 単体テスト自動化/ モック化 手法の提案とサンプルとなるテストコード作成（Jest）（テストコード作成コストの観点から採用ならず）
- CI/CD を実現する手法としての git ブランチ運用および CodePipeline を使用した CI/CD パイプラインのアーキテクチャ構成の提案と概念実証（上位ベンダーとの役割分担のため採用ならず）
- SAM CLI(CloudFormation)を利用した AWS 環境へのデプロイで利用するテンプレートファイルの作成とデプロイ
- 上記の SAM CLI デプロイをさらに自動化するための bash(shell)スクリプトの作成
- Aurora(Postgrsql)に対して psql クライアントから SQL を利用してテストデータの 確認/ 修正/ 投入
- DynamoDB/ SSM/ Coginito などの AWS サービスに対して AWS CLI を利用してテストデータの 作成/ 修正/ 投入
- CloudWatch Logs を利用した テスト故障の調査/ テスト証跡の取得

### 不動産情報サイト運営企業様の内部ツールの AWS 移行およびメインサイトのテスト故障対応【PHP, Java, AWS】（2020）

#### 案件概要:

お客様先となる不動産情報サイト運営企業様では稼働しているシステムのプラットフォームを AWS へ移行中だが、一部の社内ツールについては移行が積み残されている状況で、その 1 つについて AWS 移行およびシステムの最新化を行うことが決まった

#### 担当:

該当の社内ツールについて AWS 移行とシステムの最新化を担当。また、ツールの移行作業完了後はメインサイトの AWS 移行のテスト故障の調査と対応を担当した

#### 作業実績:

##### ツール移行【PHP, JavaScript, AWS】

- PHP4 で動作していたものを PHP7.1 にバージョンアップし、廃止されていたり非推奨になっていた組み込み関数を使用した処理を最新化
- 移行前の Oracle データベースを参照していた処理や Oracle 用の SQL 文に対して、移行後の参照 DB である Aurora(PostgreSQL) データベースに適した処理へ改修
- 移行後の Aurora では廃止されているテーブルを参照していた一部の処理について、代替として API から情報を取得するように改修
- 放置されていたバグをフィックスし、処理を高速化
- お客様要望により、監査用の操作ログを作成し、S3 バケットに転送する処理を新規実装(Cron と Bash で定時転送)
- E2E テストについて、Puppeteer を使用した自動テスト環境を構築
- ソースコードを VPC 上の EC2(Amazon Linux2) へ配置し、社内ネットワークからのみアクセスできるようにルーティング
- コスト削減のため、CloudWatch Event と AWS Lambda(Python) を組み合わせて、インスタンスを平日の営業時間に合わせて 自動起動/ 停止 するように設定

##### テスト故障対応【PHP, Java】

- テスト故障の原因切り分けと対応を行った
- Java で作成された API サーバーのバグフィックスや、Oracle から PostgreSQL への SQL 書き換えミスの対応

### 業務 Web システム開発【OutSystems】（2019）

#### 案件概要:

建設会社様の次期システムの開発案件。現行システムでは Lotus Notes/ Domino を使用したクライアント/サーバー方式の業務システムが構築されているが、支店や部門ごとに個別にシステムが乱立しているという状態であったため、これらを 1 つにポータルサイトに集約した Web システムを構築し、業務の効率化と運用コストの削減を図る

#### 担当:

システム開発チームで開発を担当した。また、開発にはローコードプラットフォームである OutSystems を使用した

#### 作業実績:

- ローコードプラットフォームである OutSystems を使用した、GUI プログラミングによるシステム開発
- 一部の読み込み負荷の高い処理について、SQLServer データベースに対して実行する SQL を直接作成
- 一部の業務機能について、SE に与えられた要件から詳細設計（画面、処理、エンティティ設計）を行いシステムを作成
