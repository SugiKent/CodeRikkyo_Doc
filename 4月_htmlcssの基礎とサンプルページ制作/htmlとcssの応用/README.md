# htmlとcssの応用

実際に自分の思い描くデザインをhtmlとcssで表現できるようになりましょう。
ここでは、いくつかの課題を通して様々な手法を学びます。

## 第一問

### 問題
以下の様に、要素を横並びにしてみましょう。

![横並びの画像](http://www)

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

