# FAQ

## Installazione

**Da repo wordpress.org:**
1. Accedi a "Plugins" e cerca "Amministrazione Trasparente"
2. Installa e attiva il plugin

**Installazione manuale:**
1. Scarica il pacchetto aggiornato da https://it.wordpress.org/plugins/amministrazione-trasparente/
2. Carica il contenuto estratto nella cartella `/wp-content/plugins/`
3. Attiva il plugin dal menu ‘Plugins’ in WordPress

## Come inserisco una nuova voce?
Per inserire le voci seleziona, dal menù di amministrazione, Trasparenza > Nuova Voce

## Compatibilità

### Template

Questo plugin funziona con la maggior parte dei temi WordPress.

Viene inoltre garantita compatibilità e perfetta coerenza grafica con i seguenti template:

- Pasw2013
- Pasw2015

### Breadcrumb NavXT
A partire dalla versione 3.2 di Amministrazione Trasparente, il plugin mostra automaticamente le briciole di pane per Pasw2013 e Pasw2015. Chi non usa uno di questi temi può comunque installare il plugin Breadcrumb NavXT configurandolo manualmente o ricorrere a soluzioni differenti (il risultato gerarchico potrebbe differire).

La gerarchia ideale per le briciole di pane in Amministrazione Trasparente potrebbe essere del tipo **Home > Amministrazione Trasparente** (pagina) ** > Sottosezione** (archivio) **> NomeVoce** (articolo singolo).
Data la diversa natura delle varie parti delle briciole di pane, è necessario procedere ad un’accurata messa a punto del plugin Breadcrumb NavXT che supporta questo tipo di configurazioni.
Per effettaure queste modifiche, accedere al back-end di WordPress e cliccare su Impostazioni -> Breadcrumb NavXT -> Tipi di post.
Tutte le opzioni da cambiare sono raccolte in [questa guida](http://supporto.marcomilesi.ml/2014/breadcrumb-navxt-e-le-briciole-di-pane/).

## Problemi comuni

### Errore 404

**Problema:** i contenuti e le sezioni di Amministrazione Trasparente ritornano errore 404 - non trovato

**Soluzione:** aggiornare i permalink da Impostazioni -> Permalink

### Descrizione sezione nelle pagine di archivio

Chi non utilizza un tema PASW può comunque abilitare la visualizzazione della descrizione espandibile e il link ‘Torna al sommario’ sotto il titolo degli archivi dei documenti modificando il file archive.php (il nome può cambiare) dalla cartella contenente i file del tema attivo.

Per abilitarla, aprire il file aggiungendo

`<?php if (function_exists('at_archive_buttons')) { at_archive_buttons(); } ?>`

subito sotto al codice che genera il titolo.