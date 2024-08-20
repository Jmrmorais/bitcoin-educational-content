---
term: NULLDUMMY
---

Правило консенсуса, введенное с BIP147 в мягком форке SegWit, требующее, чтобы фиктивный элемент, используемый в опкодах `OP_CHECKMULTISIG` и `OP_CHECKMULTISIGVERIFY`, был пустым байтовым массивом (`OP_0`). Эта мера была реализована для устранения вектора изменчивости, запрещая использование любого значения, отличного от `OP_0`, для этого элемента.