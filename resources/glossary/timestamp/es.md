---
term: TIMESTAMP
---

El sellado de tiempo, o "timestamp" en inglés, es un mecanismo que implica asociar un marcador temporal preciso con un evento, dato o mensaje. En el contexto general de los sistemas informáticos, el sellado de tiempo se utiliza para determinar el orden cronológico de las operaciones y para verificar la integridad de los datos a lo largo del tiempo.

En el caso específico de Bitcoin, los timestamps se utilizan para establecer la cronología de las transacciones y bloques. Cada bloque en la cadena de bloques contiene un timestamp que indica el momento aproximado de su creación. Satoshi Nakamoto incluso habla de un "servidor de timestamp" en su White Paper, para describir lo que hoy llamaríamos la "blockchain". El papel del sellado de tiempo en Bitcoin es determinar la cronología de las transacciones, con el fin de determinar, sin la intervención de una autoridad central, qué transacción ocurrió primero. Este mecanismo permite a cada usuario verificar la no existencia de una transacción en el pasado, y así prevenir que un usuario malicioso realice un doble gasto. Este mecanismo es justificado por Satoshi Nakamoto en su White Paper con la famosa frase: "*La única manera de confirmar la ausencia de una transacción es estar al tanto de todas las transacciones.*" Este estándar se establece sobre el tiempo Unix, que representa los segundos totales transcurridos desde el 1 de enero de 1970.

> ► *El sellado de tiempo de los bloques en Bitcoin es relativamente flexible, ya que para que un timestamp sea considerado válido, simplemente necesita ser mayor que la mediana del tiempo de los 11 bloques precedentes (MTP) y menor que la mediana de los tiempos devueltos por los nodos (tiempo ajustado por la red) más 2 horas.*