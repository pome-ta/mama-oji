# mama-oji


Twitter アカウント<br>
[ママレードおじさん 🍊ホームページ作るぞ大作戦日記](https://twitter.com/mikanojisan)


応援リポジトリ

## GitHub Pages

[preview page](https://pome-ta.github.io/mama-oji/index)


## LOG
> 2020/05/11

- リポジトリ作成
- CSS リセットを `bootstrap-reboot` に
- CSS デバック設置
- GitHub Pages 設置


## CSS リセット


絶対に必要という訳ではないです。私は、Reboot で慣れてしまったので、毎回入れてます。


### 参考記事

- [Reboot.css　Bootstrap製Reset.cssからCSSの新しいスタンダードを読み解く](https://goodpatch.com/blog/reboot-css/)
- [CSSリセット、2019年におすすめのカスタマイズ方法](https://coliss.com/articles/build-websites/operation/css/my-css-reset-by-ire.html)


## CSS デバック

スタンダードな手法ではないのです。私がなんとなく慣れてしまったので。


### 参考記事

- [CSSで実装したレイアウトの構造や階層を簡単に確認できる、私のお気に入りのCSSハック -My favorite CSS hack](https://coliss.com/articles/build-websites/operation/css/my-favorite-css-hack-by-gajus.html)


なお、記事掲載のコードは、

- `:` が全角になっている
- `,` が `、` となっている

typo があるので自分で書き換えをしてます

### 間違ったコード(サイトに掲示されているもの)

``` mistake.css
* {background-color: rgba(255,0,0,.2)}
* * {background-color：rgba(0,255,0、.2)}
* * * {background-color：rgba(0,0,255、.2)}
* * * * {background-color：rgba(255,0,255、.2)}
* * * * * {background-color：rgba(0,255,255、.2)}
* * * * * * {background-color：rgba(255,255,0、.2)}
* * * * * * * {background-color：rgba(255,0,0、.2)}
* * * * * * * * {background-color：rgba(0,255,0、.2)}
* * * * * * * * * {background-color：rgba(0,0,255、.2)}
```

### 修正版コード

``` fix.css
* {background-color: rgba(255,0,0,.2)}
* * {background-color: rgba(0,255,0,.2)}
* * * {background-color: rgba(0,0,255,.2)}
* * * * {background-color: rgba(255,0,255,.2)}
* * * * * {background-color: rgba(0,255,255,.2)}
* * * * * * {background-color: rgba(255,255,0,.2)}
* * * * * * * {background-color: rgba(255,0,0,.2)}
* * * * * * * * {background-color: rgba(0,255,0,.2)}
* * * * * * * * * {background-color: rgba(0,0,255,.2)}
```


## Grid Layout

サイトの外観調整は、GridLayout を使用(ブラウザ表示時)


### 参考サイト

- [これで分かった！10分でほとんど理解できる「CSSグリッド」の基礎](https://ferret-plus.com/8351)
- [CSS Grid Layout入門 対応ブラウザが出揃った新しいレイアウト仕様](https://ics.media/entry/15649/)

## Flex Layout

各コンテンツ内のレイアウト調整は、FlexBox を想定

### 参考サイト

- [日本語対応！CSS Flexboxのチートシートを作ったので配布します](https://www.webcreatorbox.com/tech/css-flexbox-cheat-sheet)
  - サイト内の設定でダークモードにすると、画像の説明がクッソ見辛いから注意
- [CSS Flexbox の基礎知識と使い方をやさしく解説](https://coliss.com/articles/build-websites/operation/css/css3-flexbox-properties-by-scotch.html)


## SP 表示

ディスプレイサイズを検知し、レスポンシブなレイアウトに調整






## 画像


[Pexels Cats](https://www.pexels.com/cats)


ぬこ


サンプル画像として使う予定
