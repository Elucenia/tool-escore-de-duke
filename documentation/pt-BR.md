<!-- ELUCENIA technical documentation · escore-de-duke · pt-BR · no clinical/professional/rights approval -->

# Escore de Duke (esteira)

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/escore-de-duke)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Tempo de exercício (protocolo de Bruce)

`tempo`

min · intervalo: 0–30

### Maior desnível do ST (em qualquer derivação, exceto aVR)

`st`

mm · intervalo: 0–10

### Angina durante o teste

`angina`

- `0` — Não
- `1` — Não limitante
- `2` — Limitante (motivo da interrupção)

## Edição do método

Duke Treadmill/Mark 1987:tempo−5 ST−4 angina; nomograma validado 1991

## Fórmula documentada

Escore = tempo de exercício (min) − 5 × desnível do ST (mm) − 4 × índice de angina (0 = ausente, 1 = não limitante, 2 = limitante).

## Limites e população

O Duke Treadmill Score de 1987 foi desenvolvido para prognóstico em pessoas com dor torácica submetidas a teste de esteira e cateterismo. A fórmula depende das convenções de tempo, desvio de ST e índice de angina do protocolo. O prognóstico do escore não confirma diagnóstico coronário nem a segurança de realizar esforço em uma pessoa.

## Referências

- [Mark DB et al. Exercise treadmill score for predicting prognosis in coronary artery disease. Ann Intern Med, 1987.](https://doi.org/10.7326/0003-4819-106-6-793)

- [Mark DB et al. Prognostic value of a treadmill exercise score in outpatients with suspected coronary artery disease. N Engl J Med, 1991.](https://doi.org/10.1056/NEJM199109193251204)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
