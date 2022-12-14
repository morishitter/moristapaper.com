---
layout: "../../layouts/BlogPost.astro"
title: ブログを移転した
pubDate: "2018-02-16"
description: "これまではてなブログを自分のブログとしていたが、自作で自分のドメインのブログに移転することにした。技術的な Tips は引き続き Qiita に投稿しつつ、その他のことをここに集約していきたいと思っている。"
---

これまではてなブログを自分のブログとしていたが、自作で自分のドメインのブログに移転することにした。技術的な Tips は引き続き Qiita に投稿しつつ、その他のことをここに集約していきたいと思っている。

[Medium](https://medium.com) か [note](https://note.mu/) を利用することも考えたが、PV を稼ぎたいわけではないし、両方ともエディタが絶妙に使いづらく Markdown で書きたかったので使わなかった。サイトのデザインを100%自分でコントロールしたかったのと、フロントエンド技術を検証する場にもなると思い、自作することにした。

今のデザインのコンセプトとしては「シンプルでクリーン」にしている。有彩色を使わず、コントラストも抑えめで全体的に白っぽい雰囲気にした。

リンクには下線を付けているだけで、 `:visited` のスタイルは付けなかった。リンクに色を付けるなど目立つ装飾を施すと、興味のないリンクは文章を読んでいるときの邪魔になる。「これは何だろう」と思ったときに「リンクになっている」と気付ける程度の装飾で十分ではないかと思う。

`<hr>` の区切り線やコードブロックの背景色も薄すぎるくらい薄いが、これも読むことの妨げにならず **認識しようとしたときに認識できる程度の装飾** を試している。本文の[スタイル確認用の記事](/styleguide)があるので、それを見ると雰囲気がわかる。

今のデザインでは、「読者のモニターの色設定の多様さも考慮せずに何がデザインだ」というアクセシビリティ云々についてのマサカリはある程度無視することにした。

また、技術面ではこのブログは React 製の静的サイトジェネレーターの [Gatsby](https://www.gatsbyjs.org/) を使っており、GitHub にソースコードを push して [Netlify](https://www.netlify.com/) でビルドしてホスティングしている。Netlify、設定が簡単で独自ドメインの SSL 対応もできるので便利だった。

せっかく重い腰を上げてブログをこしらえたので、これを機に文章のアウトプット量を増やしていきたい。
