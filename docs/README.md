# 職務経歴書
## 基本情報

記載欄 | リンク
 --- |  ---
氏名 | 多田 貞剛（ただ さだよし）
生年月日 | 1989/09/19
Twitter | [tada_infra](https://twitter.com/tada_infra)
LinkedIn | [LinkedIn](https://www.linkedin.com/in/sadayoshi-tada-51530145/)
Blog | [継続は力なり](https：//sadayoshi *tada.hatenablog.com/)
Qiita | [Qiita](https://qiita.com/tada_infra)
note | [note](https://note.com/tady0919)
Zenn | [Zenn](https://zenn.dev/sadayoshitada)
SpeakerDeck | [SpeakerDeck](https://speakerdeck.com/sadayoshitada0919/)
Wantedly | [Wantedly](https://www.wantedly.com/id/sadayoshi_tada_b)

## 保有スキル
* AWS でのシステム基盤の設計/実装/運用
* Mackerel の導入および組織内での運用体制の構築
* GitHub Actions , Terraform や Ansible 等による標準化の推進
* 企業内のデータ基盤整備および非エンジニアへのSQL教育推進
* エンジニアの教育およびOJT担当に従事
* 情報システム部門の業務整備、標準化
* 社内勉強会の企画、開催、運営

## 技術スタック
### 言語
* Python
* Shell
* Node.js
* TypeScript

### フレームワーク・その他
* FastAPI
* AWS
* GCP
* Docker
* CloudFormation
* AWS CLI
* Terraform
* Ansible
* Mackerel
* Datadog
* redash
  
## 職務経歴詳細
### 株式会社スナックミー 2020/09〜現在
SRE として AWS 上にあるサービスの安定稼働のために効率的な運用方法を検討したり、障害対応、開発者の生産性向上、システムの状況をモニタリングしてレイテンシーやパフォーマンス改善等をエンジニアリングによって効率化や自動化する業務を担当してます。一部 GCP にて BigQuery を利用したデータ分析基盤にも携わってます。
また、Corporete Enginner として社員の業務アプリケーションの利用方針策定、セキュリティのベースライン向上、社員の入社・退社における業務フロー策定・推進を担当しています。

1, サービス基盤の運用改善
* プロジェクト概要：
  * [自社サービス](https://snaq.me/)のAWS活用における運用課題の改善と開発者体験の向上
    * システムの監視のために Mackerel の導入および開発チーム内での運用体制整備
    * AWS アカウントを用途ごとに分離, SSO をログイン方式に適用
    * 社内システムリリースフローにおける CI/CD の刷新
    * 既存アーキテクチャを変更してセキュリティとネットワークセグメントを最適化
    * API サーバーを EC2 から ECS 化
      * 開発言語を PHP から Python（FastAPI）に変更
    * SLI および SLO の策定(仕掛かり中)
* プロジェクト詳細：
  * AWS のアーキテクチャデザイン、実装、運用
  * リソース管理されていないものを Terrafrom , Ansible を使ったコードによる管理に変換
  * GitHub Actions を使った CI/CD の導入
  * Mackerel の監視の導入と運用ドキュメント作成、開発チームへのレクチャー
  * FastAPI を使ったコンテナの開発・運用、CI/CD の導入、分散トレーシングの設定
  * esa によるドキュメンテーション
* プロジェクト規模：
  * メンバー 1〜3人での開発、運用
* 役割：
  * 各取り組みは私による問題提起から起こり、チームとのネゴシエーション->検証->実装、運用をほぼ1人で行った
  * 適宜 CTO によるレビュー、各チームへの相談、会議体、運用に載せるドキュメンテーション・レクチャーを実施

2, 情報システムエンジニアの業務
* プロジェクト概要：
  * 社内システムへのアクセスとして VPN を導入してセキュアなやりとりをするよう改善
  * 社員の業務アプリケーションのセキュリティベースラインを上げるために二段階認証の設定展開、レクチャー
  * 業務アプリケーションの利用の業務フローの策定
* プロジェクト詳細：
  * 経営層が別々で業務アプリケーションのアカウント発行をしていたところを専門担当者を私に統一化
  * AWS Client VPN の検証、導入、運用
  * AWS SSO と連携して認証機構を採用
  * esa によるドキュメンテーション
  * 利用者へのレクチャー
* プロジェクト規模：
  * メンバー 1〜2人での開発、運用
* 役割：
  * CEO およびバックオフィス担当への私による問題提起から起こり、検証->実装、運用を1人で行った
  * 利用者へのレクチャーおよびヘルプを適宜実施
  * 業務アプリケーションに関する疑問、不明点のフォローアップ

3, 組織内のデータ活用のための基盤構築、運用および非エンジニアの教育支援
* プロジェクト概要：
  * 社内のデータ活用を行うために各種ツール整備、データの ETL、レクチャーを実施
* プロジェクト詳細：
  * データ分析としてクライアントアプリから SQL をデータベースに直接投げていたところを readash に変更
    * データソースもデータベースだけでなく BigQuery , Athena など分析したいデータに応じて変更
  * データ基盤の運用のためにデータの転送や ETL を実施
  * esa によるドキュメンテーション
  * ツールごとに利用者へのレクチャー
  * 非エンジニアへの SQL 勉強会を開催
* プロジェクト規模：
  * メンバー 1〜2人での開発、運用
* 役割：
  * 既存メンバー 3人 がやっていた取り組みを引継ぎ、メインメンバーとして1人でアクションした
    * 適宜メンバーと相談、情報の共有を行った
  * 利用者へのレクチャーおよびヘルプを適宜実施

### 株式会社サーバーワークス 2016/02〜2020/08
AWSでシステムを構成するにあたっての要件定義、設計、実装、テスト支援、運用業務に携わっていました。
また、携わった代表的なプロジェクトについて3つ記載します。

1, グループ各社で利用するクラウドプラットフォームの設計・実装・テスト支援
* プロジェクト概要： 
 * 某企業のグループ各社が利用するクラウドプラットフォームの利用方針の策定、設計・実装・テスト支援を担当
 * サブリーダーとして参画

* 主な技術スタック：
  * 利用AWSサービス： VPC ,EC2 ,ELB ,S3 ,Lambda ,API Gateway ,CloudFormation ,CloudTrail ,AWS Config ,CloudWatch
  * 言語：Python
  * 利用ツール：Backlog ,Serverless Framework ,Mackerel ,JP1

2, SREチームでのCI/CDパイプラインの設計、実装支援
* プロジェクト概要： 
 * 某企業のプロジェクトにおけるSREチームとしてインフラに関する業務および他のチームと連携してCI/CDパイプラインの方針策定、設計、実装を担当
 * メンバーとして参画

主な技術スタック：
利用AWSサービス： VPC ,EC2 ,Lambda ,ECS ,Fargate ,ECR ,ELB ,S3 ,DynamoDB ,AWS IoT ,API Gateway ,CodeBuild ,CloudFormation ,Cloud9 ,Kinesis Streams ,GuardDuty ,CloudTrail ,AWS Config ,CloudWatch
言語：Java ,Python
利用ツール：GitLab ,Jenkins ,Redmine ,Ansible ,Docker ,AWS SAM ,Microsoft Teams ,Microsoft Sharepoint

3, スマートフォン決済アプリの実行基盤の設計、構築、運用
* プロジェクト概要： 
 * スマートフォン決済アプリの実行基盤の設計、構築およびそのAWS の権限方針の策定、運用ルールの策定、実装
 * サブリーダーとして参画
 * アプリケーションのリリース後はプロジェクトの運用上の課題および内部の運用業務の最適化に従事

* 主な技術スタック：
  * 利用AWSサービス： VPC ,EC2 ,Lambda ,ECS ,Fargate ,ECR ,ELB ,S3 ,DynamoDB ,EFS ,AutoScaling ,Resshift ,DataPipeline ,RDS・Aurora ,API Gateway ,CodeCommit ,CloudFormation ,CloudFront ,Kinesis Streams ,AWS WAF ,GuardDuty ,CloudTrail ,AWS Config ,CloudWatch
  * 利用ツール：Docker ,CircleCI ,DataDog ,Scutum ,Backlog ,Slack ,Box ,JP1

### 株式会社グローバルワイズ 2013/05〜2016/01

1, 自社ERPパッケージの保守対応
 * メンバーとして参画
 * 手順書に従ってモジュールのアップロードおよびデプロイ
 * ソースコードのデバッグを行いながら改修対応
* 主な技術スタック
  * 言語： Java
  * ミドルウェア： Apache ,Tomcat

2, ERPパッケージの導入・保守業務
 * メンバーとして参画
 * 客先もしくは社内で手順書に従って ERP パッケージソフトの定期パッチ適用の保守対応
 * ERPパッケージの導入におけるサーバー、ミドルウェア（ WebSphere , Oracle ）のセットアップおよび保守
* 主な技術スタック
  * 言語： Windows PowerShell , COBOL , Java
  * ミドルウェア： WebSphere ,Oracle Database 10,11 g
  * OS：Windows Server 2003/2008/2012

3. 仮想化基盤のサーバー設計・構築
 * メンバーとして参画
 *大手マーケティング会社様Webサイト基盤更改におけるサーバー設計・構築
 *主にアプリケーションのミドルウェア（Apache ,WebLogic ,Oracle）の設計・構築および性能試験などを担当
* 主な技術スタック：
  * 言語： bash
  * ミドルウェア： Apache2.2 ,WebLogic ,Oracle 11 g /12 g
  * OS： Red Hat Enterprise 6
  * 仮想化ソフト： VSphere

### 株式会社イクス 2012/04〜2013/03

## 業務外活動
### 各種勉強会での登壇
* AWS DevDay Online（2020/10/21）
  * エンジニアおよび非エンジニアがデータを活用しようとしているもののシステムや組織的な課題があり改善を行った事例を話した。
  * [データドリブンな組織を目指す、AWSを活用したデータ分析基盤の取り組み](https://speakerdeck.com/sadayoshitada0919/aws-based-data-analytics-infrastructure-initiatives-for-a-data-driven-organization)
* JAWS-UG 朝会#15 （2020/11/18）
  * AWSアカウントが1つしかないことによる開発のしづらさ、開発効率向上のために用途に応じて分割して開発体験の向上の取り組み事例を話した。
  * [AWS Organizations と一緒にはじめるアカウント分離](https://speakerdeck.com/sadayoshitada0919/starting-account-separation-with-aws-organaizations)
* July Tech Festa 2021（2021/01/24）
  * JAWS-UGでの発表を推進した結果と運用で実践している取り組み事例を話した。
  * [スタートアップ企業でのAWS マルチアカウント運用の実践と普及](https://speakerdeck.com/sadayoshitada0919/practice-and-dissemination-of-aws-multi-account-operation-in-a-start-up-company)
* コネヒトマルシェオンライン「機械学習・データ分析」（2021/02/25）
  * 会社でのデータ活用に向けての改善にあたった取り組みを話した。
  * [スタートアップ企業でのデータ活用に向けての取り組み](https://speakerdeck.com/sadayoshitada0919/working-with-startups-to-leverage-data)
* JAWS DAYS 2021 re：Connect（2021/03/20）
  * 開発者が安心かつスムーズなリリースフローを作り、開発生産性を向上させたいと言う課題感からリリースフロー刷新の取り組みを話した。
  * [スタートアップ企業での散乱した システムリリースフローをととのえる話](https://speakerdeck.com/sadayoshitada0919/maintainthe-system-release-flow)

### 技術記事の寄稿および執筆
* [Amazon Web Servicesのシン・ノウハウ](https://gihyo.jp/magazine/SD/archive/2016/201611)
* [日経クラウドファースト Amazon VPC / AWS Direct Connect ](http://itpro.nikkeibp.co.jp/atclncf/service/00006/071500001/)
* [実践CDK TypeScriptでインフラもアプリも！](https://booth.pm/ja/items/1881928)

### その他
* [Podcast](https://anchor.fm/y2-radio)
* [Mackerel アンバサダー](https://sadayoshi-tada.hatenablog.com/entry/2021/03/15/110000)
  * [CRE TGIF](https://hatena.connpass.com/event/207279/)
* 取得資格
  * [AWS](https://www.credly.com/users/sadayoshi-tada.5e7c1af1)
  * Python3エンジニア検定
  * LPIC Level1