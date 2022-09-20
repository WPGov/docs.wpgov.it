# Shortcode

## Lista delle sezioni

Questo shortcode genera la lista delle sezioni previste dalla normativa e può essere inserito in una pagina.

Si consiglia di creare una nuova pagina "Amministrazione Trasparente" con slug `/amministrazione-trasparente` e inserire lo shortcode.

Ai fini della trasparenza e per la convalida da parte di comuni bot di compliance screening, si consiglia di inserire un link diretto dalla homepage.

`[at-sezioni col="2" bar="2" con="1"]`

| Parametro | Valori ammissibili |Default |Note |
|-----------|-----------|-----------|-----------|
|col|1-2-3|1|Numero di colonne|
|bar|0-1-2|0|0 = non visualizzare la barra superiore.<br></br>1 = visualizza la barra con ricerca e link archivio<br></br>2 = visualizza la barra con ricerca, link archivio e descrizione |
|con|0-1|0|0 = non visualizzare il contatore di voci/sezione<br></br>1 = visualizza il contatore di voci/sezione|

## Altri shortcode

| Shortcode | Note |
|-----------|-----------|
|`[at-desc]`|Mostra la descrizione di Amministrazione Trasparente.|
|`[at-search]`|Mostra un box orizzontale per la ricerca in A.T., con filtro per tipologia|
|`[at-head]`|Mostra un sommario delle voci cliccabili. Da usare nella stessa pagina di [at-list] o [at-table]|
|`[at-list]`|Visualizza una lista di tutte le voci/sottovoci(**deprecato**)|
|`[at-table]`|Visualizza una lista delle sezioni in 2 colonne (**deprecato**)|

## Utilizzo nel template

Tutti gli shortcode possono essere utilizzati all'interno di template php o integrazioni custom, tramite l'utilizzo della seguente chiamata:

`<?php echo do_shortcode('[at-list]') ?>`