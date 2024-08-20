---
term: ASSUME UTXO
---

ASSUME UTXO是比特币核心客户端中的一个配置参数，它允许刚刚初始化（但尚未经历IBD）的节点推迟交易和UTXO集的验证，直到给定的快照。这个概念依赖于使用由Core提供并假定为准确的UTXO集（在给定时间内所有现存UTXO的列表），这允许节点非常快速地与累积工作量最多的链同步。由于节点跳过了漫长的IBD步骤，它可以很快为用户运行。ASSUME UTXO将同步（IBD）分为两部分：
* 首先，节点执行Header First Sync（仅验证头部）并认为Core提供的UTXO集有效；
* 然后，一旦它开始运行，节点将在后台验证完整的区块历史，更新它自己验证的新UTXO集。如果这个新的UTXO集与Core提供的不匹配，它将产生一个错误消息。

因此，ASSUME UTXO通过推迟交易验证过程和通过Core提供的更新快照的UTXO集，加速了新比特币节点的准备工作。