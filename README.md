# Controlli Qualita

| Parametro | Descrizione |
| --- | --- |
| pr | Daily precipitation amount |
| Tx | Daily maximum temperature |
| Tm | Daily mean temperature |
| Tn | Daily minimum temperature |

Controlli di qualità implementati da SCIA e altri organismi

| Precipitazione | ECA&D |
| --- | --- |
| Soglie fisse | pr < 300 mm & pr >= 0 mm |
| Persistenza valori > 1.0 mm | Non deve ripetersi lo stesso valore per >= 10 gg |
| Persistenza valori > 5.0 mm | Non deve ripetersi lo stesso valore per >= 5 gg |
| Dry days period: suspect | if the amount of drydays liesoutside a 14·bivariate standard deviation |

| Tx | ECA&D |
| --- | --- |
| Soglie fisse | Tx < 60 °C & Tx > -90 °C |
| Soglie variabili | Tx >= Tn |
| Soglie variabili | Tx >= Tm |
| Persistenza valori | **Non deve ripetersi lo stesso valore per >= 5 gg** |



## Riferimenti

- [ECA&D](https://www.ecad.eu/documents/atbd.pdf)


