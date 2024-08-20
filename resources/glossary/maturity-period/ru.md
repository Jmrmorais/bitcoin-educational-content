---
term: СРОК ЗРЕЛОСТИ
---

Необходимая задержка перед тем, как вознаграждение за блок может быть потрачено майнером, который его получил. Этот период установлен на 100 блоков после добытого блока, что равно 101 подтверждению для транзакции coinbase. В течение этого времени вновь созданные биткойны в вознаграждении за блок не могут быть потрачены. Цель этого правила - избежать сложностей, связанных с использованием биткойнов из цепочки, которая позже может быть признана устаревшей. Действительно, случается, что действительные блоки в конечном итоге аннулируются, если другой блок на той же высоте включается в цепочку, над которой было выполнено больше работы. Это явление, известное как реорганизация, приводит к созданию "сиротского блока" или "устаревшего блока", тем самым лишая майнера биткойнов, содержащихся в coinbase отброшенного блока. Если бы вновь созданные биткойны сразу были доступны для расходования, любая транзакция с их участием могла бы быть отменена ретроспективно, вызывая убытки для держателей этих биткойнов. Такой сценарий мог бы привести к каскаду отмен иначе действительных транзакций, тем самым затрагивая всех пользователей, участвующих в этой цепочке транзакций. Таким образом, срок зрелости является предохранительным механизмом против этого риска. Устанавливая задержку в 100 блоков перед тем, как вновь выпущенные биткойны могут быть использованы, это предотвращает циркуляцию монет из блоков, которые в конечном итоге аннулируются, и влияние на другие транзакции. Вероятность реорганизации за 101 блок настолько низка, что считается пренебрежимо малой.