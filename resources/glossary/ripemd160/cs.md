---
term: RIPEMD160
---

Akronym pro *Research and development in Advanced Communications technologies in Europe Integrity Primitives Evaluation Message Digest 160*. Jedná se o kryptografickou hašovací funkci, která generuje 160bitový souhrn z libovolného vstupu. Používá se v Bitcoinu pro transformaci veřejného klíče na přijímací adresu pro standardy Legacy a SegWit v0 (pro SegWit v1 není veřejný klíč hašován). Proces nejprve zahrnuje aplikaci hašovací funkce `SHA256` na veřejný klíč, následovanou aplikací `RIPEMD160` na výsledek. Tato kombinace dvou odlišných hašovacích funkcí je v kontextu Bitcoinu známá jako `HASH160`. `RIPEMD160` se také používá v deterministických a hierarchických peněženkách pro výpočet otisků klíčů. Konkrétně se `HASH160` používá pro výpočet otisku rodičovského klíče, který je poté zahrnut do metadat rozšířeného klíče (xpub, xprv...).