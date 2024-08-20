---
term: RECURSIVE (COVENANT)
---

Рекурсивный ковенант в Bitcoin — это тип смарт-контракта, который накладывает условия не только на текущую транзакцию, но и на будущие транзакции, которые используют выходы этой транзакции. Это позволяет создавать цепочки транзакций, где каждая должна соответствовать определенным правилам, установленным первой в цепочке. Рекурсивность создает последовательность транзакций, где каждая наследует ограничения от своей родительской транзакции. Это позволило бы осуществлять сложный и долгосрочный контроль над тем, как можно тратить биткоины, но также вводило бы риски, касающиеся свободы трат и взаимозаменяемости.

Подводя итог, не рекурсивный ковенант ограничивал бы себя только транзакцией, которая непосредственно следует за установившей правила транзакцией. В отличие от этого, рекурсивный ковенант имеет возможность накладывать конкретные условия на биткоин на неопределенный срок. Транзакции могут следовать одна за другой, но биткоин всегда будет сохранять первоначальные условия, прикрепленные к нему. Технически, установление не рекурсивного ковенанта происходит, когда `scriptPubKey` UTXO определяет ограничения на `scriptPubKey` выходов транзакции, которая тратит данный UTXO. С другой стороны, установление рекурсивного ковенанта происходит, когда `scriptPubKey` UTXO определяет ограничения на `scriptPubKey` выходов транзакции, которая тратит данный UTXO, и на все последующие `scriptPubKey`, которые будут следовать за тратой этого UTXO.

Более обще, в вычислительной технике то, что называется "рекурсивностью", это способность функции вызывать саму себя, создавая своего рода петлю.