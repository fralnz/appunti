---
tags:
  - OS
  - esercizi
---
## Fattoriale
Il fattoriale in C si può fare in questo modo:
```c
#include <stdio.h>

int fattoriale(int n){
    int res = 1;
    for (int i = 1; i <= n; ++i){
        res = res * i;
    }
    return res;
}

int main() {
    int fatt = fattoriale(5);
    printf("%i", fatt);    //stampa a video il risultato, in questo caso 120
    return 0;
}
```
In alternativa, si può implementare usando le **funzioni ricorsive**:
```c
#include <stdio.h>

int fattoriale(int n){
    int res = n * (n-1);    //condizione di uscita
    if (n<=1){
        return 1;
    }
    return (n * fattoriale(n-1));    //richiamo della stessa funzione
}

int main() {
    int fatt = fattoriale(5);
    printf("%i", fatt);    //stampa a video il risultato, in questo caso 120
    return 0;
}
```
Tra i due metodi, è più efficiente **il primo**: il metodo con le funzioni ricorsive continua a spostare lo stack e assegnare celle per nuovi parametri, occupando più spazio.