# Come ho fatto il sito

Come specificato in [Home](index), questo sito e' il risultato della conversione del mio vault di Obsidian in pagine statiche per il web.

Per realizzarlo ho utilizzato [Quartz](https://quartz.jzhao.xyz/), un generatore di siti statici che converte file Markdown in pagine web.

## Requisiti

Per usare quartz servono:

- Node (minimo v18.14);

- npm (minimo v9.3.1);

- git (opzionale ma raccomandato)

## Procedimento

Scarica il codice di quartz da [GitHub](https://github.com/jackyzha0/quartz.git), puoi farlo sia manualmente che utilizzando git:

```
git clone https://github.com/jackyzha0/quartz.git
```

Dopodiche entra nella cartella scaricata con la shell e utilizza questi comandi:

```
cd quartz
npm i
npx quartz create
```
