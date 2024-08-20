---
term: MULTISIG
---

多重签名钱包，通常简称为“multisig”，旨在通过要求多个不同私钥的签名来授权支出，从而增强比特币的安全性。这种方法将风险分散到几个密钥中，有助于降低丢失和盗窃的风险（取决于multisig配置）。Multisig钱包采用“m-of-n”模型，其中`m`代表验证交易所需的最小签名数量，`n`是涉及的密钥总数。例如，2-of-3设置要求三个可能的签名中的两个来验证交易。与单密钥钱包相比，这种方法提供了更高的安全性，但它也在管理和备份方面引入了更多的复杂性。此外，使用较旧的multisig标准的交易比传统的singlesig交易在隐私性和费用上更为不利。然而，最近的创新，如Taproot和描述符的使用，预计将最小化，如果不是消除，multisigs的这些缺点。

> ► *一些比特币用户在“Multisig”和“Threshold Multisig”这两个术语之间做出区分。确实，一些人认为multisig必然是n-of-n，而threshold multisig是m-of-n。然而，在通用语言中，即使对于m-of-n也接受使用“Multisig”这一术语。*