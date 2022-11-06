---
layout: "../../layouts/BlogPost.astro"
title: 次世代 Web カンファレンスの CSS のセッションで話した
pubDate: "2019-01-16"
description: "ブラウザが存在する限り、CSS がなくなることは考えられない。しかし人はこれからもずっと CSS を手で書き続けるのだろうか。"
---

今月の13日に開催された[次世代 Web カンファレンス](https://nextwebconf.connpass.com/event/103056/)の CSS のセッションで登壇させていただいた。事前打ち合わせなしで80分ディスカッションできるのかと不安に思っていたが、始まると意外と時間が早く過ぎ、もっと話せるなと感じた。

話したのはざっくりと以下の内容。YouTube に当日の動画が上がっています。

- 今後実装されていく仕様
- ユーザーとしての現場感
- CSS とそのユーザーの未来

[CSS - 次世代Webカンファレンス #nwc_css](https://www.youtube.com/watch?v=YxJ61YbbZmk)

---

僕は2015年の同カンファレンスでも CSS のセッションで参加しており、その当時から CSS とその周辺ツールは特に変化がないように思っている。
当日も話したが、Selector Level 4 や Houdini の API など、仕様の策定は進んでいるが IE をサポートし続ける限り使えないものがほとんどで、CSS のユーザーとしては4年前とほとんど状況が変わっていないのではないか。

ツール周りについては、4年前がちょうどいわゆる CSS-in-JS 系のツールが出始めた頃で、その頃と比べて多くの実装ができて、 styled-components というデファクトスタンダード的なライブラリが決定したが、特に革新的な斬新な道具が生まれたわけではない。Houdini から WICG に移動した Parser API の仕様がいつ決まるのかわからないが、Parser API と Typed OM と Properties and Values API が実装されれば、既存のものとは違う新しい CSS のメタ言語や周辺ツールが生まれる気がしている。

この4年間で使えるようになり、便利になった仕様といえば CSS Grid だと思う。既存の CSS と JavaScript のレイアウト手法で再現できず、CSS Grid で解決できるものはないのかもしれないが、これまでは複雑だった実装をシンプルにできるようになった。僕は、CSS Grid の1番のメリットは、グリッドを表現したいときに `display: grid` と記述すれば良くなったところだと思う。昔のテーブルレイアウトや `float` を使ってもグリッドを表現できたが、コードを読んで何をしているのか理解しやすくなった。CSS にはこのような実現したい視覚表現と記述内容にギャップがあることが多く（例えば gradient を使ってパターン背景を作るなど）、今後に期待したい。

他には、4年前と比べて実装可能な視覚表現が増えていないと思う。と言っても今の実装範囲で表現できないことはほとんどなく、CSS でのアニメーションの制御と、CSS Shapes、マルチカラムのレイアウトくらいしか思いつかない。

---

ブラウザが存在する限り、CSS がなくなることは考えられない。しかし人はこれからもずっと CSS を手で書き続けるのだろうか。僕は、何年後に実現できるかはわからないが、Sketch や Figma のような WYSIWYG ツールを使ってブラウザに表示される見た目部分を実装できるようになると思う。今でもコードを書かずに制作できるツールはあるが、バージョン管理とメンテナンス性の観点でまだ不十分だと思う。

観測範囲の CSS をメイン武器としていたユーザーの人たちは、例えば Nicolas Gallagher がバリバリの React ユーザーになったように、徐々に他の武器を見つけていってるように見える。僕もここ1年くらいは UI デザインがメインの仕事となってしまった。

当日、「50年後くらいに縁側に座って CSS を書いていたい」と発言したら思ったよりウケたのがウケた。僕がこの業界に興味を持った1番のきっかけは CSS だったりするので、愛着があるし、今後も動向を追って行きたいと思う。
