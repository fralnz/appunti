---
tags:
  - PM
---
## Monitorare il progetto Agile
**Monitorare** un progetto in corso di svolgimento è parte fondamentale del lavoro del Project Manager / Scrum Master ed è necessario al fine di prevenire o mitigare situazioni che possono recare danno al progetto.
Il 98% delle startup falliscono perché non si **autosostengono**.
Calcolo del **rischio** = impatto / probabilità.
![[DiagrammaRischio.png]]

Elementi per il monitoraggio di un progetto agile:
- Velocità pianificata del team vs velocità effettiva;  
- Data di fine progetto attesa, minima e massima;
- Variazioni di costo minime e massime.
### Velocità del progetto
Durante la pianificazione di un progetto scrum, identificheremo una velocità media del team.
Tuttavia, questa potrebbe **variare** durante gli sprint e avere un impatto sulla data di consegna del progetto.
![[VelocitaEffettiva.png]]
Best case scenario: Tutti gli sprint alla velocità massima;
Worst case scenario: tutti gli sprint alla velocità minima;
Most likely scenario: tutti gli sprint alla velocità media.

Team Velocity = Total Story Points Completed Per Sprint / Number of Sprints (last 3/4).

### Come monitorare un progetto Agile
Nei progetti Scrum o Kanban, esistono diversi grafici per il controllo e monitoraggio dei progetti:
- [[#Burndown|Burndown chart]]
- [[#Burnup|Burnup chart]]
- [[#Sprint Report|Sprint report]]
- [[#Diagrammi cumulativi|Diagrammi cumulativi]]
#### Burndown
![[Burndown.png]]
Il burndown parte dal numero totale degli SP e ha come obiettivo ridurli fino a zero. Fornisce una chiara indicazione temporale dello sprint, con una barra che identifica il percorso ideale per “bruciare” tutti gli story point di uno sprint.
Viene poi riportato l’andamento attuale del team e dello sprint.
E’ evidente notare un andamento fuori dalle previsioni sia in negativo che in positivo.
**NB**: Questo grafico ha una rappresentazione diagonale. Di solito è difficile che le righe siano diagonali, è molto più probabile che si generino dei **gradini**.
#### Burnup
![[Burnup.png]]
Il Burnup chart fornisce una chiara indicazione degli story points **completati**.
Differentemente dal primo, in questo grafico la barra totale degli story point viene mostrata in orizzontale da sinistra a destra, mentre la diagonale indica sempre il percorso ideale.
Mostrando il totale degli story point con la barra orizzontale, è immediatamente visibile in caso ci siano variazioni di scope nello sprint.
#### Sprint Report
![[SprintReport.png]]
Lo Sprint Report mostra l'elenco dei problemi in ogni sprint. È utile per le tue riunioni Sprint Retrospective e anche per i controlli di avanzamento a metà sprint.
E' l'unione di [[#Burndown|burndown]] e attività completate e non completate.
Lo Sprint report riporta:
- Grafico Burndown dello sprint
- Resoconto di tutte le attività svolte nello sprint
- Attività pianificate
- Attività completate
- Attività non completate
- Attività rimosse
- Attività completate fuori dallo sprint
#### Diagrammi cumulativi
![[DiagrammaCumulativo.png]]
Il diagramma cumulativo, di base, rappresenta l'**accumulo di qualcosa**.
Sono molto utili per monitorare l’avanzamento di specifiche attività nel tempo:
- Quanti bug creati vs quanti bug risolti;
- Quante story aggiunte al backlog vs quante story completate;
- Quanti test pianificati vs quanti test automatizzati.
### Diagrammi di Gantt
Elementi fondamentali di un diagramma di Gantt:
- Linea temporale (suddivisa anche in sprint se possibile);
- Attività nidificate;
- Possibili dati su allocazione risorse.
![[Gantt.png]]
Conviene usare i diagrammi di Gantt per:
- Roadmap;
- Programmi;
- Gestione di grandi progetti con una durata temporale medio lunga 1+ anni.