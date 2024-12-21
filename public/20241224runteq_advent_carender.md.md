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
試技結果の入力フォームは、入力項目数が最大20項目になってしまいます。
最初は画像のように1ページに20項目を収めていました。

※【before】MVPリリース時点の入力フォーム。
<img width=30% src="https://i.gyazo.com/78b1852ad847831b0057cd0e380a141b.png">

使いづらい・見づらいという問題点がありました。
そこで、ステップ入力フォームを採用し、1ページに収めていた入力フォームを5ページに分割し問題点を改善しました。

※【after】ステップ入力フォーム採用後
<img width=40% src="https://i.gyazo.com/588d5b635d6d500027f11a71d3c12a80.gif">

本記事ではRuby on RailsのAction Viewテンプレート `ERBビューテンプレート`を用いた
ステップ入力フォームの実装方法と
画面設計をする際にUI/UX設計面で考えた事をまとめました。


:::note warn
**記事を読むうえでの注意点**

Ruby on Rails、画面のデザインやUI/UX設計については経験が浅く、一部おかしな記述があるかもしれません。
そのためもし間違いなどがありましたらご指摘いただけると幸いです。よろしくお願いします。
:::

### 環境

- 開発環境


### ステップ入力とは

- ステップ入力のサラッとした説明



### 記事の目標・記事で達成できるゴール

### 作ったものややったことの説明

### 実装の流れ（アジェンダ)

### 実装の流れ詳細

### おわりに

### 参考文献