Webアプリケーションエンジニア研修
============================
![mindmap](https://raw.githubusercontent.com/plusfor/engineer-textbook/master/summary_mindmap.png)
https://mm.tt/701022538?t=SqbrHsTv7w

開発経験の浅い新入社員が、
Webアプリケーションエンジニアとして現場はいることができるようになるため、
また継続的に成長できるようになるため、
習得していることが望ましい技術や心構えをまとめています。

各項目について
具体的に現場で求められるポイントや将来的に求められそうなポイント、
参考となる書籍やweb上の情報を記載しています。

はじめに
----------------------
研修ではGit, Github, Slackをつかいます。環境を整えましょう。

### Git
#### Gitのインストール
#### .gitconfig
ホームディレクトリに `.gitconfig` ファイルを作成し以下の内容をコピペしましょう。
（メールアドレス等は自分を設定すること）
```
git config --global user.name "xxxxxxxx"
git config --global user.email "xxxxxxxx@plusfor.co.jp"

git config --global core.editor "vim"
git config --global core.pager "less -R"
git config --global help.autocorrect true

git config --global color.ui "auto"

git config --global core.autocrlf false
git config --global core.safecrlf true
git config --global core.whitespace trailing-space,space-before-tab,indent-with-non-tab

git config --global push.default "simple"

git config --list --global
```

### Github
#### Githubアカウントの取得

#### plusforオーガナイゼーションへの参加
アカウントができたら教えて下さい。追加します。

### Slack
#### Slackインストール

#### チームplusforへの参加
以下のURLからJOINしてください。

https://plusfor.slack.com/signup

インターネットの仕組み、プロトコル
----------------------
### HTTP, TCP/IP
- インターネットの仕組みや文化についての理解

#### チェックポイント
- 自宅でインターネットに接続できる
- HTTPが何の略か知っている
- telnetで手打ちHTTP通信を行い、Webページの取得やフォームへのデータ送信ができる
- DNSによる名前解決の仕組みを知っている
- 自分のドメインを持っていてなにか公開している

#### 参考資料
- [書籍] Webを支える技術 -HTTP、URI、HTML、そしてREST (WEB+DB PRESS plus)

### サーバー
- 問題発生時に問題の切り分けや追跡調査を行うための知識
- 環境構築、ミドルウェア、サービスの知識

#### チェックポイント
- Apache, nginxを知っている

### 仮想環境
- 開発環境の整備
- クラウド, IaaS
- 構成管理

#### チェックポイント
- VirtualBox,Vagrant等を使って適当な仮想環境を作れる
- puppet,chefなどの構成管理ツールを使ってプロビショニングを行える
- AWS上にWebサービスを公開できる
- AWS上に大規模Webサービスを想定した環境を構築しデプロイメントパイプラインと監視体制を整備できる

### Webサービス基礎
- SEOやユーザビリティへの配慮

#### 参考資料
- [Web] ニールセン博士のAlertbox https://u-site.jp/alertbox/

VCS
----------------------
### Git
- Gitの概念を理解し、Gitによるソースコードの管理
- Git, Githubを使った共同作業

#### チェックポイント
- git管理しているファイルを変更してcommitできる
- ブランチを作成して作業できる
- ~/.gitconfigに便利なaliasを設定している
- mergeとrebaseの違いを理解している
- revertとresetの違いを理解している

#### 参考資料
- [Web] サルでもわかるGit入門 http://www.backlog.jp/git-guide/

### Github
- pull requestベースの開発
- issueでの議論, pull requestによるレビュー

#### チェックポイント
- 自分の(もしくは共有の)リポジトリにpull requestを出した
- 他人のリポジトリ出したpull requestがマージされた

Web開発
----------------------
### セキュリティ
- セキュリティ的に問題のないアプリケーションの作成

#### チェックポイント
- XSS,CSRF,SQLインジェクションといった基本的な脆弱性の仕組みを理解している
- 書籍「体系的に学ぶ 安全なWebアプリケーションの作り方」の内容を理解している
- OWASP ZAPなどの脆弱性検査ツールを使っている
- 一般公開されているWebサービスの脆弱性を指摘したことがある

#### 参考資料
- [書籍] 体系的に学ぶ 安全なWebアプリケーションの作り方　脆弱性が生まれる原理と対策の実践 (SBクリエイティブ)

### フレームワーク/ツール
- MVCの理解
- フレームワークを利用した開発経験

#### チェックポイント
- MVCが何のことか知っている
- なにかしらMVCフレームワークを使ったことがある
- 簡単なフレームワークを自作したことがある
- オープンソースのフレームワークにコントリビュートしている

#### 参考資料
- [Web] フラットなPHPからフレームワークへ http://www.slideshare.net/brtriver/php-14295877
 - ただのPHPファイルを変更していく過程を追いながらフレームワークの仕組みと必要性を理解できます

プログラミング言語
----------------------
### PHP
- モダンなPHP, PSR, Composer
- 良い設計
- 良いコード
- 良いコメント
- 良いユニットテスト
- 効率のよい開発のための環境づくりやツールの利用

#### 参考資料
- [Web] PHP The Right Way http://ja.phptherightway.com

### JavaScript
- なんちゃってJS対応,jQueryの活用
- ブラウザの開発者ツールを活用した開発
- JSを取り巻くビルドツールやフレームワークの変化

### HTML/CSS
HTML5
Sass

Linux
----------------------
### 基本操作
- SSHの概念やツールの理解
- サーバーにログインして作業する

#### 参考資料
- [書籍] Linuxの教科書　改訂版 （マイコミムック） (MYCOMムック)

プロジェクト管理
----------------------
### チームの一員として
- 作業見積もりや自身の進捗管理、報告
- タスクの洗い出しや分割、スケジューリング
- 要件定義

データ処理
----------------------
### RDB
- RDBのテーブル設計, 正規化などの理解
- パフォーマンスチューニングの知識

### 分散処理
- 分散処理の必要性やツールの知識

### 非同期処理
- 非同期処理の必要性やツールの知識

テスト
----------------------
### システムテスト
- 仕事として必要なテスト作業
- 境界値分析などのテスト技法
- よいバグ報告
- ユーザテストの活用

設計
----------------------
### 設計と成果物
- 画面設計、機能設計
- 状態遷移図、シーケンス図の読み方、書き方

チーム開発
----------------------
### 心構えや知識
- コードレビューの観点や心構え
- ペアプログラミング

情報収集
----------------------
### 情報収集
- 雑誌,ニュース,SNSなどで技術動向をおさえる
- 勉強会にいってやる気を出す
