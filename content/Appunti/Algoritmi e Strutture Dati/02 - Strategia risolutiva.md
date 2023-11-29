---
tags:
  - algo
---
Un algoritmo è la descrizione in passi sequenziali di istruzioni elementari. L'algoritmo deve arrivare sempre alla stessa soluzione in un tempo determinato. L'algoritmo non può essere ambiguo.

Esercizio 16:
```python
i = 1
array = []
numero = int(input("Inserisci un numero: "))
num = numero//2

while i<=num:
    if num%i == 0:
        array.append(i)
    i = i+1
for i in array:
    print(i)
```
Esercizio 17:
```python
#ESERCIZIO 17
parola=['C','I','A','O']
parolautente = []
while True:
    lettera = input("Inserisci una lettera: ").upper()
    for i in parola:
        if lettera == i and lettera not in parolautente:
            parolautente.insert(parola.index(i), lettera)
    for i in parolautente: print(end=i)
    print("")
    if parolautente == parola:
        break
```
