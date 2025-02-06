# Wordpress検証用

## 前提条件

- Docker Desktop for Mac がインストールされていること

## 環境構築手順

1. リポジトリのクローン

```bash
git clone https://github.com/takyafumin/sample-wordpress-apache.git
cd sample-wordpress-apache
```

2. Dockerコンテナの起動

```bash
docker compose up -d
```

3. WordPressの初期設定

- http://localhost:8000 にアクセス
- 表示される画面に従って初期設定を実施

## 環境情報

- WordPress: 6.7.1 (PHP 8.3 Apache)
- MySQL: 8.0.41
- ポート: 8000

### データベース設定

|      項目      |    値     |
| -------------- | --------- |
| データベース名 | wordpress |
| ユーザー名     | wordpress |
| パスワード     | wordpress |
| ホスト         | db:3306   |

### DBツール

- adminer
    - http://localhost:8080
    - ユーザー名: wordpress
    - パスワード: wordpress
    - データベース: wordpress   
