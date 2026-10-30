# ZWA CMS site

ZWA CMS（Zero Web Admin CMS）のサイトを GitHub Actions から公開するためのリポジトリです。予約投稿の時刻になると、ZWA CMS の予約用の Worker がこのリポジトリのワークフローを起動してサイトを公開します。

記事・画像・テーマはここには入っていません（Cloudflare の D1・R2 にあります）。

## 使い方

1. このテンプレートからリポジトリを作ります（「Use this template」→「Create a new repository」）
2. ZWA CMS の「サイト情報」→「GitHub 連携」で、作ったリポジトリを連携します

Actions のシークレット（`CLOUDFLARE_API_TOKEN` / `CLOUDFLARE_ACCOUNT_ID` / `ZWA_SITE_ID`）は ZWA CMS が設定します。自分で設定する必要はありません。

## 中身

- `.github/workflows/zwa-publish.yml` … サイトを公開するワークフロー。Actions の画面から手動でも実行できます

ワークフローは手を加えても構いません。ZWA CMS はワークフローのファイル名（`zwa-publish.yml`）で起動するので、名前は変えないでください。
