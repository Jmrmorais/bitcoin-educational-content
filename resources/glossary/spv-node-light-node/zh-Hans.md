---
term: SPV节点（轻节点）
---

SPV（*简单支付验证*）节点，有时被称为“轻节点”，是比特币节点的一种轻量级客户端，它允许用户在不需要存储整个区块链的情况下验证交易。SPV节点仅存储区块头信息，并在必要时通过查询全节点来获取特定交易的信息。这种验证原理得益于比特币区块中交易的结构，这些交易在一个加密累加器（默克尔树）内被组织起来。

这种方法对于资源有限的设备（如手机）来说是有利的。然而，SPV节点依赖于全节点来获取信息，这意味着需要额外的信任级别，因此，与全节点相比，安全性较低。SPV节点不能自主验证交易，但它们可以通过查询默克尔证明来验证交易是否被包含在一个区块中。