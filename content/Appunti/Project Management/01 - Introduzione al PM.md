---
tags:
  - PM
---
Metodologia: **Agile**.
Stakeholder: chi ne risente del tuo progetto.
## Chi è il Project Manager?

Il Project Manager è responsabile della pianificazione e controllo di progetti, dall’idea sino al loro completamento. Coordina persone e processi con l’obiettivo di consegnare progetti nel tempo, budget e nei requisiti richiesti per raggiungere uno o più obiettivi.

Il triangolo del PM: tempo, costo e raggio si uniscono per determinare la **qualità** del progetto.

``` mermaid
graph LR
  S0(Tempo)
  T1(Costo)
  T2(Raggio)
  S0<-->T1
  S0<-->T2
  T1<-->T2
```

Se voglio fare di più, spenderò di più.
## Progetto vs Processo

**Progetto**: uno sforzo temporaneo intrapreso per creare un servizio o un risultato di progetto unico, in un lasso di tempo definito.
**Processo**: insieme di attività eseguite ripetutamente, con lo scopo di ottenere lo stesso risultato.
In breve, un progetto è unico, il processo no.
## Cosa significa pianificare

La pianificazione è il processo di pensare alle attività richieste per il raggiungimento degli obiettivi desiderati.
Regola delle cinque W (e una H):
- Who
- What
- When
- Where
- Why
- How
## Tipologie di progetto e PM

### Predittivo vs Adattivo

**Predittivo**: in grado di consentire anticipazioni e previsioni.
- Guidato da un piano
- Requisiti fissi
- Analisi utente più importante della scoperta
- Grande sforzo di Design all’inizio
- Architettura predefinita
- Stime fornite all’inizio
- Previsioni basate sulle stime iniziali
- Tutti i requisiti hanno la stessa priorità

**Adattivo**: che favorisce o consente l'adattamento.
- Guidato dalla pianificazione
- Requisiti variabili
- La scoperta è più importante dell’analisi
- Sforzo minimo indispensabile di Design all’inizio
- Architettura si evolve
- Stime in costante aggiornamento
- Previsioni basate sul lavoro già svolto
- Requisiti prioritizzati a seconda del loro valore per l’utente

| Predittivo                                | Adattivo                                          |
|-------------------------------------------|---------------------------------------------------|
| Plan driven                               | Planning driven                                   |
| Requirements/scope fixed                  | Requirements/scope flexible                       |
| Uses discovery over analisys              | Uses analisys over discovery                      |
| Big upfront design                        | Initial upfront design                            |
| Architecture pre-determined               | Architecture evolves                              |
| Estimates given up-front                  | Estimates constantly revised                      |
| Forecasting based on upfront estimates    | Forecasts driven by work already delivered        |
| Requirements treated as of equal priority | Requirements prioritised by value of the business |

A volte è meglio usare un mix tra predittivo e adattivo $\to$ ES: fare un progetto predittivo ogni due settimane.
### Waterfall vs Agile

Il **Waterfall** è il migliore processo di pianificazione predittiva.
L'**Agile** è il miglior processo di pianificazione adattiva.

![](https://lh6.googleusercontent.com/L6_zn6uqI5-HykGc0cJrMTaT4sO6rIzdpyQjPObINlvWW29IxuKtppSiprlN6Sp67XVxJKwdFlK03Fh0gTAkaOd1SVwR6eeVMO0I2aCt79k1-nUh30x40TtflJ9dqs9myb_i3uS7v7oxnweyXpK7Dg=s2048)

**Waterfall**: Il modello a cascata è il più tradizionale modello di ciclo di vita del software. Secondo questo modello, il processo di realizzazione del software è strutturato in una sequenza lineare di fasi o passi.
**Agile**: i metodi agili propongono un approccio focalizzato sull'obiettivo di consegnare al cliente, in tempi brevi e frequentemente, software funzionante e di qualità.
### Profilo di rischio

Con un metodo predittivo, il profilo di rischio diminuisce solo verso la fine del progetto, mentre all'inizio del progetto il rischio è altissimo.
Con un metodo adattivo, invece, il rischio rimane basso indipendentemente dalla fase del progetto.
### Evoluzione del progetto

**Metodo Waterfall**: Lo stato di progetto tende ad allontanarsi dall’esigenza reale del business, perché questa varia nel tempo, mentre il progetto inizia e finisce con requisiti fissi e invariabili.
![](https://lh4.googleusercontent.com/hQjJU8WmiUN3WXmol8h4Ar4Q8940bzeMvEu49abODEBcfaFik0pvKpSnHncZR_qSVNDvfGNqX43vCPComQSwZqAxftV3Pnr3EV2rr8kLF1DY3ob6I3_31gMQGa6f71YSY8_8sR6CqDN9oEATIncUHg=s2048)

**Metodo Agile**: Lo stato di progetto si avvicina ad ogni iterazione all’esigenza reale del business, perché questa varia nel tempo, ed il progetto si _adatta_ alle nuove esigenze.
![](https://lh6.googleusercontent.com/k5Z52BHLEeVsC9TLV6bpwYDPf_nJCemQCfZhscDR9zF3SV0Pc0kixB0YdxfbGTyBd64_c7g7h_UgHKDM5VzYBGdUzv9xz-tLkqKwfgmMcw2QEvRS5v9TuPiFBlCN5Iu71Lbcgv5SS6GMlXST-sUT6A=s2048)

Quindi: qual'é il metodo migliore tra l'Agile e il Waterfall? Dipende, non sempre è melio l'Agile.