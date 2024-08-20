---
term: TIMELOCK
---

智能合约的一种基本功能，允许设置一个基于时间的条件，该条件必须满足才能将交易添加到区块中。在比特币上有两种类型的时间锁：
* 绝对时间锁，指定一个确切的时刻，在此之前交易不能被包含在区块中；
* 相对时间锁，从接受前一个交易开始设置一个延迟。
时间锁可以定义为以Unix时间表示的日期，或者作为区块号。最后，时间锁可以通过在锁定脚本中使用特定的操作码（`OP_CHECKLOCKTIMEVERIFY` 或 `OP_CHECKSEQUENCEVERIFY`）应用于交易输出，或者通过使用特定的交易字段（`nLockTime` 或 `nSequence`）应用于整个交易。