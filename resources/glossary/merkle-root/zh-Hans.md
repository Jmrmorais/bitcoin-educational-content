---
term: 默克尔根
---

默克尔根是默克尔树的摘要或“顶部哈希”，代表了树中所有信息的总结。默克尔树是一种加密累加器结构，有时也被称为“哈希树”。在比特币的上下文中，默克尔树被用来组织一个区块内的交易，并且便于快速验证特定交易的包含情况。因此，在比特币区块中，通过成对地连续哈希交易直到只剩下一个哈希（即默克尔根）来获得默克尔根。然后，这个哈希被包含在相应区块的头部。这种哈希树也出现在UTREEXO中，这是一种允许压缩节点的UTXO集的结构，以及在MAST Taproot中。