term: ANCHOR OUTPUTS

Una proposta volta a migliorare la gestione delle commissioni di transazione all'interno dei canali Lightning. Con ogni cambio di stato in un canale Lightning, le parti interessate creano e firmano una nuova transazione di impegno che riflette la nuova distribuzione dei fondi all'interno del canale. Il problema con questo meccanismo risiede nel determinare le commissioni di transazione al momento della sua creazione. Infatti, le commissioni di transazione sulla rete Bitcoin sono soggette a significative fluttuazioni, sia verso l'alto che verso il basso. Se le commissioni stabilite per l'ultima transazione di impegno sono insufficienti al momento della chiusura unilaterale del canale, non solo la transazione impiegherà un tempo considerevole per essere confermata, ma i meccanismi di blocco temporale (timelocks) potrebbero anche consentire il furto di fondi. Gli anchor outputs riservano una piccola parte dei fondi in una transazione di impegno per coprire le future commissioni. In caso di congestione della rete e aumento delle commissioni, gli anchor outputs consentono la modifica delle commissioni di transazione dopo la creazione della transazione di impegno, garantendo così una chiusura sufficientemente rapida del canale Lightning.