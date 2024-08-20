---
term: OP_CHECKMULTISIG (0XAE)
---

检查多个签名是否与多个公钥匹配。它输入一系列的`N`个公钥和`M`个签名，其中`M`可以小于或等于`N`。`OP_CHECKMULTISIG`验证是否至少有`M`个签名与`N`个公钥中的`M`个匹配。注意，由于一个历史上的偏差错误，`OP_CHECKMULTISIG`会从堆栈中移除一个额外的元素。这个元素被称为“*虚拟元素*”。为了避免在`scriptSig`中出现错误，因此包含了一个`OP_0`，这是一个无用的元素，用以满足移除操作并绕过该错误。自从BIP147（2017年与SegWit一同引入）以来，由于该错误而消耗的无用元素必须是`OP_0`，以使脚本有效，因为它是一个可变性向量。这个操作码在Tapscript中被移除。