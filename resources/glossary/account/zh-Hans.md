---
term: 账户
---

在HD（分层确定性）钱包中，账户代表了根据BIP32在深度3的派生层。每个账户都从`/0'/`（强化派生，实际上是`/2^31/`或`/2 147 483 648/`）开始顺序编号。正是在这个派生深度，众所周知的`xpubs`位于。如今，通常在一个HD钱包中只使用一个账户。然而，最初，它们被设计为在同一个钱包内隔离不同类别的使用。例如，如果我们取一个外部Taproot（P2TR）接收地址的标准派生路径：`m/86'/0'/0'/0/0`，账户索引是第二个`/0'/`。

![](../../dictionnaire/assets/17.png)