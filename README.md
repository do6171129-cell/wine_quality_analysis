# Wine Quality Analysis（EDA）

## 概要
赤ワインの化学的特性と品質スコア（quality）の関係を、探索的データ分析（EDA）の作法に沿って確認した事例です。  
可視化 → 仮説 → 数値による裏取り、の順序を重視しています。

## 目的
- ワインの化学特性と品質スコアの関係性を探索する
- 相関を見る前に、分布・構造を把握するEDAの進め方を示す

## データ
- Wine Quality Dataset（Red Wine）
- 各ワインの化学特性（例：total sulfur dioxide, residual sugar など）と品質スコア（quality）

※ CSV は `data/` ディレクトリに配置しています。

## 分析内容
- データ概要の確認
- 基本統計量・分布の確認
- quality 別の分布比較（箱ひげ図）
- 散布図による関係性の確認
- 相関係数（Pearson）による仮説の裏取り

## 分かったこと
- total sulfur dioxide と quality の間には **弱い負の関係**が示唆された
- residual sugar と quality の間には **明確な関係は見られなかった**

## 限界
- 相関はいずれも弱く、因果関係は判断できない
- quality は離散値であり、外れ値や分布の歪みの影響が残る可能性がある

## 次の一手
- 他の化学特性を含めた多変量での検証
- 条件分けやモデル化による関係性の再確認

## 実行方法
Jupyter Notebook を上から順に実行してください。

## 構成
```
.
├─ analysis.ipynb
├─ README.md
├─ .gitignore
└─ data/
   └─ winequality-red.csv
```
## データについて

本分析では、Kaggleで公開されているワイン品質データを使用しています。

Data source:
Wine Quality - Red Wine  
https://www.kaggle.com/datasets/anairamcosta/winequality-red-csv  
Provided via Kaggle (originally from UCI Machine Learning Repository)  
Used for educational and analytical purposes.

