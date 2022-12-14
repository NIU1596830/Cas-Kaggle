# Pràctica Kaggle APC UAB 2022-23
### Nom: Raúl Villar Casino ### DATASET: Student Grade Prediction
### URL: [kaggle](https://www.kaggle.com/datasets/dipam7/student-grade-prediction)
## Resum
S'utilitza una base de dades proporcionada per la universitat de Minho, on s'han agafat mostres d'alumnes de dues escoles: Gabriel Pereira i Mousinho da Silveira.
Tenim 395 dades amb 33 atributs. Un 87.87% d'ells és categoric i els altres són numérics sense normalitzar.
### Objectius del dataset
Volem aprender quins son els factors més importants a l'hora de que un estudiant tingui bona o mala nota.
## Experiments
Durant aquesta pràctica hem realitzat diferents experiments amb diferents atributs i manipulant les dades per a utilitzar més varietats de models.
### Preprocessat
Eliminació dels outliers, normalització de les dades, PCA, feature selection.
### Model
| Model | Hiperparametres | Mètrica |
| -- | -- | -- | -- |
| [Random Forest](link) | 100 Trees | 54.31% |
| [Kneighbors] | n=3 | 45.68% |
| [Regressió lineal] | kernel: lineal default | 66% |
| -- | -- | -- | -- |
## Conclusions
Les regressions lineals son els millors models per a predir la nota amb la base de dades otorgada, encara que la seva predicció no és precisa, posiblement per la quantitat de mostres, o perque l'informació dels atributs no és relevant.
No tota la informació obtinguda de la base de dades és relevant, més de la meitat dels atributs tenen una correlació baixa.
Encara amb tan poques mostres, podem obtenir informació valuosa a l'hora de predir notes, com per exemple la gran importancia que té la quantitat d'assignatures que has suspés previament, i l'educació dels pares de l'estudiant (els 3 atributs amb més correlació)
La base de dades tracta informació molt interesant, com la diferencia de notes entre el sexe masculí i femení, o la diferencia de notes quan un alumne consum alcohol els caps de setmana. Però desgraciadament la quantitat de mostres és massa petita com per a obtenir una conclusió real d'aquestes dades.
## Idees per treballar en un futur
Crec que seria interesant indagar més en els atributs de mitjana correlació, els quals poden donar informació molt curiosa sobre com l'entorn pot afectar a una persona.
