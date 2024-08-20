---
term: PAYJOIN
---

Особая структура транзакции Bitcoin, которая повышает конфиденциальность пользователя во время оплаты за счет сотрудничества с получателем платежа. Уникальность Payjoin заключается в его способности генерировать транзакцию, которая на первый взгляд выглядит обычной, но на самом деле является мини-coinjoin между двумя сторонами. Для этого структура транзакции включает в себя участие получателя платежа во входах наряду с фактическим отправителем. Таким образом, получатель включает платеж самому себе в середине транзакции, что позволяет ему получить оплату. Например, если вы покупаете багет за `6,000 сатоши`, используя UTXO на `10,000 сатоши`, и выбираете Payjoin, ваш пекарь добавит UTXO на `15,000 сатоши`, принадлежащее ему, в качестве входа, который он полностью получит обратно в виде выхода, в дополнение к вашим `6,000 сатоши`.

Транзакция Payjoin преследует две цели. Во-первых, она стремится ввести в заблуждение внешнего наблюдателя, создавая ложный след в анализе цепочки на основе эвристики общего владения входами (CIOH). Обычно, когда транзакция в блокчейне имеет несколько входов, предполагается, что все эти входы, скорее всего, принадлежат одному и тому же субъекту. Таким образом, когда аналитик рассматривает транзакцию Payjoin, он приходит к выводу, что все входы исходят от одного человека. Однако это восприятие неверно, поскольку получатель платежа также вносит свой вклад во входы наряду с фактическим плательщиком. Во-вторых, Payjoin также вводит в заблуждение внешнего наблюдателя относительно фактической суммы совершенного платежа. Изучая структуру транзакции, аналитик может подумать, что платеж эквивалентен сумме одного из выходов. На самом деле сумма платежа не соответствует ни одному из выходов. Это на самом деле разница между UTXO получателя в выходе и UTXO получателя во входе. В этом Payjoin транзакция попадает в область стеганографии. Она позволяет скрывать фактическую сумму транзакции внутри ложной транзакции, которая выступает в качестве ловушки.

![](../../dictionnaire/assets/14.png)

> ► *Payjoin иногда также называют "P2EP (Pay-to-End-Point)", "Stowaway" или "стеганографическая транзакция".*