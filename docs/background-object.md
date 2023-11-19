
# 背景にオブジェクトを入れる実装

<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="oNJMBOW" data-user="tkm1695" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/tkm1695/pen/oNJMBOW">
  背景にオブジェクトを入れる実装</a> by tkm1695 (<a href="https://codepen.io/tkm1695">@tkm1695</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

下記のURLにアクセスして大きい画面でご確認ください。<br>
[https://codepen.io/tkm1695/pen/oNJMBOW](https://codepen.io/tkm1695/pen/oNJMBOW)

## CSSのポイント

- 親要素に`position: relative`を指定
- 子要素（配置したい要素）に`position: absolute`を指定 + 親要素を基準とした時の座標（`top: 20px` `right: -100px`など）を指定