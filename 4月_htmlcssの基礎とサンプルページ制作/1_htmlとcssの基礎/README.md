# html/cssの基礎

## html/cssとは

 言語 | 役割  | 機能 
--|---|--
 html  |  webサイトの構造を表す言語 |  webサイトに何を表示するかを記述する
 css  | webサイトにスタイルを当てる言語  |  文字の色や画像のサイズ、レイアウトなどを記述する

## HTMLタグの使用方法と基本的な用語  
HTMLは、①開始タグと終了タグで一つの要素、②一つのタグのみで成り立つ要素の2つがある。  
①の場合、開始タグと終了タグの間に表示したいものを記述する。終了タグには "/" をつける。
 ```html
 <!-- この枠で囲んだものはコメントアウトと言って書いたコードを無効化できる -->
 <!-- ①の例 -->
 構文： <開始タグ 属性="属性値">コンテンツ</終了タグ>
 <h1 class="html_basic">多くの要素は開始タグと終了タグが必要</h1>
 <!-- ②の例 -->
 構文： <タグ 属性="属性値">
 <img src="hoge.jpg" class="my_image">
 ```
## HTMLの基本構成  
<p>HTMLの構造を大きく分けると次のようになります。</p>
<p><img src = "assets/img/htmlSample.png" width="400px"></p>  

## 実際にHTMLを書いてみよう！  
```html
<!DOCTYPE html>
<html>
  <head>
    <!-- この中はウェブブラウザに現れない -->
    <meta charset="utf-8">
    <title>HTMLの基本</title>
  </head>
  <body>
    <!-- ここに書かれたことは実際に表示される -->
    <h1>Hello, world!</h1>
  </body>
</html>
```
## ウェブブラウザで書いたコードを確認しよう
### 書いたコードのファイルをダブルクリック
このアプリケーションで開くを押して、Chrome または Safari(ウェブブラウザ)を選択
<p><img src = "assets/img/folder_sample.png" width="300p"></p>
問題がなければブラウザで自分の書いたコードが見れるはず
<p><img src = "assets/img/hello_world.png" width="300p"></p>

## タグの一つ一つを知っていこう！
### h1 ~ h6(見出しを作るためのタグ)
```html
<h1> h1 について知ろう！</h1>
<h2> h2 について知ろう！</h2>
<h3> h3 について知ろう！</h3>
<h4> h4 について知ろう！</h4>
<h5> h5 について知ろう！</h5>
<h6> h6 について知ろう！</h6>
```

1. p(段落区切りを示すタグ)  

```html
<p>段落を示すのはpタグ！</p>
```

2. ul, li (リストを作るタグ)  

```html
<ul>
  <li>1個目</li>
  <li>2個目</li>
  <li>3個目</li>
  <li>4個目</li>
  <li>5個目</li>
</ul>
```

3. div (大きなかたまりを作るタグ)  

```html
<div>
  <h1>かたまりの見出し</h1>
  <p>かたまりの文章</p>
</div>
```

4. img (画像を貼るためのタグ)  
```html

<div>
  <!-- フォルダの階層を辿って画像ファイルまで正確に記述する！ -->
  <img src="assets/img/hello_world.png">
</div>

```

5. table, tr, th, td (表を作るために必要なタグ)  
```html

<div>
  <h1>テーブルについて</h1>
  <table border="1">
    <caption>表題</caption><!-- 表題に使う -->
    <thead>
      <tr>
        <th>ヘッダ１</th>
        <th>ヘッダ２</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>１ー１</td>
        <td>２ー１</td>
      </tr>
      <tr>
        <td>１ー２</td>
        <td>２ー２</td>
      </tr>
    </tbody>
  </table>
</div>

```

5. header,main,footer(Webページの上、真ん中、下を表す)
```html

<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="utf-8">
  <title>ヘッダー、メイン、フッターの勉強</title>
</head>
<body>
<!-- ここからヘッダー -->
  <header style="background-color: #111">
    <div style="color: #fff">
      <h1>ヘッダー</h1>
      <p>ヘッダーだよ</p>
    </div>
  </header>
<!-- ここからメイン -->
  <main style="background-color: #aaa">
    <div>
      <h1>メイン</h1>
      <p>メインだよ</p>
    </div>
  </main>
<!-- ここからフッター -->
  <footer style="background-color: #fff">
    <div>
      <h1>フッター</h1>
      <p>フッターだよ</p>
    </div>
  </footer>
</body>
</html>

```
















