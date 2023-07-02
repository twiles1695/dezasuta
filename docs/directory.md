# ディレクトリ構成

サイトを制作する上で、まずはディレクトリを作成する必要があります。
このページではどのように構成したらよいかを解説します。

## ディレクトリとフォルダの違い

Webでは「ディレクトリ」と「フォルダ」と似た言葉が出てきますが、どちらも同じ意味です。

ただ、「フォルダ」はPC内でファイルを扱う時に使われることが多く、「ディレクトリ」はWebサーバーなどアップロードする時に使われることが多いです。このページでは「ディレクトリ」と呼んでいきます。

一般的には以下のようなディレクトリ構成になることが多いです。

## 全体的な構成
```
portfolio
├── css
│   ├── common.css … リセットCSSやヘッダー・フッターなどサイト全体に共通するCSS
│   └── style.css … トップページのCSS
├── images … サイト全体で流用するする画像
├── js
│   └── script.js … サイト全体に適用するJS
├── index.html … トップページ
├── about … 自己紹介ページ
├── works … 制作実績一覧ページ
└── thanks.html … お問い合わせのサンクスページ
```

## 下層ページの構成

下層ページは、その名の通りトップページより深い階層にあり、サブページにあたります。
自己紹介ページを例にすると、以下のような構成になります。

```
portfolio
└── about
    ├── css
    │   └── style.css … 自己紹介ページのみに適用するCSS
    ├── images … 自己紹介ページのみで使用する画像を格納
    └── index.html … 自己紹介ページ
```

さらに制作実績一覧のようにページ数が多い場合は以下のようにすると管理しやすいです。

```
portfolio
└── works
    ├── css
    │   └── style.css … 制作実績ページのみに適用するCSS
    ├── images … 制作実績ページのみで使用する画像を格納
    ├── index.html … 制作実績一覧ページ
    ├── work1.html … 制作実績1のページ
    ├── work2.html … 制作実績2のページ
    └── work3.html … 制作実績3のページ
```

## index.htmlのURL省略

`index.html`ファイルは、ディレクトリの中で`索引`を意味します。

なので一つのディレクトリにつき一ファイルのみ置くことができ、かつ、URLでは`index.html`を省略することができます。

例）`https://dezasuta.com/portfolio/index.html` → `https://dezasuta.com/portfolio/`

こちらの方がスッキリしているので覚えやすい・入力しやすいというメリットがあります。

詳細はこちらを参照ください。
[ファイル名省略時の動作について](https://www.tohoho-web.com/wwwxx076.htm)

上記を踏まえると、各ページのURLはこのようになります。

---

トップページ：`https://dezasuta.com/portfolio/`

自己紹介ページ：`https://dezasuta.com/portfolio/about/`

制作実績一覧ページ：`https://dezasuta.com/portfolio/works/`

制作実績詳細ページ：`https://dezasuta.com/portfolio/works/work1.html`

---