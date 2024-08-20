---
term: 压缩公钥
---

公钥在脚本中使用（直接以公钥形式或作为地址），用于接收和保护比特币。原始公钥由椭圆曲线上的一个点表示，包含两个坐标（`x, y`），每个坐标256位。在原始格式中，公钥因此为512位，不包括用于识别格式的额外字节。另一方面，压缩公钥是一种更紧凑的公钥表示形式。它仅使用`x`坐标和一个前缀（`02`或`03`），该前缀指示`y`坐标的奇偶性（偶数或奇数）。

如果我们将其简化到实数领域，鉴于椭圆曲线相对于x轴是对称的，对于曲线上的任何点$P$（`x, y`），存在另一个点$P'$（`x, -y`）也将位于同一曲线上。这意味着对于每个`x`，`y`只有两个可能的值，正数和负数。例如，对于给定的横坐标`x`，在椭圆曲线上会有两个点$P1$和$P2$，它们有相同的横坐标但纵坐标相反：

![](../../dictionnaire/assets/29.png)
为了在曲线上的两个潜在点之间进行选择，会添加一个指定选择哪个`y`的前缀到`x`上。这种方法允许将公钥的大小从520位减少到仅264位（前缀8位 + `x`的256位）。这种表示形式被称为公钥的压缩形式。

然而，在椭圆曲线密码学的上下文中，我们使用的不是实数，而是阶为`p`（一个质数）的有限域。在这种情况下，`y`的“符号”由其奇偶性决定，即`y`是偶数还是奇数。前缀`0x02`则表示偶数`y`，而`0x03`表示奇数`y`。

考虑以下椭圆曲线上的原始公钥（一个点）的十六进制示例：
```plaintext
K = 04678afdb0fe5548271967f1a67130b7105cd6a828e03909a67962e0ea1f61deb649f
6bc3f4cef38c4f35504e51ec112de5c384df7ba0b8d578a4c702b6bf11d5f
```

我们可以分离前缀、`x`和`y`：
```plaintext
前缀 = 04
为了确定`y`的奇偶性，我们检查`y`的最后一个十六进制字符：
```plaintext
十六进制（Base 16）: f
十进制（Base 10）: 15
y是奇数
```

压缩公钥的前缀将是`03`。压缩公钥的十六进制形式变为：
```plaintext
K = 03678afdb0fe5548271967f1a67130b7105cd6a828e03909a67962e0ea1f61deb6
```