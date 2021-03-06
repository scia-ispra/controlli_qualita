# Controlli Qualita

| Parametro | Descrizione |
| --- | --- |
| pr | Daily precipitation amount |
| Tx | Daily maximum temperature |
| Tm | Daily mean temperature |
| Tn | Daily minimum temperature |

Controlli di qualità implementati da SCIA e altri organismi

| Precipitazione | ECA&D | SCIA |
| --- | --- | --- |
| Soglie fisse | **pr < 300 mm & pr >= 0 mm** |  **pr < 800 mm & pr >= 0 mm** |
| Persistenza valori > 1.0 mm | Non deve ripetersi lo stesso valore per >= 10 gg | Non deve ripetersi lo stesso valore per >= 10 gg, senza contare i dati NA |
| Persistenza valori > 5.0 mm | Non deve ripetersi lo stesso valore per >= 5 gg | |
| Persistenza giorni asciutti | if the amount of drydays liesoutside a 14·bivariate standard deviation -> suspect | 180 o più valori nulli consecutivi |

| Tx | ECA&D | SCIA |
| --- | --- | --- |
| Soglie fisse | Tx < 60 °C & Tx > -90 °C | Tx <= 50 °C & Tx >= -30 °C |
| Soglie variabili | Tx >= Tn | **QUESTO CONTROLLO NON VIENE ESEGUITO** |
| Soglie variabili | Tx >= Tm | **QUESTO CONTROLLO NON VIENE ESEGUITO** |
| Persistenza valori | **Non deve ripetersi lo stesso valore per >= 5 gg** | **Non deve ripetersi lo stesso valore per >= 10 gg** |

| Tn | ECA&D | SCIA |
| --- | --- | --- |
| Soglie fisse | Tn < 60 °C & Tn > -90 °C | Tn <= 40 °C & Tn >= -40 °C |
| Soglie variabili | Tn <= Tx | **QUESTO CONTROLLO NON VIENE ESEGUITO** |
| Soglie variabili | Tn <= Tm | **QUESTO CONTROLLO NON VIENE ESEGUITO** |
| Persistenza valori | **Non deve ripetersi lo stesso valore per >= 5 gg** | **Non deve ripetersi lo stesso valore per >= 10 gg** |


## Note

Il volume dell'ECA&D descrive una serie di controlli per parametri diversi da temperatura e precipitazione. **Quali possono essere implementati in SCIA?**

## Riferimenti

- [ECA&D](https://www.ecad.eu/documents/atbd.pdf)


