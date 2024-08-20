---
term: MINING
---

参与比特币系统的工作量证明（Proof-of-Work）的行为。工作量证明是一种抵抗Sybil攻击的机制。它是中本聪共识机制的基础，该机制用于在网络的不同节点之间就分布式账本的单一版本达成一致。

具体来说，挖矿是寻找一个值，该值通过一个随机数学函数后，产生的结果低于一个目标数字。这个工作量证明的目标每2016个区块由节点调整一次，这被称为难度调整。目标数字降低以增加挖矿难度，或者提高以降低难度，这取决于矿工在前一时期部署的计算能力的演变。

![](../../dictionnaire/assets/34.png)

矿工所做的这项工作每发现一个有效区块就会得到奖励。获胜的矿工会收到金钱奖励，包括区块补贴（凭空创造新的比特币）和交易费用。今天，比特币上的工作量证明难度如此之高，以至于挖矿需要显著的计算能力才能成功赢得区块。因此，通常需要有专门的电子芯片来执行`SHA256d`，这种芯片被称为ASIC，并且参与挖矿池。