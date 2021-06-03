## section 7 （レイアウトパーツ後半）

## 修正内容

1. q8 の画像に対してのhoverに`transition: 0.5s all;`は不要。
   -  `transition: 0.5s all;`を消しました。（コメントアウト）

2. q8 のアニメーションの `@keyframes`での内容に、`0%`から始まる値がない
   - `@keyframes`の中に、
   ```css
   0% {
    transition: rotate(0deg);
   }
   ```
   を書きました。
3. q9 の divタグ（`q9__content`）内のテキストタグにフォントサイズを当てていたが、divタグに要素を当てると子要素に影響が出るから不要。
   - divタグ(`q9__content`)にテキストのフォントサイズを当てました。
   ```css
   q9__content {
   、、、、
   、、、、
   font-size: 16px;
   line-height: 16px;
   }
   ```