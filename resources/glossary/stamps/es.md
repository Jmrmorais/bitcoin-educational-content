---
term: STAMPS
---

Un protocolo que permite la integración de datos de imagen formateados directamente en la blockchain de Bitcoin a través de transacciones multisignatura en bruto (P2MS). Stamps codifica el contenido binario de una imagen en base 64 y lo añade a las claves de un P2MS de 1/3. Una clave es real y se utiliza para gastar los fondos, mientras que las otras dos son claves ficticias (la clave privada asociada es desconocida) que almacenan los datos. Al codificar los datos directamente como claves públicas en lugar de usar salidas `OP_RETURN`, las imágenes almacenadas con el protocolo Stamps son particularmente intensivas en términos de carga de trabajo para los nodos. Este método crea notablemente múltiples UTXOs, lo que aumenta el tamaño del conjunto de UTXOs y plantea problemas para los nodos completos.