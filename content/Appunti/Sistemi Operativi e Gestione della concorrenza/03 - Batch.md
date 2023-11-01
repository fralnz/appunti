BIOS: Basic Input Output Software
Il bios, una volta riconosciuto il disco, ne legge i settori (grandi 512 byte) che introducono il SO.
**Processo**: un programma in esecuzione.
Un processo usa:
- CPU
- Memoria
- Risorse hardware
**Programma**: insieme di istruzioni che vengono eseguite dal processore durante il fetch.
**Task**: una attività che uno user richiede ad una elaboratore "attivita' di calcolo". Normalmente viene svolta da un processo. Produce un risultato "spendibile" da un essere umano.
**Job**: Termine obsoleto, designava una attività all' Interno del SO.
Ora sostituito da Processo. Si usa ancora nel SO realtime per designare pes. Attività NON ripetitive.
# Layout di un Processo
- Text section: il codice eseguibile
- Data section: variabili globali
- Heap section: memoria allocata dinamicamente durante l'esecuzione del programma
- Stack section: spazio temporaneo quando si invocano funzioni (variabili locali, return adress...)
![[LayoutProcesso.png|200]]
**Record di attivazione**: una parte di stack che viene chiamata prima di fare una chiamata ad una funzione.