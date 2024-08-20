---
term: BIP173
---

引入了用于SegWit V0地址的bech32地址格式。这种地址格式的特点是前缀`bc1q`。bech32格式提供了几个优点：
* 它在QR码中占用的空间更少；
* 它更容易被人类解读；
* 它拥有一种创新的校验和机制，这种机制更高效，并且允许检测和潜在的自动更正输入错误。
这些特性使得接收地址的使用变得更加容易，同时最小化了错误的风险。