# htmlとcssの応用

実際に自分の思い描くデザインをhtmlとcssで表現できるようになりましょう。
ここでは、いくつかの課題を通して様々な手法を学びます。

## 第一問

### 問題
以下の様に、要素を横並びにしてみましょう。

![横並びの画像](https://raw.githubusercontent.com/SugiKent/CodeRikkyo_Doc/master/4%E6%9C%88_htmlcss%E3%81%AE%E5%9F%BA%E7%A4%8E%E3%81%A8%E3%82%B5%E3%83%B3%E3%83%97%E3%83%AB%E3%83%9A%E3%83%BC%E3%82%B8%E5%88%B6%E4%BD%9C/2_html%E3%81%A8css%E3%81%AE%E5%BF%9C%E7%94%A8/images/inline-block%E3%81%AE%E3%82%B5%E3%83%B3%E3%83%97%E3%83%AB.png)

### 答え

``` index.html

<body>
  <div class="Wrapper">
    <div class="Block">

    </div>
    <div class="Block">
    </div>
  </div>
<body>

```

``` master.css
* {
  margin: 0px;
  padding: 0px;
}
.Wrapper {
  width: 100%;
  height: 500px;
}
.Block {
  width: 50%;
  hieght: 500px;
  display: inline-block;
}
```
### ポイント

htmlにはblock要素とinline要素と呼ばれるものがあります。  
block要素は通常縦並びで、inline要素は横並びになります。  
`display: inline-block;`により、本来block要素であるdiv要素を **横並びのblock要素** にすることができます。  
この手法を用いれば、簡単に要素を横並びにすることが可能です。  

横並びにする手法として、 `float` というパラメータを使う方法がありますが、floatは他のスタイルを崩してしまう要因になりやすいため、昨今のwebではあまり使用しません。

