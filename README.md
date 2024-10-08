# nicoarch

[nicoarch-app](https://github.com/tksnnx/nicoarch-app.git)<br/>
[nicoarch-worker](https://github.com/tksnnx/nicoarch-worker.git)

ニコニコ動画の動画ファイル・メタデータ・コメントデータをアーカイブするツール

## 使い方

1. `.env.sample`を`.env`にコピーし、編集する。<br>
    `NICONICO_MAIL`: ニコニコ動画のメールアドレス<br>
    `NICONICO_PASSWORD`: ニコニコ動画のパスワード<br>
    `WORKER_COUNT`: workerの数 (コメント取得に難があるため1推奨)<br>
    `NGINX_PORT`: ホストするポート番号(デフォルト: 8080)<br>
    `CONTENTS_DIR`: 動画ファイルや画像ファイルを保存するディレクトリ(デフォルト: ./contents)

2. 下記コマンドを実行し、localhost:8080にアクセスすると使用できる。

    ```sh
    docker compose up -d --build
    ```

## ライセンス
[MIT License](LICENSE)
