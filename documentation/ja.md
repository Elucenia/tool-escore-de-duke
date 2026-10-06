<!-- ELUCENIA technical documentation · escore-de-duke · ja · no clinical/professional/rights approval -->

# Dukeトレッドミルスコア

[条件・出典・許諾](https://elucenia.org/ja/tools/escore-de-duke)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 運動時間（Bruceプロトコル）

`tempo`

min · 範囲: 0–30

### 最大ST偏位（aVR以外の任意の誘導）

`st`

mm · 範囲: 0–10

### 検査中の狭心症

`angina`

- `0` — いいえ
- `1` — 運動を制限しない
- `2` — 運動を制限（中止の理由）

## 方法の版

Duke Treadmill/Mark 1987：時間−5ST−4狭心痛、1991検証ノモグラム

## 記載された計算式

点数 = 運動時間（min）− 5 × ST偏位（mm）− 4 × 狭心痛指数（0 = なし、1 = 制限なし、2 = 制限あり）。

## 限界・対象集団

1987年のDuke Treadmill Scoreは、トレッドミル検査と心臓カテーテル検査を受けた胸痛のある人の予後評価のために開発されました。式は、プロトコルにおける時間、ST偏位、狭心症指数の規約に依存します。スコアによる予後は、冠動脈疾患の診断や、その人が運動を行う安全性を確定するものではありません。

## 参考文献

- [Mark DB et al. Exercise treadmill score for predicting prognosis in coronary artery disease. Ann Intern Med, 1987.](https://doi.org/10.7326/0003-4819-106-6-793)

- [Mark DB et al. Prognostic value of a treadmill exercise score in outpatients with suspected coronary artery disease. N Engl J Med, 1991.](https://doi.org/10.1056/NEJM199109193251204)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 記録された結果

以下の情報は、合成例に対する手法の出力を保持したものです。独立した臨床的検証を示すものではありません。

### 1

中等度リスク

| 結果の詳細 | |
| --- | --- |
| 推定年間死亡率 | 1.25% |


### 2

低リスク

| 結果の詳細 | |
| --- | --- |
| 推定年間死亡率 | 0.25% |


### 3

高リスク

| 結果の詳細 | |
| --- | --- |
| 推定年間死亡率 | 5.25% |

