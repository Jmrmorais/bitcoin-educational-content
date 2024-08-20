---
término: BIP12
---

Propuesta de Gavin Andresen para mejorar la flexibilidad y privacidad de los scripts de transacción de Bitcoin. Este BIP sugiere implementar un nuevo opcode de script, denominado `OP_EVAL`, que permite la evaluación de un script contenido dentro de los datos de un `scriptSig` durante el proceso de validación de la transacción. La principal modificación de BIP12 es permitir la inclusión de un script dentro de otro script. Esta técnica posibilita la creación de condiciones más complejas que pueden ser verificadas en el momento del gasto, sin necesidad de revelarlas a los usuarios que envían bitcoins a la dirección utilizada. BIP12 fue posteriormente reemplazado por propuestas más seguras, notablemente BIP16 (P2SH), que ofrece un método diferente para alcanzar los mismos objetivos que `OP_EVAL`.