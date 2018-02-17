# アンサンブル学習でスパムメールを分類
<br>3種類の分類器、ロジスティック回帰分類器、決定木分類器、k近傍分類器を1つのアンサンブル分類器にまとめてスパムメールを分類した。</br>
## 説明
<br>数値化されたスパムメールのデータを弱い学習器のロジスティック回帰分類器、決定木分類器、k近傍分類器を多数決型のアンサンブル学習を使って予測した。<br>
<br>まず、データを標準化と主成分分析を使って学習しやすいデータに加工した。その後、トレーニングデータを10分割交差検証して性能を確認。思うような結果が出なかったのでグリットサーチを使ってパラメータをチューニングをして性能をあげた。最終的に学習曲線を使ってバリアスとバイアスを確認して問題がなそうであったの最終的なモデルを作った。<br>
<br>最後に決定領域をプロットしてモデルがどのように分類しているのかを確認をした。<br>

### draw_function.pyについて
<br>draw_function.pyは決定領域と簡単な散布図を描画してくれる関数のプログラムである。</br>
### 実行した環境
<br>mac os</br>
<br>python 3.6.2</br>
<br>numpy 1.13.1</br>
<br>pandas 0.20.3</br>
<br>matplotlib 2.0.2</br>
<br>scikit-laern 0.19.0</br>
## 今後の方針
<br>今回は数値化されたスパムデータを分類したが、次回はテキストデータから数値化に挑戦しようと思う。</br>
### 参考文献
Pyhon機械学習プログラミング　達人データサイエンティストによる理論と実践
<br>著者:Sebastian Raschka  監訳者：福島慎太郎</br>


