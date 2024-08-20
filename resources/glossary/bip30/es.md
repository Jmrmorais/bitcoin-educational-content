---
term: BIP30
---

Propuesta de mejora que involucra un soft fork implementado el 15 de marzo de 2012, para resolver el problema de identificadores de transacción duplicados. Antes de BIP30, era técnicamente posible tener dos transacciones diferentes con el mismo identificador de transacción (TXID) en la blockchain. Esto ocurrió notablemente dos veces para transacciones coinbase: la del bloque 91,880 tiene el mismo TXID que la coinbase del bloque 91,722, y la del bloque 91,842 tiene el mismo TXID que la coinbase del bloque 91,812. BIP30 resolvió este fallo imponiendo una nueva regla simple: ninguna nueva transacción puede tener el mismo TXID que una transacción previamente registrada a menos que la transacción original haya sido completamente gastada (es decir, todos sus outputs hayan sido utilizados). Este soft fork fue activado utilizando el método de flag day. Por lo tanto, es uno de los primeros UASFs.