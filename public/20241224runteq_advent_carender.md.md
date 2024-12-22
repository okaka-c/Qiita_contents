---
title: 'ステップ入力'
tags:
  - 'Ruby on Rails'
private: false
updated_at: ''
id: null
organization_url_name: null
slide: false
ignorePublish: false
---
### はじめに
プログラミングスクールRUNTEQ卒業生のおかかチーズと申します。([@Yoo_pr](https://x.com/Yoo_pr))
RUNTEQアドベントカレンダー2024🎄 24日目を担当致します。

https://qiita.com/advent-calendar/2024/runteq

ポートフォリオで、私が5年ほど続けている競技「パワーリフティング」の試技結果が記録・管理ができるサービスを制作しました。
サービス名: [PowerLifter's Log](https://www.powerlifterslog.com/)
GitHub: https://github.com/okaka-c/goodlifterlog

サービスでの工夫ポイントは、試技結果の入力フォームをステップ入力フォームにしたことです。




本記事ではRuby on RailsのAction Viewテンプレート `ERBビューテンプレート`を用いた
ステップ入力フォームの実装方法と
画面設計をする際にUI/UX設計面で考えた事をまとめました。


:::note warn
**記事を読むうえでの注意点**

Ruby on Rails、画面のデザインやUI/UX設計については経験が浅く、一部おかしな記述があるかもしれません。
そのためもし間違いなどがありましたらご指摘いただけると幸いです。よろしくお願いします。
:::

### 環境
| カテゴリ | 技術 |
| --- | --- |
| PC | MacBook Air M2 |
| 開発環境 | Docker |
| フロントエンド |TailwindCSS, daisyUI|
| バックエンド | Ruby 3.2.2 / Ruby on Rails 7.0.8.1 |
| データベース | PostgreSQL |

### この記事のゴール
- Ruby on Railsの以下の機能を使ったステップ入力フォームの実装方法がわかる
  -  sessionメソッド
  - `ActiveModel::Modelモジュール`
  - `ActiveModel::Validationsモジュール`
- ステップ入力フォームの `UI/UX設計`のポイントがわかる

### ステップ入力フォームとは
入力フォームを1ページにすべて表示するのではなく、いくつかのステップに分割して順番に表示する形式です。
複数の入力項目を1ページにまとめるとフォームが長くなり、ユーザーにとって見にくく、入力の心理的ハードルが上がることがあります。

例えば、以下のイメージ画像の左側には、氏名、メールアドレス、パスワード、住所情報、クレジットカード情報を1ページにまとめた会員登録フォームがあります。
これを画像のように「ユーザー情報」「住所情報」「クレジットカード情報」の3つに分け、それぞれをステップごとに順番に入力する形式にしたものがステップ入力フォームです。
<img width="auto" src="https://i.gyazo.com/5e2f8b94b7135fa0c8287f2e7e2ffca5.jpg">

詳しい内容やメリットについては、以下の参考サイトで詳しく解説されていますので、ぜひご覧ください。本記事では詳細な説明を割愛します。

https://ds-b.jp/dsmagazine/what-is-stepform/

### 本サービスへ導入した経緯
※【before】MVPリリース時点の入力フォーム。
<img width="auto" src="https://i.gyazo.com/78b1852ad847831b0057cd0e380a141b.png">

使いづらい・見づらいという問題点がありました。
そこで、ステップ入力フォームを採用し、1ページに収めていた入力フォームを5ページに分割し問題点を改善しました。

※【after】ステップ入力フォーム採用後
<img width="auto" src="https://i.gyazo.com/588d5b635d6d500027f11a71d3c12a80.gif">

### 作ったものややったことの説明

### 実装の流れ（アジェンダ)

### 実装の流れ詳細

### おわりに

### 参考文献
https://ds-b.jp/dsmagazine/what-is-stepform/
https://edito.jp/corporate/231220/