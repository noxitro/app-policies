# app-policies

個人で作って使っているアプリの案内ページとプライバシーポリシーを、GitHub Pages で公開するためのリポジトリ。

公開先: https://noxitro.github.io/app-policies/

## なぜ要るか

Google の OAuth 同意画面を「本番環境」にするには、公開されたホームページとプライバシーポリシーの URL が要る
(テストのままだと許可が 7 日で切れる)。そのための置き場。

| ページ | 使っている所 |
|---|---|
| `index.html` | Google Cloud プロジェクト `book-log-sync` の同意画面の「ホームページ」 |
| `book-log/privacy.html` | 同じく「プライバシーポリシー」 |

承認済みドメインは `noxitro.github.io`。

## アプリを足すとき

`<アプリ名>/privacy.html` を足し、`index.html` に 1 項目足す。中身はアプリが求める権限とその使い道、アプリが端末に残して利用者が書き出せる情報(不具合の報告など)の扱いを書く。
