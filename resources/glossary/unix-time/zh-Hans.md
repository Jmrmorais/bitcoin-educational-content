---
术语：UNIX 时间
---

Unix 时间或 Unix 时间戳表示自1970年1月1日午夜UTC（Unix 纪元）以来已经过去的秒数。这一系统在Unix操作系统及其衍生系统中被用来以一种通用和标准化的方式标记时间。它使得时钟同步和基于时间的事件管理成为可能，无论时区如何。

在比特币的上下文中，它被用于节点的本地时钟，因此用于NAT（网络调整时间）的计算。网络调整时间是每个节点本地计算的节点时间的中位数，然后这个参考被用来验证区块时间戳的有效性。实际上，要使一个节点接受一个区块，其时间戳必须在MTP（最后11个挖掘区块的过去中位时间）和NAT加2小时之间：

```text
MTP < 有效时间戳 < (NAT + 2h)
```

Unix 时间也被用来建立基于实际时间的时间锁，而不是基于区块数量。