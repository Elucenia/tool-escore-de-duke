<!-- ELUCENIA technical documentation · escore-de-duke · it · no clinical/professional/rights approval -->

# Punteggio di Duke (test su tapis roulant)

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/escore-de-duke)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Tempo di esercizio (protocollo di Bruce)

`tempo`

min · intervallo: 0–30

### Massima deviazione del ST (in qualsiasi derivazione tranne aVR)

`st`

mm · intervallo: 0–10

### Angina durante il test

`angina`

- `0` — No
- `1` — Non limitante
- `2` — Limitante (motivo dell’interruzione)

## Edizione del metodo

Duke Treadmill/Mark 1987: tempo−5ST−4angina; nomogramma validato 1991

## Formula documentata

Score = durata esercizio (min) − 5 × deviazione ST (mm) − 4 × indice angina (0 = assente, 1 = non limitante, 2 = limitante).

## Limiti e popolazione

Il Duke Treadmill Score del 1987 è stato sviluppato per la prognosi in persone con dolore toracico sottoposte a test su tapis roulant e cateterismo. La formula dipende dalle convenzioni del protocollo per tempo, deviazione ST e indice di angina. La prognosi del punteggio non conferma la diagnosi di coronaropatia né la sicurezza di sottoporre una persona a uno sforzo.

## Riferimenti

- [Mark DB et al. Exercise treadmill score for predicting prognosis in coronary artery disease. Ann Intern Med, 1987.](https://doi.org/10.7326/0003-4819-106-6-793)

- [Mark DB et al. Prognostic value of a treadmill exercise score in outpatients with suspected coronary artery disease. N Engl J Med, 1991.](https://doi.org/10.1056/NEJM199109193251204)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Risultati documentati

Le informazioni seguenti conservano gli output del metodo per esempi sintetici. Non costituiscono una validazione clinica indipendente.

### 1

Rischio intermedio

| Dettagli del risultato | |
| --- | --- |
| Mortalità annua stimata | 1,25% |


### 2

Rischio basso

| Dettagli del risultato | |
| --- | --- |
| Mortalità annua stimata | 0,25% |


### 3

Rischio elevato

| Dettagli del risultato | |
| --- | --- |
| Mortalità annua stimata | 5,25% |

