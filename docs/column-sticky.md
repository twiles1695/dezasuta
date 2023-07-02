# 横並びsticky

横並びレイアウトで、スクロールした時に片方だけ固定して表示させたい場合の実装方法です。

ポイントは2点です。

- 3レイヤー（親要素・子要素・孫要素）を作成

- 孫要素に`position: sticky` `top: 0`を指定

<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="xxQdeRx" data-user="tkm1695" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/tkm1695/pen/xxQdeRx">
  横並びsticky</a> by tkm1695 (<a href="https://codepen.io/tkm1695">@tkm1695</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>