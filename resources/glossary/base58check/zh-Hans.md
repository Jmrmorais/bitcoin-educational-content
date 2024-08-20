---
term: BASE58CHECK
---

`Base58Check`是比特币系统中使用的一种编码，用于以人类可读的字符字符串形式表示传统接收地址和某些其他数据，如扩展密钥。它是`Base58`系统的一个变种，`Base58`是一种基于58的位置表示法，旨在最小化人为的抄写错误。它使用一组58个字母数字字符，包括从`1`到`9`的数字，从`A`到`Z`的大写字母（排除了字母`I`和`O`以避免与数字`1`和`0`混淆），以及从`a`到`z`的小写字母（排除了字母`l`以避免与数字`1`混淆）。`Base58Check`与`Base58`的不同之处在于增加了校验和。它通过在`Base58`编码的数据末尾添加一个简化版的双重`SHA256`哈希（`SHA256d`或`HASH256`）来表示。在验证时，会重新计算校验和并与编码过程中添加的校验和进行比较。如果两个哈希匹配，则认为数据有效；否则，会报告损坏或抄写错误。

`Base58Check`在比特币地址和密钥中的使用具有几个优点。首先，它通过避免含糊不清的字符，减少了抄写和阅读中的人为错误。其次，它通过通过校验和检测和报告错误来防止打字错误。第三，`Base58Check`中数据的紧凑表示减少了存储和分享地址及密钥所需的空间。最新的接收地址（SegWit之后）已经放弃了`Base58Check`编码，转而使用具有更高级校验和（使用BCH码）的`Bech32`和`Bech32m`编码。