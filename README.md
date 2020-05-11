# mama-oji


Twitter アカウント<br>
[ママレードおじさん 🍊ホームページ作るぞ大作戦日記](https://twitter.com/mikanojisan)


応援リポジトリ


> 2020/05/11

- リポジトリ作成
- CSS リセットを `bootstrap-reboot` に
- CSS デバック設置


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

### 修正版コード(`:` の半角修正)

``` fix.css
* {background-color: rgba(255,0,0, .2)}
* * {background-color: rgba(0,255,0、.2)}
* * * {background-color: rgba(0,0,255、.2)}
* * * * {background-color: rgba(255,0,255、.2)}
* * * * * {background-color: rgba(0,255,255、.2)}
* * * * * * {background-color: rgba(255,255,0、.2)}
* * * * * * * {background-color: rgba(255,0,0、.2)}
* * * * * * * * {background-color: rgba(0,255,0、.2)}
* * * * * * * * * {background-color: rgba(0,0,255、.2)}
```
