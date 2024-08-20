---
term: BIP47
---

由Justus Ranvier在2015年提出，这一协议旨在解决比特币地址重用的关键问题，这一做法严重威胁了系统上用户的隐私。比特币白皮书中的中本聪已经强调了每次交易使用不同密钥对以维持用户不同操作间隔离的重要性。BIP47引入了可重用支付代码的概念，允许用户接收多次支付而无需为每笔交易手动生成一个新的比特币地址。这些代码作为虚拟标识符，派生自用户的钱包种子，并位于HD钱包的派生结构的账户级别。通过双方支付代码的组合，每一方都能派生出属于另一方的大量唯一地址，无需再次与对方通信。这一协议的核心依赖于ECDH算法（*椭圆曲线Diffie-Hellman*），这是建立在椭圆曲线上的Diffie-Hellman密钥交换的变体，它允许双方建立一个共享的秘密，用于生成唯一的接收地址。尽管BIP47尚未被添加到比特币核心，并且从社区收到了褒贬不一的反馈，但像Samourai Wallet和Sparrow Wallet这样的实现已经采纳并完全集成到它们的隐私工具生态系统中。