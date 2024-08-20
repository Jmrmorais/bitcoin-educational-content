---
term: 成熟期
---

在矿工接收到区块奖励之后，必须经过一段延迟时间才能花费这些奖励。这个期限被设定为在挖出区块后的100个区块，相当于coinbase交易的101次确认。在此期间，区块奖励中新创建的比特币是无法被花费的。这条规则的目的是为了避免使用可能稍后会被废弃的链上的比特币所导致的复杂问题。实际上，如果另一个区块（在相同高度）被并入一个完成工作量更多的链中，那么有效的区块最终可能会被废弃。这种现象，被称为重组，导致产生了一个“孤块”或“陈旧块”，从而使矿工失去了被遗弃的区块coinbase中包含的比特币。如果新创建的比特币立即可以被花费，那么涉及它们的任何交易都可能被追溯取消，给这些比特币的持有者造成损失。这种情况可能导致一连串本来有效的交易被取消，从而影响到那个交易链中所有涉及的用户。因此，成熟期是一种预防这种风险的机制。通过在新发行的比特币可以使用之前强加100个区块的延迟，它阻止了最终被废弃的区块中的币流通并影响其他交易。在101个区块上发生重组的概率是如此之低，以至于被认为是可以忽略不计的。