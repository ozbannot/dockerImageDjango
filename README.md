# dockerImageDjango

## 環境
・Docker<br>
※ Docker Desktopをinstall<br>
https://docs.docker.com/desktop/

## 構成
```
◆アプリケーション構成群
・DB
・Buildinserver
・Python
◆Docker-compose.yml(アプリケーション構成群記述ファイル)
◆app(アプリケーション格納場所)
```

## 構成スペック
```
・DB
- Postgre
・Python
- v3
・Django
- v3.2
```

## 環境構築
```
① git clone {this repository} cd {this repository}

② docker compose up -d --build

③ appにアプリケーションロジック記述

```

## アクセス
```
http://127.0.0.1:8000/
```

## Dockerコマンド
```
・Dockerfileの書き換えなどのビルド処理の変更をイメージに反映させる
docker-compose up --build
・イメージを元にコンテナを起動する(Dockerfileの変更がなければこっちでOK)
docker-compose up
・option -d
デタッチ、バックグラウンド起動
・コンテナを落とす
docker-compose down
```
