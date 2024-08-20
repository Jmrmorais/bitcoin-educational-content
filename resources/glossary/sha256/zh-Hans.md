---
term: SHA256
---

缩写代表“*安全哈希算法 256 位*”。它是一种产生 256 位摘要的加密哈希函数。由*国家安全局*（NSA）在 2000 年代初设计，它已成为处理敏感数据的联邦标准。在比特币协议中，`SHA256` 函数无处不在。它用于作为工作证明的一部分对区块头进行哈希处理。`SHA256` 也用于从公钥派生接收地址的过程中。此外，它还用于区块中的交易和见证人在默克尔树内的聚合。`SHA256` 也用于密钥指纹的计算、某些校验和的计算以及围绕比特币的许多其他过程中。当连续两次应用时，它被称为 `HASH256`。这种双重应用是比特币上主要使用的一种。当 `SHA256` 与 `RIPEMD160` 函数结合使用时，它被称为 `HASH160`。这种双重哈希用于密钥指纹和哈希公钥。`SHA256` 函数是 SHA 2 家族的一部分。