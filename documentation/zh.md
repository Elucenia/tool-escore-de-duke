<!-- ELUCENIA technical documentation · escore-de-duke · zh · no clinical/professional/rights approval -->

# Duke 平板运动评分

[条件、来源与许可](https://elucenia.org/zh/tools/escore-de-duke)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 运动时间（Bruce 方案）

`tempo`

min · 范围: 0–30

### 最大 ST 段偏移（除 aVR 外任何导联）

`st`

mm · 范围: 0–10

### 试验期间心绞痛

`angina`

- `0` — 否
- `1` — 不限制运动
- `2` — 限制运动（停止试验的原因）

## 方法版本

Duke Treadmill/Mark 1987：时间−5ST−4心绞痛；1991验证列线图

## 已记录的公式

评分 = 运动时间（min）− 5 × ST偏移（mm）− 4 × 心绞痛指数（0 = 无，1 = 不限制运动，2 = 限制运动）。

## 限制与适用人群

1987年的Duke Treadmill Score为接受运动平板试验和心导管检查的胸痛患者的预后评估而开发。公式依赖方案中运动时间、ST偏移和心绞痛指数的约定。评分所提供的预后不能确诊冠状动脉疾病，也不能确定某人进行运动的安全性。

## 参考文献

- [Mark DB et al. Exercise treadmill score for predicting prognosis in coronary artery disease. Ann Intern Med, 1987.](https://doi.org/10.7326/0003-4819-106-6-793)

- [Mark DB et al. Prognostic value of a treadmill exercise score in outpatients with suspected coronary artery disease. N Engl J Med, 1991.](https://doi.org/10.1056/NEJM199109193251204)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 已记录的结果

以下信息保留该方法对合成示例的输出，不构成独立的临床验证。

### 1

中等风险

| 结果详情 | |
| --- | --- |
| 估计年死亡率 | 1.25% |


### 2

低风险

| 结果详情 | |
| --- | --- |
| 估计年死亡率 | 0.25% |


### 3

高风险

| 结果详情 | |
| --- | --- |
| 估计年死亡率 | 5.25% |

