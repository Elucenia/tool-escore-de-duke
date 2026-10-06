<!-- ELUCENIA technical documentation · escore-de-duke · en · no clinical/professional/rights approval -->

# Duke Treadmill Score

[conditions, sources and permissions](https://elucenia.org/en/tools/escore-de-duke)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Exercise duration (Bruce protocol)

`tempo`

min · range: 0–30

### Greatest ST deviation (in any lead except aVR)

`st`

mm · range: 0–10

### Angina during the test

`angina`

- `0` — No
- `1` — Non-limiting
- `2` — Limiting (reason for stopping)

## Method edition

Duke Treadmill/Mark 1987: time−5ST−4angina; nomogram validated 1991

## Documented formula

Score = exercise time (min) − 5 × ST deviation (mm) − 4 × angina index (0 = none, 1 = non-limiting, 2 = limiting).

## Limits and population

The 1987 Duke Treadmill Score was developed for prognosis in people with chest pain undergoing treadmill testing and catheterization. The formula depends on the protocol’s conventions for time, ST deviation and angina index. Score prognosis does not confirm coronary disease or the safety of exercise testing in an individual.

## References

- [Mark DB et al. Exercise treadmill score for predicting prognosis in coronary artery disease. Ann Intern Med, 1987.](https://doi.org/10.7326/0003-4819-106-6-793)

- [Mark DB et al. Prognostic value of a treadmill exercise score in outpatients with suspected coronary artery disease. N Engl J Med, 1991.](https://doi.org/10.1056/NEJM199109193251204)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Documented results

The information below preserves the method outputs for synthetic examples. It does not constitute independent clinical validation.

### 1

Intermediate risk

| Result details | |
| --- | --- |
| Estimated annual mortality | 1.25% |


### 2

Low risk

| Result details | |
| --- | --- |
| Estimated annual mortality | 0.25% |


### 3

High risk

| Result details | |
| --- | --- |
| Estimated annual mortality | 5.25% |

