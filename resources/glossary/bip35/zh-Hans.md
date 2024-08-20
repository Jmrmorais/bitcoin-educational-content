---
term: BIP35
---

提案允许比特币节点打开其内存池（mempool）的信息，即等待确认的交易。因此，其他参与者可以通过向节点发送特定消息来实时接收未确认交易的数据。在采用BIP35之前，节点只能访问已确认交易的信息。这一改进为SPV钱包提供了接收未确认交易信息的能力，允许矿工在重启期间避免错过高费用的交易，并便于外部服务分析内存池信息。