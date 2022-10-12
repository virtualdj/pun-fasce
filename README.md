# pun-fasce

Mostra i costi del PUN di un anno, diviso per mesi e fasce orarie (F1, F2 e F3).
I valori vengono scaricati dal sito [MercatoElettrico.org](https://www.mercatoelettrico.org/It/Default.aspx).

## Installazione dei prerequisiti

`python3 -m pip install -r ./requirements.txt`

## Utilizzo

`python3 ./pun-fasce.py <anno>`

L'`anno` può non essere specificato (in quel caso si intende l'anno corrente).
Il risultato è simile a questo:

```text
Mese    F1 (€/kWh)      F2 (€/kWh)      F3 (€/kWh)
1/2022  0.257190        0.242350        0.196390
2/2022  0.224880        0.225680        0.193650
3/2022  0.320080        0.329120        0.286190
4/2022  0.256230        0.266580        0.228860
```
