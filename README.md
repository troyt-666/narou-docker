# Narou.rb Docker Image

Narou.rb を Docker で実行するための Docker イメージ<br>
最終的な参照先は同じ作者製の fork 先である [laprusk/narou-docker](https://github.com/laprusk/narou-docker)をベースとしています。 <br>
このページのファイルは quiita のページの手順の為に準備しました。

# イメージの構成

- Alpine Linux 3.19
- Ruby 3.3.0
- [改造版 AozoraEpub3](https://github.com/kyukyunyorituryo/AozoraEpub3) から AozoraEpub3-1.1.1b23Q.zip

# 使い方

最低限以下のファイルを同じディレクトリに保管し、コマンドを実行

- Dockerfile
- docker-compose.yml
- init.sh

```sh
$ docker compose up -d
```

自動的に WEB UI が起動します。<br>
http://localhost:9200/ にアクセスしてください。
