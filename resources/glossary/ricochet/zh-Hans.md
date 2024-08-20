---
term: RICOCHET
---

一种技术，涉及对自己进行多次假交易，以模拟比特币所有权的转移。Ricochet用于模糊可能妨碍比特币硬币可替代性的具体细节。例如，如果你执行一个coinjoin，你的输出硬币将被识别为此类硬币。这种“_来自coinjoin的硬币_”的标签可能会影响UTXO的可替代性。受监管的实体，如交易平台，可能拒绝接受经过coinjoin的UTXO，甚至要求其所有者解释，冒着账户被封锁或资金被冻结的风险。在某些情况下，平台甚至可能向国家机关报告您的行为。这就是Ricochet方法发挥作用的地方。为了模糊coinjoin留下的痕迹，Ricochet执行四次连续交易，用户将其资金转移到不同的地址上。在这一系列交易之后，Ricochet工具最终将比特币路由到其最终目的地，如交易平台。目标是在原始coinjoin交易和最终支出行为之间创造距离。这样，链分析工具很可能会假设在coinjoin之后已经发生了所有权转移，因此没有必要对发行者采取行动。Ricochet最常见的用例发生在需要隐藏UTXO上先前参与coinjoin的情况，特别是为了避免成为受监管平台或黑名单AML/CTF政策的目标。Ricochet工具可在Samourai Wallet上使用。