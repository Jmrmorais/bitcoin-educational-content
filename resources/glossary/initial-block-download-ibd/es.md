---
term: INITIAL BLOCK DOWNLOAD (IBD)
---

Se refiere al proceso mediante el cual un nodo descarga y verifica la blockchain desde el bloque Génesis, y se sincroniza con otros nodos en la red de Bitcoin. El IBD debe llevarse a cabo al lanzar un nuevo nodo completo. Al comienzo de esta sincronización inicial, el nodo no tiene información sobre transacciones anteriores. Por lo tanto, descarga cada bloque de otros nodos en la red, verifica su validez y luego lo agrega a su versión local de la blockchain. Cabe destacar que el IBD puede ser largo e intensivo en recursos debido al creciente tamaño de la blockchain y el conjunto de UTXO. La velocidad de su ejecución depende de las capacidades de computación del ordenador que aloja el nodo, su capacidad de RAM, la velocidad del dispositivo de almacenamiento y el ancho de banda. Para darte una idea, si tienes una conexión a internet potente, y el nodo está alojado en el último MacBook con mucha RAM, el IBD solo tomará unas pocas horas. Por el contrario, si usas un microordenador como una Raspberry Pi, el IBD podría tardar una semana o más.

> ► *En francés, generalmente se acepta referirse directamente a un IBD. La traducción que a veces se utiliza es "synchronisation initiale", o "téléchargement initial des blocs".*