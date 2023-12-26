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
Mese    MO (€/kWh)      F1 (€/kWh)      F2 (€/kWh)      F3 (€/kWh)      F23 (€/kWh)
1/2023  0.174490        0.196240        0.184240        0.155100        0.168504
2/2023  0.161070        0.174330        0.172890        0.144220        0.157408
3/2023  0.136380        0.139780        0.151950        0.124660        0.137213
4/2023  0.134970        0.135550        0.152050        0.126400        0.138199
```
