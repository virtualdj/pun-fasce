# pun-fasce

Mostra i costi del PUN di un anno, diviso per mesi e fasce orarie (F1, F2 e F3).
I valori vengono scaricati dal sito [MercatoElettrico.org](https://www.mercatoelettrico.org/it-it/Home/Esiti/Elettricita/MGP/Statistiche/DatiStorici).

È stato aggiunto anche il valore della fascia mono-oraria e F23, quest'ultima basata su calcoli documentati non in modo perfetto ma che sembrano portare a risultati identici (o perlomeno simili) alle tariffe ufficiali.

## Installazione dei prerequisiti

`python3 -m pip install -r ./requirements.txt`

## Utilizzo

`python3 ./pun-fasce.py <anno>`

L'`anno` è opzionale e in quel caso si intende l'anno corrente.  
Il risultato è simile a questo:

```text
Mese	MO (€/kWh)	F1 (€/kWh)	F2 (€/kWh)	F3 (€/kWh)	F23 (€/kWh)
1/2026	0.132660	0.151260	0.137400	0.118290	0.127081
2/2026	0.114410	0.122280	0.119840	0.105300	0.111988
3/2026	0.143400	0.143020	0.153910	0.138090	0.145367
4/2026	0.119470	0.111140	0.138260	0.116630	0.126580
```
