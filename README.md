# survey-of-price-elasticity
価格弾力性に関する調査一般

## 言葉の定義
 - [価格弾力性とは](http://careergarden.jp/column/kakakudanryokusei/)

## 野球でのユースケース
 - [京大教授が“切る”現代経済 vol.6　ダイナミック・プライシングは消費者の味方か](http://www.business-plus.net/business/columnist/Idatakanori/series/170802_tp0018.html)  
 
価格を決めるのにこれらの特徴量を利用しているらしい
```
1. 過去にその席が「福岡ヤフオク！ドーム」5万席の中で何番目に購入されたのか
2. 現在の対象のチケットの売れ行き
3. 天候やホークスの順位、相手チーム、開始時刻や曜日
```

 - [楽天のチケット価格変動制の賛否。MLBでは定着も空席増える課題も](https://thepage.jp/detail/20170128-00000001-wordleafs?page=1)  
> チケット価格変動制は、先発投手やその日の天候などの影響で、需要の変化に応じて値段がリアルタイムで変動するものと、リアルタイムでは変動しないが、あらかじめシーズン前に分かっている対戦相手や試合開始時間、曜日などによって異なる価格設定をしているものがある。現在、メジャーリーグの大半の球団がこのどちらかのケースや、2つを組み合わせた形でチケットを販売している。

## エンターテイメント施設でのユースケース
 - [「一物一価の法則」はもう古い？刻一刻と価格が動く世界の到来](https://diamond.jp/articles/-/87829)
> インディアナポリス動物園では、入園料が繁閑に合わせて8～30ドルで変化する。ミシガン州のスキー場の入場料も10ドル程度から30ドル超まで変動する（米紙「ウォールストリート・ジャーナル」） 

## コードスニペットと例
 - [Developing a Pricing Strategy to Maximize Revenue](https://www.datascience.com/resources/notebooks/python-dynamic-pricing)

## アドテク的な側面でのプライス調整
 - [How Dynamic Pricing Uses Machine Learning to Increase Revenue](https://sweetpricing.com/blog/2017/02/machine-learning/)
 
## 考えていること
 - 席やサービスのユーザ接触数Sと、券売確率pと独立だと仮定する。  
 - pは価格によって変化する変数だと捉えることができる => p(m):mはmoney 
 - Income = S * p(m) 
 
 - Sはサービスの特定の粒度で機械学習modelAで学習する
 - p(m)もSと同じサービスの粒度で機械学習modelBを学習する
 
 特定の月, 曜日, 休日とうのパラメータを特徴量として、予想するIncome量は、このようになる  
 
  `Income = S * p(m)`
