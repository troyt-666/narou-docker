# Narou.rb Docker Image

Narou.rb を Docker で実行するための Dockerイメージ<br>
最終的な参照先は同じ作者製のfork先である [laprusk/narou-docker](https://github.com/laprusk/narou-docker)をベースとしています。 <br>
このページのファイルはquiitaのページの手順の為に準備しました。

# イメージの構成
- Alpine Linux 3.19
- Ruby 3.3.0
- [改造版AozoraEpub3](https://github.com/kyukyunyorituryo/AozoraEpub3) から AozoraEpub3-1.1.1b22Q.zip
- kindlegen 2.9 (正規ダウンロードじゃない)

# 使い方
最低限以下のファイルを同じディレクトリに保管し、コマンドを実行

- Dockerfile
- docker-compose.yml
- init.sh
- narou-3.8.2.patch

```sh
$ docker compose up -d
```

自動的に WEB UI が起動します。<br>
http://localhost:9200/ にアクセスしてください。