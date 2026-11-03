# ZWA CMS site

[ZWA CMS](https://github.com/imo-tikuwa/zwa-cms) のサイト用のテンプレートリポジトリです。

- `theme/`: サイトのテーマ。ZWA CMS の「テーマ」画面で編集すると、保存ごとにここへコミットされます。ここに置いたファイルが既定のテーマのファイルを上書きします（書き方は `theme/README.md`）
- `.github/workflows/zwa-publish.yml`: サイトを公開するワークフロー。予約投稿の時刻になると ZWA CMS が起動します

## 注意

どちらも ZWA CMS が使っています。

- `theme/` は、クローンして編集し、push しても構いません。ZWA CMS は「テーマ」画面を開いたときに最新を読み込みます。ZWA CMS で未保存の変更があるときに push すると、ZWA CMS 側の保存は止まります（どちらかの変更が消えないように）
- `.github/workflows/zwa-publish.yml` は、ファイル名を変えたり削除したりしないでください。予約投稿が動かなくなります。中身を変えると、公開がうまくいかなくなることがあります
