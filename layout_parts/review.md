# section 7

## 修正内容

1. q1 の（`q1__content__text`）子要素の`box-sizeing`と`width`の値は、親要素（`q1__content__box`）が値を指定しているので要らない。

   - （修正内容）css ファイルの`box-sizing`と`width`を消しました。（コメントアウト）

2. q2 div タグの子要素に`float`を使用しているので div タグに`clearfix`を使用しないと、付け足していくときに要素があふれてしまう。

   - （修正内容）div タグに`clearfix`クラスを書き`clearfix`を指定して、float が重ならないようにした。

3. span タグは文章の継ぎ足しになるのでそれ以外は、block 要素になるので`tr`,`th`,`td`は改行する必要がある。

   - （修正内容）HTML ファイルの`tr`,`th`,`td`を改行して見やすくした。

4. q4 の css ファイル で `q4__content__boxes div` の div と `box__content__box` は入らない。`margin-top:20px`も boxes だとクラスが増えた時に変動するから first-child は`margin:0;`にする。

   - css ファイルの`q4__content__boxes div` と `box__content__box`を消して、見やすくした。

5. css の `q5__content` クラスは要らない。`q5__content.box-skin`の`postion:absolute`を 消す。`q5__contetns div` も変更。html ファイルに`q5__content`で指定してあるから`q5`は不要。

   - html ファイルの`q5`と css の `q5__content`,`position:absolute`を省略。`q5__contents div`も `q5__content `へ変更。

6. クラス名が分かりづらいので、css を読む際にも場所のイメージが伝わるクラス名を書く。
   - クラス名を簡潔にして、html,css のクラス名を修正しました。
