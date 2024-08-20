---
term: 标准化规则
---

标准化规则是每个比特币节点单独采用的，除了共识规则外，还用来定义它接受进入其内存池并广播给其节点伙伴的未确认交易的结构。因此，这些规则由每个节点在本地配置和执行，可能会从一个节点到另一个节点有所不同。它们仅适用于未确认的交易。因此，一个节点只有在交易已经包含在一个有效的区块中时，才会接受它认为的非标准交易。

值得注意的是，大多数节点保留了在比特币核心中建立的默认配置，从而在网络中创建了标准化规则的一致性。一个虽然符合共识规则，但不遵守这些标准化规则的交易，在网络中的广播将会遇到困难。然而，如果这种交易到达了矿工，它仍然可以被包含在一个有效的区块中。实际上，这些被称为“非标准”的交易，通常通过比特币点对点网络之外的外部方式直接传输给矿工。这通常是确认这类交易的唯一方式。

例如，一个不分配手续费的交易，根据共识规则是有效的，同时也是非标准的，因为比特币核心的默认策略对于`minRelayTxFee`参数是`0.00001`（以BTC/kB计）。

> ► *“内存池规则”这个术语有时也用来指代标准化规则。*