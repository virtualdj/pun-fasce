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
1/2025	0.143030	0.158320	0.151610	0.128540	0.139152
2/2025	0.150360	0.157640	0.158950	0.139910	0.148668
3/2025	0.120550	0.121680	0.134860	0.111650	0.122327
4/2025	0.099850	0.095840	0.115080	0.095050	0.104264
5/2025	0.093580	0.089090	0.110640	0.087110	0.097934
6/2025	0.111780	0.113060	0.126760	0.103630	0.114270
7/2025	0.113130	0.108960	0.127100	0.108490	0.117051
8/2025	0.108790	0.105580	0.117970	0.106040	0.111528
9/2025	0.109080	0.109590	0.120930	0.101880	0.110643
10/2025	0.111040	0.117830	0.121660	0.099480	0.109683
```
