---
tags:
  - algo
---
# Elementi mutabili e immutabili
Costituiti da **chiavi** e **valori**.
Variabili:
- **Immutabili**: interi, floating, booleani, stringhe, caratteri, tuple.
- **Mutabili**: liste, dizionari, set/insiemi.
## Tuple
Le **tuple** sono liste immutabili, racchiuse tra parentesi tonde.
```python
tupla = tuple(immutabile)
tupla
lista = list(tupla)   #casting da tupla a lista
lista
```
La tupla viene usata per conservare dati in maniera immutabile. Nel caso in cui la tupla conservi elementi mutabili, essi possono essere modificati.
## Stringa
Non si possono modificare le stringhe in python, in quanto immutabili.
```python
y = 'floating'
print(y[0])
y[0] = 'F'   #cerchiamo di cambiare la prima lettera della stringa rendendola maiuscola
```
Il codice sopra da **errore**! Ecco una versione corretta:
```python
y = 'floating'
print(y[0])
y = y.capitalize()
```
## Dizionario
Per creare un dizionario vuoto:
```python
dizionario = dict()
dizionario.keys()   #stampa le chiavi del dizionario
dizionario.values()   #stampa i valori del dizionario
dizionario.items()   #riporta chiavi e valori come se fossero tuple
```
