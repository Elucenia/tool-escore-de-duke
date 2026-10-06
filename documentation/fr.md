<!-- ELUCENIA technical documentation · escore-de-duke · fr · no clinical/professional/rights approval -->

# Score de Duke (épreuve d’effort sur tapis)

[conditions, sources et autorisations](https://elucenia.org/fr/outils/escore-de-duke)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Durée de l’effort (protocole de Bruce)

`tempo`

min · intervalle: 0–30

### Déviation maximale du ST (dans toute dérivation sauf aVR)

`st`

mm · intervalle: 0–10

### Angor pendant le test

`angina`

- `0` — Non
- `1` — Non limitante
- `2` — Limitante (motif d’arrêt)

## Édition de la méthode

Duke Treadmill/Mark 1987 : durée−5ST−4angor ; nomogramme validé 1991

## Formule documentée

Score = durée d’exercice (min) − 5 × déviation ST (mm) − 4 × indice d’angor (0 = absent, 1 = non limitant, 2 = limitant).

## Limites et population

Le Duke Treadmill Score de 1987 a été développé pour le pronostic chez des personnes présentant une douleur thoracique et ayant subi une épreuve d’effort sur tapis roulant et un cathétérisme. La formule dépend des conventions de durée, de déviation ST et d’indice d’angor du protocole. Le pronostic du score ne confirme ni le diagnostic coronarien ni la sécurité d’un effort chez une personne.

## Références

- [Mark DB et al. Exercise treadmill score for predicting prognosis in coronary artery disease. Ann Intern Med, 1987.](https://doi.org/10.7326/0003-4819-106-6-793)

- [Mark DB et al. Prognostic value of a treadmill exercise score in outpatients with suspected coronary artery disease. N Engl J Med, 1991.](https://doi.org/10.1056/NEJM199109193251204)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Résultats documentés

Les informations ci-dessous conservent les sorties de la méthode pour des exemples synthétiques. Elles ne constituent pas une validation clinique indépendante.

### 1

Risque intermédiaire

| Détails du résultat | |
| --- | --- |
| Mortalité annuelle estimée | 1,25% |


### 2

Faible risque

| Détails du résultat | |
| --- | --- |
| Mortalité annuelle estimée | 0,25% |


### 3

Risque élevé

| Détails du résultat | |
| --- | --- |
| Mortalité annuelle estimée | 5,25% |

