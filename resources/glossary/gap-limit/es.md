---
term: GAP LIMIT
---

Un parámetro utilizado en el software de monederos de Bitcoin para determinar el número máximo de direcciones consecutivas sin usar que se generarán antes de detener la búsqueda de transacciones adicionales. Ajustar este parámetro es a menudo necesario cuando se recupera un monedero para asegurar que se encuentren todas las transacciones. Un Límite de Brecha insuficiente podría resultar en la pérdida de algunas transacciones si las direcciones se omitieron durante las fases de derivación. Aumentar el Límite de Brecha permite al monedero buscar más adelante en la secuencia de direcciones, con el fin de recuperar todas las transacciones asociadas.

De hecho, un único `xpub` puede derivar teóricamente más de 4 mil millones de direcciones de recepción (tanto direcciones internas como externas). Sin embargo, el software del monedero no puede derivar y verificar todas ellas para su uso sin incurrir en un enorme costo operacional. Por lo tanto, proceden en orden de índice, ya que este es normalmente el orden en el que todo el software de monederos genera direcciones. El software registra cada dirección utilizada antes de pasar a la siguiente, y detiene su búsqueda cuando encuentra un número de direcciones vacías consecutivamente. Este número es lo que se llama el Límite de Brecha.

Si, por ejemplo, el Límite de Brecha se establece en `20`, y la dirección `m/84'/0'/0'/0/15/` está vacía, el monedero derivará direcciones hasta `m/84'/0'/0'/0/34/`. Si este rango de direcciones permanece sin usar, la búsqueda se detiene allí. Por consiguiente, una transacción que utilice la dirección `m/84'/0'/0'/0/40/` no sería detectada en este ejemplo.