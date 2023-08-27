# 左右中央配置の使い分け

要素を左右中央に配置したい時、どのプロパティを使えばいいのか？がわかるようになるための違い解説です。

## `display: flex;`  と  `justify-content: center;`
- 中央寄せしたい要素の **親要素** に指定します（最重要）
- 複数の要素を真ん中に寄せる時に使えます

<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="YzdwqRm" data-user="tkm1695" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/tkm1695/pen/YzdwqRm">
  【サンプル】flex-center</a> by tkm1695 (<a href="https://codepen.io/tkm1695">@tkm1695</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

```html
<div class="flex">
  <div class="flex-item">子要素</div>
  <div class="flex-item">子要素</div>
</div>
```

```css
.flex {
  display: flex;
  justify-content: center;
}
.flex-item {
  width: 30%;
}
```



##  `margin: 0 auto;`

- 中央寄せしたい要素 **そのもの** に指定します。
- 横幅が固定値(px)の時に使えます。逆に言えば、横幅指定しないと効かないので注意。
- ひとつの要素を真ん中に寄せたい時に使います

<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="YzdwqRm" data-user="tkm1695" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/tkm1695/pen/YzdwqRm">
  【サンプル】flex-center</a> by tkm1695 (<a href="https://codepen.io/tkm1695">@tkm1695</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

```html
<div class="container">
  （コンテンツ内容）
</div>
```

```css
.container {
  max-width: 1200px;
  margin: 0 auto;
}
```


## `text-align: center;`
基本的に**テキスト**を中央寄せする時に使います。

<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="RwEraYb" data-user="tkm1695" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/tkm1695/pen/RwEraYb">
  【サンプル】text-center</a> by tkm1695 (<a href="https://codepen.io/tkm1695">@tkm1695</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

```html
<p class="text-center">テキストテキストテキストテキスト<br>テキストテキストテキストテキスト</p>
```

```css
.text-center {
  text-align: center;
}
```

!!! さらなる解説
    テキスト以外であっても、インライン要素であれば中央寄せにすることができます。
    
---

!!! Point
    左右中央配置させる方法は様々あり、唯一の答えがあるわけではありません。<br>
    状況によって最適解はあるかもしれませんが、はじめから最適解にたどり着くのは至難の業なので<br>
    まずは試行錯誤してプロパティの違いを手を動かしながら確かめてみましょう。