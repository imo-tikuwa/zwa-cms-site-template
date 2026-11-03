# ZWA CMS site

[ZWA CMS](https://github.com/imo-tikuwa/zwa-cms) のサイト用のテンプレートリポジトリです。

- `theme/`: サイトのテーマ。ZWA CMS の「テーマ」画面で編集すると、保存ごとにここへコミットされます。ここに置いたファイルが既定のテーマのファイルを上書きします（書き方は `theme/README.md`）
- `.github/workflows/zwa-publish.yml`: サイトを公開するワークフロー。予約投稿の時刻になると ZWA CMS が起動します。ファイル名は変えないでください
