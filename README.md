# Slack Remind テキストメイカー

ぽちぽち選択するだけで Slack の `/remind` コマンドを生成できるツールです。

🔗 https://h-kono-it.github.io/slack-remind-maker/

## 使い方

1. 宛先（自分 / チャンネル）を選ぶ
2. リマインドしたい内容を入力する
3. 繰り返しパターン（毎日 / 毎週 / 隔週 / 毎月 / 一度だけ）を選ぶ
4. 時刻を選ぶ
5. 生成された `/remind` コマンドをコピーして、Slack のメッセージ欄に貼り付けて送信する

Slack のリマインドはワークスペースのタイムゾーン設定に従います。

## 技術構成

- 素の HTML / CSS + [Alpine.js](https://alpinejs.dev/) のみで構成された単一ファイル（`index.html`）
- ビルド不要、GitHub Pages（`main` ブランチ）でそのまま配信

## OGP 画像について

`ogp.png` は OGP 用の画像です。デザインを直す際は手元の `ogp-source.html`（HTML/CSSでデザインしたものをヘッドレスブラウザで撮影する用のソース、`.gitignore` 対象）を編集し、Playwright などで 1200×630px のスクリーンショットを撮って `ogp.png` を差し替えてください。
