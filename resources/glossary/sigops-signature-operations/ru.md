---
term: SIGOPS (SIGNATURE OPERATIONS)
---

Относится к операциям с цифровой подписью, необходимым для проверки транзакций. Каждая транзакция Bitcoin может содержать несколько входов, каждый из которых может требовать одну или несколько подписей для признания действительным. Проверка этих подписей осуществляется с использованием специфических операционных кодов, называемых "sigops". В частности, это включает `OP_CHECKSIG`, `OP_CHECKSIGVERIFY`, `OP_CHECKMULTISIG` и `OP_CHECKMULTISIGVERIFY`. Эти операции накладывают определенную нагрузку на узлы сети, которые должны их проверять. Чтобы предотвратить DoS-атаки через искусственное увеличение количества sigops, протокол, таким образом, устанавливает лимит на количество sigops, разрешенное за блок, чтобы гарантировать, что нагрузка на проверку остается управляемой для узлов. В настоящее время этот лимит установлен на максимум 80 000 sigops за блок. Для подсчета узлы следуют этим правилам:

В `scriptPubKey`, `OP_CHECKSIG` и `OP_CHECKSIGVERIFY` считаются как 4 sigops. Операционные коды `OP_CHECKMULTISIG` и `OP_CHECKMULTISIGVERIFY` считаются за 80 sigops. Действительно, при подсчете, эти операции умножаются на 4, если они не являются частью входа SegWit (для P2WPKH количество sigops будет, следовательно, 1);

В `redeemScript`, операционные коды `OP_CHECKSIG` и `OP_CHECKSIGVERIFY` также считаются как 4 sigops, `OP_CHECKMULTISIG` и `OP_CHECKMULTISIGVERIFY` учитываются как `4n`, если они предшествуют `OP_n`, или 80 sigops в противном случае;

Для `witnessScript`, `OP_CHECKSIG` и `OP_CHECKSIGVERIFY` стоят 1 sigop, `OP_CHECKMULTISIG` и `OP_CHECKMULTISIGVERIFY` считаются как `n`, если они введены `OP_n`, или 20 sigops в противном случае;

В скриптах Taproot sigops обрабатываются иначе по сравнению с традиционными скриптами. Вместо прямого подсчета каждой операции подписи, Taproot вводит бюджет sigops для каждого входа транзакции, который пропорционален размеру этого входа. Этот бюджет составляет 50 sigops плюс размер в байтах свидетельства входа. Каждая операция подписи уменьшает этот бюджет на 50. Если выполнение операции подписи снижает бюджет ниже нуля, скрипт считается недействительным. Этот метод позволяет большую гибкость в скриптах Taproot, одновременно обеспечивая защиту от потенциальных злоупотреблений, связанных с sigops, напрямую связывая их с весом входа. Таким образом, скрипты Taproot не включены в лимит 80 000 sigops за блок.