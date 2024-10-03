# えんつむぎ -御朱印めぐりで紡ぐご縁-
### サービスURL：https://en-tsumugi.com/
![entsumugi](./app/assets/images/ogp2.png)


## サービス概要
神社と御朱印の情報共有サービスです。<br>
神社情報は、都道府県名、御利益カテゴリ、フリーワード、マップからマルチに検索できます。<br>
ログインをすると、御朱印の写真投稿、ブックマーク登録、マイページをご利用いただけます。

## このサービスへの思い
webアプリを開発するにあたり、誰かの課題解決になるサービスや役に立つサービスを作りたいという思いが膨らみました。<br>
また日頃から「何事も縁」と考える自身の価値観から、「縁」をテーマにし、家族が熱心に集めていた御朱印に関する情報を提供できるサービスを作りたいと考え、webアプリ「えんつむぎ」を開発いたしました。

## ユーザー層
- 御朱印に興味がある人、集めている人
- 神社が好きな人

## サービスの差別化ポイント・推しポイント
1. **神社のご利益カテゴリで検索できる**<br>
  「この神社の御朱印がほしい」と思う時、大きな理由となるのが御朱印のデザインもしくは訪れたい神社自体に興味があるかのいずれかであると考えました。<br>
  後者の理由である場合、どんな御利益がある神社なのかということは重要な決め手になると思いますので、神社のご利益別に検索できる機能を実装いたしました。

2. **レスポンシブ対応**<br>
  スマートフォンでの閲覧にも支障がないよう、レスポンシブ対応いたしました。

3. **メイン機能はログインなしで使える**<br>
  サービス利用のハードルを下げるため、メイン機能である検索機能はログインせずに誰でもご利用いただけるようにしました。<br>
  さらにサービスを楽しみたいという方に向けては、ログインすることで投稿機能、ブックマーク機能、マイページ機能などを提供します。


## 機能一覧
< 検索機能 >
  - 都道府県検索
  - ご利益カテゴリ検索
  - フリーワード検索
  - マップ検索

< 認証 >
  - ユーザー登録
  - ログイン機能(devise, Googleログイン)
  - ログアウト機能
  - パスワードリセット機能
  - ユーザー情報編集機能

< メイン >
  - 御朱印写真投稿機能
  - 神社ブックマーク機能


< マイページ >
  - プロフィール表示
  - 投稿一覧
  - ブックマーク一覧


< その他 >
  - Xシェア機能
  - お問い合わせフォーム
  - 利用規約
  - プライバシーポリシー

## 使用技術

| カテゴリー | 技術 |
:----|:----
| フロントエンド | Rails 7.0.8.4, JavaScript, TailwindCSS, daisyUI |
| バックエンド | Rails 7.0.8.4 (Ruby 3.2.3 )  |
| インフラ | Heroku, Google Cloud Storage |
| データベース | PostgreSQL |
| 開発環境 | Docker |
| 認証 | devise, Googleログイン |
| API | Google Maps API(JavaScript API, Places API) |
| CI/CD | GitHub Actions |


## 画面遷移図
https://www.figma.com/design/HmFLujwHeo0iRhkuUzUVph/entsumugi-%E7%94%BB%E9%9D%A2%E9%81%B7%E7%A7%BB%E5%9B%B3?node-id=0-1&node-type=canvas&t=PTIfvibK3PpdGZhg-0

## ER図
[![Image from Gyazo](https://i.gyazo.com/cf980ab406849ee7047bafc950f51598.png)](https://gyazo.com/cf980ab406849ee7047bafc950f51598)

## 今後の開発
<追加予定の機能>
  - 神社登録機能
  - 投稿時の神社名入力のオートコンプリート機能
  - 投稿ごとのxシェア機能
  - 投稿に対するいいね機能
  - 参拝マナーや神社・御朱印に関するコンテンツ