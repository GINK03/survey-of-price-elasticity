# 2018年にメルカリの価格推定コンペティションがKaggleで行われた。

その時目的関数が価格であったが、trainデータに含まれている価格と製品のカテゴリと売れたかどうかを扱い、
カテゴリごとの平均のカテゴリ価格を1としてみていって0.05刻みでその時の勾配確率が算出できる。 　

すべてのカテゴリの平均をさらにとって、一般的に、どの程度売れるかわかる。

<div align="center">
  <img width="400px" src="https://user-images.githubusercontent.com/4949982/46245191-ce12b780-c424-11e8-8549-07a623a16c15.png">
</div>

このように平均の半額ぐらいから購買確率が上がるようです。
（shippingが相手が配送負担の可能性あり）
