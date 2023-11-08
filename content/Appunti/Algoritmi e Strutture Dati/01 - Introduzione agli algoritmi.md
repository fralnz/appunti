**Algoritmo**: elenco finito di istruzioni, che specificano le operazioni eseguendo le quali si risolve una classe di problemi.
**Programma**: ricetta che traduce l'algoritmo ed è direttamente comprensibile, pertanto eseguibile, dall'elaboratore.

5   3
2   3  (svuoto il primo nel secondo)
2   0  (svuoto il secondo)
0   2 (svuoto il primo)
ripeto

```c
//non è propriamente C, ma uno pseudocodice. Pertanto la sintassi non è la stessa del C
int Dim, Apre;
do{
	printf("Inserisci il numero delle chiavi: ");
	read(Dim);
} while(type(Dim) != int or Dim < 1);

bool Mazzo[Dim];
Apre = Random(0, Dim-1);

for (i=0, i<Dim, i++){
	if (i == Apre){
		Mazzo[i]=False;
	}else{
		Mazzo[i]=True;
	}
}

for (i=0, i<Dim, i++){
	if(Mazzo[i]==True){
		printf("La chiave che apre è la numero: ", i);
		break;
	}
}
```