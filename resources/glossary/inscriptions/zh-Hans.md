---
term: 铭文
---

在Ordinals理论的背景下，铭文是刻在sats上的任意内容，将它们转变为原生比特币数字艺术品。铭文是通过交易制作的，这种交易在Taproot输入的脚本中暴露信息内容，方式如下：

```text
OP_0
OP_IF
<这里是数据>
OP_ENDIF
```

这些数字艺术品，如同NFTs，可以被交易和保留。