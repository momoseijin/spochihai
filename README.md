# spochihai

このアプリは、現在Spotifyで再生している曲をmstdn.jpで簡単にトゥートするためのツールです。

# 実行方法

## 環境

実行には、DockerおよびDocker Composeが必要です。

	$ docker compose build

## 設定

.env を .env.example を参考にして編集します。

Spotifyのトークンの取得方法は、[Spotify for Developers](https://developer.spotify.com/documentation/web-api/quick-start/)を参照。

	$ cp example.env .env
	$ vim .env

## 起動

.envのSPCHI\_PORTで設定したポートでHTTPサーバが起動される。 CTRL+Cで終了

	$ docker compose up

以下の方法でバックグラウンド動作になる。

	$ docker compose up -d

終了は以下の通り

	$ docker compose down


# License

MIT

except [\_reset.scss](src/client/sass/_reset.scss) (public domain)

