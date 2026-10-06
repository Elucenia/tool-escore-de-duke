<!-- ELUCENIA technical documentation · escore-de-duke · de · no clinical/professional/rights approval -->

# Duke-Treadmill-Score

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/escore-de-duke)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Belastungsdauer (Bruce-Protokoll)

`tempo`

min · Bereich: 0–30

### Größte ST-Abweichung (in jeder Ableitung außer aVR)

`st`

mm · Bereich: 0–10

### Angina pectoris während des Tests

`angina`

- `0` — Nein
- `1` — Nicht limitierend
- `2` — Limitierend (Abbruchgrund)

## Fassung der Methode

Duke Treadmill/Mark 1987: Zeit−5ST−4Angina; Nomogramm 1991 validiert

## Dokumentierte Formel

Score = Belastungszeit (min) − 5 × ST-Abweichung (mm) − 4 × Anginaindex (0 = keine, 1 = nicht limitierend, 2 = limitierend).

## Grenzen und Population

Der Duke Treadmill Score von 1987 wurde zur Prognose bei Personen mit Brustschmerzen entwickelt, die Laufbandtest und Katheteruntersuchung erhielten. Die Formel hängt von den Protokollkonventionen zu Dauer, ST-Abweichung und Anginaindex ab. Die Scoreprognose bestätigt weder eine Koronardiagnose noch die Sicherheit körperlicher Belastung bei einer Person.

## Referenzen

- [Mark DB et al. Exercise treadmill score for predicting prognosis in coronary artery disease. Ann Intern Med, 1987.](https://doi.org/10.7326/0003-4819-106-6-793)

- [Mark DB et al. Prognostic value of a treadmill exercise score in outpatients with suspected coronary artery disease. N Engl J Med, 1991.](https://doi.org/10.1056/NEJM199109193251204)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Dokumentierte Ergebnisse

Die folgenden Angaben bewahren die Ausgaben der Methode für synthetische Beispiele. Sie stellen keine unabhängige klinische Validierung dar.

### 1

Intermediäres Risiko

| Ergebnisdetails | |
| --- | --- |
| Geschätzte jährliche Mortalität | 1,25% |


### 2

Niedriges Risiko

| Ergebnisdetails | |
| --- | --- |
| Geschätzte jährliche Mortalität | 0,25% |


### 3

Hohes Risiko

| Ergebnisdetails | |
| --- | --- |
| Geschätzte jährliche Mortalität | 5,25% |

