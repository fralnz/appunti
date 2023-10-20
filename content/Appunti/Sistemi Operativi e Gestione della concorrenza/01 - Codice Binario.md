---
tags:
  - OS
---

## Introduzione

Numeri _arabi_: 145 ... $\leftarrow$ scrittura posizionale;
Numeri romani: XL / LX $\leftarrow$ scrittura non posizionale;
Simboli **binari**: 0/1, acceso/spento, true/false.

Nel caso dell'informatica, le applicazioni sono lette dalla macchina quando scritte base binaria (2), quindi composte da 1 e 0.
**NB**: ogni numero binario che termina con 0 a destra e' pari e ogni numero binario che termina con 1 e' dispari.
Altri esempi di basi sono:
- decimale: composta da 10 cifre (da 0 a 9);
- ottale: composta da 8 cifre (da 0 a 7);
- esadecimale: composta da 16 cifre (da 0 a F). Nota che oltre il 9 si usano le lettere: A=10, B=11, ..., F=15.
## Conversione da base 10 a base B

Per convertire un numero in base 10 a base B, bisogna dividere ripetutamente il numero per B fino a che non si arriva a 0, e scrivere i resti delle divisioni in ordine inverso.
**ES**: Convertiamo il numero $13_{(10)}$ in base $2$
$13_{(10)} = ?_{(2)}$

| 13 | 2 |
| --- | --- |
| 6 | 1 |
| 3 | 0 |
| 1 | 1 |
| 0 | 1 |

$13_{(10)} = 1101_{(2)}$ 

## Conversione da base B a base 10
Se vogliamo convertire da base B a base 10, dobbiamo moltiplicare ogni cifra per $B^i$, dove $i$ e' la posizione della cifra e parte da 0. Nel caso di 1101:
$$1^{(3)}1^{(2)}0^{(1)}1^{(0)}$$
_**NB**: l'apice indica il valore di $i$_
$$
1101_{(10)}=1\times2^0+0\times2^1+1\times2^2+1\times2^3=*1+0\times2+1\times4+1\times8=1+0+4+8=13_{(10)}
$$
Se vogliamo usare basi diverse da 2 il procedimento e' analogo, basta sostituire B con la base che si vuole usare.
## Cambio di base con potenze di 2

Consideriamo:
$$41_{(16)}=X_{(8)}$$
Dividiamo i bit di X in gruppi da $log_2(B)$, dove B e' la base di X. In questo caso $log_2(8)=3$ quindi dividiamo i bit di $41_{(16)}$ scritto in binario in gruppi da 3.
Utilizzando il [[01 - Codice Binario#Conversione da base 10 a base B|procedimento di prima]], sappiamo che:
$$41_{(16)} = 1000001_{(2)}$$
Ora dividiamo i bit del numero ottenuto in gruppi da 3, aggiungendo 0 nel caso di cifre mancanti:
$$\underset{1}{001} \ \underset{0}{000} \ \underset{1}{001} \\ $$
Quindi:
$$41_{(16)} = 101_{(8)}$$
Si può verificare la correttezza della conversione usando [questo sito](https://www.rapidtables.com/convert/number/hex-to-binary.html).