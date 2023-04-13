## ディレクトリ構造

ドキュメントルートは以下の通り、`html`ディレクトリにします。

```
./src
├── README.md          // この資料(非公開)
├── html               // ドキュメントルート(公開)
│   ├── answer.php
│   ├── index.php
│   ├── question.php
│   ├── questions.js
│   └── style.css
├── lib               // ライブラリ用ディレクトリ(非公開)
│   ├── data.csv
│   └── functions.php
└── template          // HTMLの中にPHPを含んだテンプレート用ディレクトリ(非公開)
    ├── 404.tpl.php
    ├── index.tpl.php
    └── question.tpl.php
```

`answer.php` の中から`functions.php`を参照する場合は、 `../lib/functions.php`を指定します。

## 実行方法

### 1. カレントディレクトリを html ディレクトリまで移動する

```
cd src/html
```

※ `src/html` 実際のファイル配置場所を指定してください。

### 2. PHP のビルトインウェブサーバーを起動する

```
php -S localhost:8080
```

### 3. ブラウザで確認

以下にアクセスします。

http://localhost:8080
