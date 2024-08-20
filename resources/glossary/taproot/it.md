---
termine: TAPROOT
---

Un importante aggiornamento del protocollo Bitcoin, adottato tramite un soft fork nel novembre 2021. Questo aggiornamento porta significativi miglioramenti in termini di privacy, efficienza e flessibilità implementando BIP340, BIP341 e BIP342. Questo aggiornamento è stato bloccato al blocco 687,284 il 12 giugno 2021, quando il 90% dei blocchi generati durante un periodo ha segnalato a favore, indicando così la prontezza dei minatori ad attivare l'aggiornamento (*Speedy Trial*). L'attivazione è avvenuta effettivamente al blocco 709,632 il 14 novembre 2021, quasi quattro anni dopo le discussioni iniziali sulla questione tra Pieter Wuille, Andrew Poelstra e Gregory Maxwell. È stato il primo tentativo di aggiornamento maggiore dal contestato attivazione di SegWit nel 2017.

Taproot è anche il nome di BIP341, implementato all'interno del soft fork omonimo, che introduce un nuovo modello di script denominato P2TR. Uno script P2TR blocca i bitcoin su una chiave pubblica Schnorr unica, denotata come $K$. Tuttavia, questa chiave $K$ è in realtà un aggregato di una chiave pubblica $P$ e di una chiave pubblica $M$, quest'ultima calcolata dalla radice di Merkle di un elenco di `scriptPubKey`. I bitcoin bloccati con uno script P2TR possono essere spesi in due modi distinti: o pubblicando una firma per la chiave pubblica $P$, o soddisfacendo uno degli script contenuti nell'albero di Merkle. La prima opzione è chiamata "*key path*" e la seconda "*script path*".