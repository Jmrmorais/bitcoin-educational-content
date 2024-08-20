---
term: REDEEMSCRIPT
---

Скрипт, который определяет конкретные условия, которые входы должны выполнить, чтобы разблокировать средства, связанные с выходом P2SH. В UTXO P2SH `scriptPubKey` содержит хеш `redeemScript`. Когда транзакция желает потратить этот UTXO в качестве входа, она должна предоставить четкий `redeemScript`, который соответствует хешу, содержащемуся в `scriptPubKey`. Таким образом, `redeemScript` предоставляется в `scriptSig` входа вместе с другими элементами, необходимыми для выполнения условий скрипта, такими как подписи или публичные ключи. Эта инкапсулированная структура обеспечивает, что детали условий расходования остаются скрытыми до тех пор, пока биткойны фактически не будут потрачены. Он особенно используется для мультиподписных кошельков Legacy P2SH.