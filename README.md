# pun-fasce

Mostra i costi del PUN di un anno, diviso per mesi e fasce orarie (F1, F2 e F3).
I valori vengono scaricati dal sito [MercatoElettrico.org](https://www.mercatoelettrico.org/It/Default.aspx).

È stato aggiunto anche il calcolo della fascia mono-oraria e F23, basata su calcoli documentati non in modo perfetto ma che sembrano portare a risultati identici (o perlomeno simili) alle tariffe ufficiali.

## Installazione dei prerequisiti

`python3 -m pip install -r ./requirements.txt`

## Utilizzo

`python3 ./pun-fasce.py <anno>`

L'`anno` è opzionale e in quel caso si intende l'anno corrente.  
Il risultato è simile a questo:

```text
Mese	MO (€/kWh)	F1 (€/kWh)	F2 (€/kWh)	F3 (€/kWh)	F23 (€/kWh)
1/2023	0.174490	0.196240	0.184240	0.155100	0.168504
2/2023	0.161070	0.174330	0.172890	0.144220	0.157408
3/2023	0.136380	0.139780	0.151950	0.124660	0.137213
4/2023	0.134970	0.135550	0.152050	0.126400	0.138199
5/2023	0.105730	0.109990	0.119810	0.095110	0.106472
6/2023	0.105340	0.108200	0.117960	0.096610	0.106431
7/2023	0.112090	0.114910	0.122320	0.104340	0.112611
8/2023	0.111890	0.110260	0.128120	0.104480	0.115354
9/2023	0.115700	0.118550	0.128080	0.105990	0.116151
10/2023	0.134260	0.144560	0.148630	0.119080	0.132673
11/2023	0.121750	0.139730	0.128260	0.105280	0.115851
```
