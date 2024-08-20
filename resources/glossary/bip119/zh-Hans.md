---
term: BIP119
---

引入了一个名为`OP_CHECKTEMPLATEVERIFY`（CTV）的新操作码。CTV将允许在交易中创建非递归契约，以便对给定硬币的使用方式施加特定条件，包括在未来的交易中。更具体地说，它将使基于作为输入花费的UTXO的`scriptPubKey`，对交易输出的`scriptPubKey`定义条件成为可能。CheckTemplateVerify旨在保持简单并且没有动态状态。其实现目标是扩展比特币的脚本功能，以便于各种应用，如交易拥堵控制、创建非交互式支付通道、DLCs、支付池等...这个新操作码将作为`OP_NOP4`的替代品引入。这一变化将意味着一个软分叉。