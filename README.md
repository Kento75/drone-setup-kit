# drone-setup-kit
Drone.io(オンプレ版)を使用したGithub接続用Docker-composeモジュール

## セットアップ

①前提条件  
・Docker、Docker-composeのセットアップ済み  
・GithubのAuth認証設定済み

②各種設定値を入力する。  
 「.env」ファイルの各項目に追記

```sh
DRONE_GITHUB_URL=     # 例) https://hogehoge-domainname.com
DRONE_GITHUB_CLIENT=  # Githubで取得したクライアントキー
DRONE_GITHUB_SECRET=  # Githubで取得したシークレットキー
DRONE_SECRET=         # ユニークな文字列
DRONE_HOST=           # ホストのIP

```

③サーバー、クライアントを起動する。

```sh
# プロジェクトディレクトリに移動
$ cd droe-setup-kit

# Docker-composeコマンドを実行
$ Docker-compose up

```

④DRONE_HOSTで設定したURLにアクセス。

