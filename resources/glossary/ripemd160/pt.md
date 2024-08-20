---
term: RIPEMD160
---

Acrônimo para *Research and development in Advanced Communications technologies in Europe Integrity Primitives Evaluation Message Digest 160*. É uma função de hash criptográfico que gera um resumo de 160 bits a partir de uma entrada arbitrária. É usado no Bitcoin para transformar uma chave pública em um endereço de recebimento para os padrões Legacy e SegWit v0 (para SegWit v1, a chave pública não é hasheada). O processo primeiro envolve a aplicação da função de hash `SHA256` à chave pública, seguida pela aplicação de `RIPEMD160` no resultado. Esta combinação de duas funções de hash distintas é conhecida como `HASH160` no contexto do Bitcoin. `RIPEMD160` também é usado em carteiras determinísticas e hierárquicas para calcular impressões digitais de chaves. Especificamente, `HASH160` é usado para calcular a impressão digital de uma chave pai, que é então incluída nos metadados de uma chave estendida (xpub, xprv...).