---
term: RIPEMD160
---

缩写代表*在欧洲高级通信技术研发中的完整性原语评估消息摘要160*。它是一种加密哈希函数，能够从任意输入生成一个160位的摘要。在比特币中，它用于将公钥转换为接收地址，适用于传统和SegWit v0标准（对于SegWit v1，公钥不进行哈希处理）。该过程首先涉及对公钥应用`SHA256`哈希函数，然后对结果应用`RIPEMD160`。这种两个不同哈希函数的组合在比特币的上下文中被称为`HASH160`。`RIPEMD160`还用于确定性和分层钱包中计算密钥指纹。具体来说，`HASH160`用于计算父密钥的指纹，然后将其包含在扩展密钥（xpub, xprv等）的元数据中。