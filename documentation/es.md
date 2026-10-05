<!-- ELUCENIA technical documentation · escore-de-duke · es · no clinical/professional/rights approval -->

# Puntuación de Duke (cinta ergométrica)

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/escore-de-duke)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Tiempo de ejercicio (protocolo de Bruce)

`tempo`

min · intervalo: 0–30

### Máxima desviación del ST (en cualquier derivación excepto aVR)

`st`

mm · intervalo: 0–10

### Angina durante la prueba

`angina`

- `0` — No
- `1` — No limitante
- `2` — Limitante (motivo de interrupción)

## Edición del método

Duke Treadmill/Mark 1987: tiempo−5ST−4angina; nomograma validado 1991

## Fórmula documentada

Score = tiempo de ejercicio (min) − 5 × desviación ST (mm) − 4 × índice de angina (0 = ausente, 1 = no limitante, 2 = limitante).

## Límites y población

El Duke Treadmill Score de 1987 se desarrolló para el pronóstico en personas con dolor torácico sometidas a prueba de esfuerzo en cinta y cateterismo. La fórmula depende de las convenciones de tiempo, desviación del ST e índice de angina del protocolo. El pronóstico de la puntuación no confirma enfermedad coronaria ni la seguridad de realizar esfuerzo en una persona.

## Referencias

- [Mark DB et al. Exercise treadmill score for predicting prognosis in coronary artery disease. Ann Intern Med, 1987.](https://doi.org/10.7326/0003-4819-106-6-793)

- [Mark DB et al. Prognostic value of a treadmill exercise score in outpatients with suspected coronary artery disease. N Engl J Med, 1991.](https://doi.org/10.1056/NEJM199109193251204)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
