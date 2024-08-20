---
term: BIP43
---

改进提案，引入了使用派生路径级别来描述HD钱包结构中的目的字段，该概念之前在BIP32中被引入。根据BIP43，HD钱包的第一级派生，紧接主密钥表示为`m/`之后，是为目的编号保留的，该编号指示了余下路径使用的派生标准。这个编号被记录为一个加固索引。例如，如果钱包遵循SegWit标准（BIP84），其派生路径的开始将是：`m/84'/`。因此，BIP43允许澄清每个钱包软件所遵循的标准，以便它们之间有更好的互操作性。余下的派生路径的标准化在BIP44中有所描述。