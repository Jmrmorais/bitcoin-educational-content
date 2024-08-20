---
术语：BIP
---

缩写代表“比特币改进提案”（Bitcoin Improvement Proposal）。比特币改进提案（BIP）是一个正式的流程，用于提议和记录对比特币协议及其标准的改进和变更。由于比特币没有中央实体来决定更新，BIP允许社区以结构化和透明的方式提出、讨论和实施改进。每个BIP详细说明了拟议改进的目标、理由、对兼容性的潜在影响，以及优点和缺点。BIP可以由社区的任何成员编写，但必须得到其他开发者和维护比特币核心GitHub数据库的编辑的批准：Bryan Bishop、Jon Atack、Luke Dashjr、Mark Erhardt（Murch）、Olaoluwa Osuntokun和Ruben Somsen。然而，重要的是要理解，这些个人在编辑BIP中的角色并不意味着他们控制比特币。如果有人提出一个在正式BIP框架内未被接受的改进，他们仍然可以直接向比特币社区提出，甚至创建一个包含他们的修改的分支。BIP流程的优势在于其正式性和集中性，有助于避免比特币用户之间的分歧，寻求以共识的方式实施更新。最终，经济多数原则决定了协议内的权力动态。

BIP分为三个主要类别：
* *标准轨道BIP*：涉及直接影响比特币实现的修改，如交易和区块验证规则；
* *信息性BIP*：提供信息或建议，而不提议直接更改协议；
* *流程BIP*：描述围绕比特币的程序变更，如治理流程。

标准轨道和信息性BIP还按“层”分类：
* *共识层*：此层的BIP涉及比特币的共识规则，如对区块或交易验证规则的修改。这些提案可以是软分叉（向后兼容的修改）或硬分叉（非向后兼容的修改）。例如，SegWit和Taproot的BIP属于此类别；
* *对等服务*：此层涉及比特币节点网络的运作，即节点如何在互联网上找到并与彼此通信。
* *API/RPC*：此层的BIP涉及应用程序编程接口（API）和远程过程调用（RPC），允许比特币软件与节点交互；
* *应用层*：此层涉及构建在比特币之上的应用程序。此类别中的BIP通常处理比特币钱包标准的修改级别。

提交BIP的过程从在*Bitcoin-dev*邮件列表上概念化和讨论想法开始。如果这个想法有前景，作者会按照特定格式起草一个BIP，并通过Pull Request提交到核心GitHub仓库。编辑会审查这个提案，以验证它是否满足所有标准。BIP必须技术上可行，对协议有益，符合所需的格式，并且符合比特币的哲学。如果BIP满足这些条件，它就会正式整合到BIP的GitHub仓库中。然后它会被分配一个编号。这个编号通常由编辑决定，经常是Luke Dashjr，并且是逻辑分配的：处理类似主题的BIP通常会收到连续的编号。

BIP在其生命周期中会经历不同的状态。每个BIP的头部都会指定当前状态：
* 草案：提案仍处于起草和讨论阶段；
* 提议：BIP被认为是完整的，并准备好由社区审查；
* 延期：BIP被提案人或编辑暂时搁置；
* 拒绝：如果BIP 3年内没有任何活动，就被分类为拒绝。其作者可以选择稍后恢复它，这将允许它返回到草案状态；
* 撤回：BIP已由其作者撤回；
* 最终：BIP被接受并在比特币上广泛实施；
* 活跃：仅对于流程BIP，一旦达成某种共识，就会分配此状态；
* 替换/过时：BIP不再适用或已被更近期的提案替换，使其变得不必要。

![](../../dictionnaire/assets/25.png)

> ► *BIP是“Bitcoin Improvement Proposal”的缩写。在法语中，它可以被翻译为“Proposition d'amélioration de Bitcoin”。然而，大多数法语文本直接使用缩写“BIP”作为一个通用名词，有时是女性，有时是男性。*