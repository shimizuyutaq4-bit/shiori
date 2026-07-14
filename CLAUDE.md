# CLAUDE.md — 栞 (shiori)

## このプロジェクト

- 青空文庫リーダーWebアプリ（縦書き読書体験）
- 構成: 単一HTMLファイル（`index.html` にHTML/CSS/JSをすべて内包）
- 公開: GitHub Pages（リポジトリ `shimi-works/shiori`）
- 管理情報: `C:\Users\smzyt\apps\dev-os\projects\`（要件・タスク・バグはdev-os側）

## 開発標準

`C:\Users\smzyt\apps\dev-os\CLAUDE.md` の「全プロジェクト共通 開発標準」に従う。

## このプロジェクト固有のルール

- ファイル分割しない。単一HTML内でセクションコメントで区画を保つ
- 青空文庫の取得はCORSの制約に注意（プロキシ利用箇所は不安定前提でエラーハンドリング）
- localStorageに読書位置・本棚を保存。スキーマ変更時は既存データのマイグレーションを書く
- スマホでの縦書き表示・タップ操作を最優先で確認する

## 動作確認

- **編集後は必ず verify-single-html スキルで検証**（構文チェック＋Edgeヘッドレス起動確認）。「編集できた」だけで完了報告しない
- リリース前: `dev-os/templates/checklists/release.md` を実施
