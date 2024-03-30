# README

## 概要

- railsのtodoアプリケーションです
  - Ruby version
    - 3.2.2

## ローカルでの環境構築方法

1. このリポジトリをクローン `git clone https://github.com/nabe-pot/rails-docker.git`
2. クローンしたリポジトリのディレクトリに移動 `cd rails-docker`
3. `docker-compose up -d` にて、コンテナを起動
4. 起動したコンテナにログイン `docker-compose exec web bash`
5. データベースを作成 `rails db:create`
6. データベースにテーブル定義を作る `rails db:migrate`
7. コンテナからログアウト `exit`
8. コンテナを再起動 `docker-compose restart`
9. ブラウザからlocalhost:3000にアクセスし、アプリケーションが起動していることを確認
