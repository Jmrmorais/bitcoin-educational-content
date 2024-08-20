---
term: 目标
---

在确定性和分层（HD）钱包中，由BIP43定义的目标（或在英语中的_目的_），代表了特定级别的派生。这个索引位于派生树的第一层深度（`m / purpose' /`），用于识别钱包采用的派生标准，以便于不同的钱包管理软件之间的兼容性。例如，在SegWit地址（BIP84）的情况下，目标被记作`/84'/`。这种方法允许在同一个HD钱包中高效地组织不同类型地址的密钥。使用的标准索引包括：
* 对于P2PKH：`44'`;
* 对于P2WPKH嵌套在P2SH中：`49'`;
* 对于P2WPKH：`84'`;
* 对于P2TR：`86'`。

![](../../dictionnaire/assets/20.png)