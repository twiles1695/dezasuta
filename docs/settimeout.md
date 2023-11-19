# タイマー機能

ページを読み込んで〜秒後に処理を実行したいといった場合、JavaScriptの`setTimeout()`関数が使えます。

```html
<script>
  $(function(){

    // タイマー機能
    setTimeout(function(){
      // ページが読み込まれて3秒後にここに記述された処理が発動します。
      console.log("3秒経過");
    }, 3000);

  });
</script>
```

`3000`の箇所をお好みの時間に変更ください（3000ミリ秒 = 3秒）。

`console.log("3秒経過");`の箇所をお好みの処理に書き換えてください。

参考:<br>
[【JavaScript入門】setTimeoutの使い方とサンプル事例まとめ！](https://www.sejuku.net/blog/24540)