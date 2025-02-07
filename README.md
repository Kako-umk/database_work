### ☑ 最新コードの取得
このリポジトリの`main`ブランチにはアプリの完成版が含まれています。以下のコマンドで最新の完成コードを取得できます:

bash
git clone https://github.com/Kako-umk/database_work​

---

## プロジェクト構成

- **フロントエンド:** CSS
- **バックエンド:** Flask (Python)
- **データベース:** PostgreSQL
- **環境構築:** Docker

---

## 概要

### プロジェクト名
employee.app

### プロジェクト概要
従業員の情報をデータベースを用いて管理するアプリケーション

### プロジェクト詳細資料
https://1drv.ms/p/c/6fc346af42772e1f/EXQxxzd3sOZLo-6cxE6kLPkBo6Qd9Xdt9X3IU45-ufUnCg?e=4ebfpc
開けない場合はgithub内にある.pptxを確認

---

## 必要な環境変数やコマンド

### 環境
- 事前に[Docker Desktop](https://www.docker.com/ja-jp/products/docker-desktop/)をインストールしておく必要がある。

**環境変数 (.envファイルをプロジェクトのルートに配置する。):**
```
# COMMON
API_PORT=3000
DB_PORT=5432

# PostgreSQL Settings
POSTGRES_USER=guest
POSTGRES_PASSWORD=password
POSTGRES_DB=guest
POSTGRES_HOST=db
```

### コマンド
- このプロジェクトではDockerを使用しているので、`docker`コマンドを使用する。

- **起動**
```bash
docker compose up
```

- **更新ビルド**
```bash
docker compose up --build -d
```

- **コンテナ削除**
```bash
docker compose down --rmi all
```
---

## トラブルシューティング

###　no configuration file provided: not found
実行するディレクトリにDockeccompose.ymlやDockerFileがないため、
GitCloneした後に、そのディレクトリに入って実行する

### docker daemon is not running
Docker Desktop が起動できていないため起動させる。

---
##　参考
https://github.com/urassh/docker-flask-app/
https://prog-8.com/docs/git-env-win
