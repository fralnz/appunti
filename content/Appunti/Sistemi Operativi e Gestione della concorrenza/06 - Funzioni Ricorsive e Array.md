---
tags:
  - OS
  - esercizi
---
# Fattoriale
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

# Array
Facciamo un programma che somma i valori contenuti in un array da 10 elementi:
```c
#include <stdio.h>  
  
int somma (int *array){    //in alternativa si può fare array[], ma con l'asterisco indichiamo che stiamo passando un indirizzo 
    int tot = 0;  
    for (int i=0; i<10 ; ++i){  
        tot = tot + *array;  
        array++;    // aumenta di 4 l'indirizzo dell'array, progredendo nello stack  
    }  
    return tot;  
}  
  
int main() {  
    int valori[10] = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};   //popoliamo l'array
    int sommavalori = somma(valori);   //sommavalori sarà 55
    return 0;
}
```
E' importante notare che quando si passa l'indirizzo di un array con <code>*array</code>, si passa l'indirizzo della prima cella dell'array.
# Stringhe (array di caratteri)
Facciamo un programma che conta il numero di caratteri in una stringa:
```c
#include <stdio.h>  
  
int lunghezzastringa(char *stringa){  
    int lunghezza = 0;  
    for (;;){  
        char c = *stringa;  
        if (c == 0) break;  
        lunghezza++;  
        stringa++;  //non metto *stringa++ perchè l'asterisco punta al contenuto, quindi se aumento di 1 il contenuto di stringa, passa alla lettera dopo  
    }  
    return lunghezza;  
}  
  
int main() {  
    char parola[100] = "CIAO";  
    int l = lunghezzastringa(parola);  
    return 0;  
}
```
## Organizziamolo in più file
Anzichè mettere tutte le funzioni in un unico file sorgente, si possono definire le funzioni in file separati.
**Ad esempio**: <code>main.c</code>, <code>stringhe.c</code>, <code>stringhe.h</code>.
main.c:
```c
#include <stdio.h>  
#include "stringhe.h"  
  
int main() {  
    char parola[100] = "CIAO";  
    int l = lunghezzastringa(parola);  
    return 0;  
}
```
**stringhe.c**:
```c
#include "stringhe.h"  
  
int lunghezzastringa(char *stringa){  
    int lunghezza = 0;  
    for (;;){  
        char c = *stringa;  
        if (c == 0) break;  
        lunghezza++;  
        stringa++;  //non metto *stringa++ perchè l'asterisco punta al contenuto, quindi se aumento di 1 il contenuto di stringa, passa alla lettera dopo  
    }  
    return lunghezza;  
}
```
**stringhe.h**:
```c
// prototipo della funzione  
int lunghezzastringa(char *stringa);
```