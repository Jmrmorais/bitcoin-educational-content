---
term: OP_ENDIF (0X68)
---

标记由`OP_IF`或`OP_NOTIF`启动的条件控制结构的结束，通常后面会跟随一个或多个`OP_ELSE`。它表示脚本的执行应该继续超出条件结构，无论执行了哪个分支。换句话说，`OP_ENDIF`用于划定脚本中条件块的结束。