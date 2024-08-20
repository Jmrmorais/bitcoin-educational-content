---
term: VIN
---

Конкретный элемент транзакции Bitcoin, который указывает источник средств, используемых для выполнения выходов. Каждый `vin` ссылается на неизрасходованный выход (UTXO) из предыдущей транзакции. Транзакция может содержать несколько входов, каждый из которых идентифицируется с помощью комбинации `txid` (идентификатор оригинальной транзакции) и `vout` (индекс выхода в той транзакции).

Каждый `vin` включает следующую информацию:
* `txid`: идентификатор предыдущей транзакции, содержащей выход, используемый здесь в качестве входа;
* `vout`: индекс выхода в предыдущей транзакции;
* `scriptSig` или `scriptWitness`: разблокирующий скрипт, который предоставляет необходимые данные для удовлетворения условий, предъявляемых `scriptPubKey` предыдущей транзакции, чьи средства расходуются, обычно путем предоставления криптографической подписи;
* `nSequence`: специфическое поле, используемое для указания, как этот вход заблокирован по времени, а также другие опции, такие как RBF.