---
term: OP_CHECKMULTISIG (0XAE)
---

Verifica múltiples firmas contra múltiples claves públicas. Toma como entrada una serie de `N` claves públicas y `M` firmas, donde `M` puede ser menor o igual a `N`. `OP_CHECKMULTISIG` verifica si al menos `M` firmas coinciden con `M` de las `N` claves públicas. Cabe destacar que debido a un error histórico de desfase por uno, un elemento adicional es eliminado por `OP_CHECKMULTISIG` de la pila. Este elemento se denomina "*elemento ficticio*". Para evitar un error en el `scriptSig`, se incluye un `OP_0`, que es un elemento inútil, para satisfacer la eliminación y sortear el error. Desde BIP147 (introducido con SegWit en 2017), el elemento inútil consumido debido al error debe ser `OP_0` para que el script sea válido, ya que era un vector de maleabilidad. Este opcode fue eliminado en Tapscript.