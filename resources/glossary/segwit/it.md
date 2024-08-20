---
term: SEGWIT
---

SegWit, acronimo di "Segregated Witness", è un aggiornamento del protocollo Bitcoin introdotto nell'agosto 2017. Ha l'obiettivo di risolvere diverse questioni tecniche, inclusi i problemi di capacità di transazione della rete, la malleabilità delle transazioni e la facilitazione di future modifiche al protocollo.

Questo soft fork modifica la struttura della transazione spostando i dati della firma in una directory separata. In particolare, con SegWit, le firme vengono rimosse dal blocco principale e inserite in una struttura dati separata alla fine del blocco, nota come i testimoni. Questa separazione consente un aumento della capacità di ciascun blocco senza modificare la dimensione massima del blocco stesso, che su Bitcoin è di 1 MB. Questo cambiamento risolve anche il problema della malleabilità delle transazioni. Prima di SegWit, le firme potevano essere alterate prima che una transazione fosse confermata, cambiando l'identificativo della transazione. Ciò rendeva difficile costruire transazioni complesse, poiché un'identificativo di una transazione non confermata poteva essere cambiato. Separando le firme, SegWit rende le transazioni non malleabili, poiché qualsiasi modifica nelle firme ora influisce solo sull'identificativo del testimone (WTXID), non sull'identificativo della transazione (TXID). Risolvendo il problema della malleabilità, SegWit ha aperto la strada a ulteriori sviluppi sul sistema Bitcoin, in particolare la Lightning Network, che consente transazioni rapide e a basso costo.