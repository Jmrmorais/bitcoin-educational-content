---
term: BIP42
---

Návrh na vylepšení Bitcoin Core, který řeší menší chybu v plánu snižování odměn za blok. Tato anomálie, pokud by nebyla opravena, by vedla k celkovému vytvoření bitcoinů přesahujícímu plánovaný limit 21 milionů. Konkrétně, po skončení halvingů by teoreticky mohl být spuštěn nový cyklus tvorby bitcoinů kolem roku 2214. Kód Core v otázce používal operaci binárního posunu vpravo na hodnotě odměny pro těžaře. Chyba pramenila z použití této operace posunu v kontextu, kde bylo chování podle standardů jazyka C++ nedefinované. Posunutí 64bitového celého čísla (`int64_t`) o více než 63 bitů doprava spadá do této kategorie nedefinovaného chování. V kódu Bitcoin Core by se to mohlo stát po 64 halvingech, na výšce bloku č. 13,440,000. Za touto hranicí nebylo chování bitového posunu definováno, což znamená, že různé kompilace by mohly kód interpretovat různě. To by mohlo vést k nepředvídatelným výsledkům, včetně možnosti vytvoření nekonečné inflace bitcoinů. BIP42 tento problém opravil tím, že požadoval, aby odměna za blok byla po 64 halvingech nastavena na nulu, čímž se vyhnul použití operace posunu vpravo v kontextu nedefinovaného chování. Tato úprava, která byla soft forkem, tedy objasnila chování kódu Bitcoin Core. Ačkoli byla tato chyba opravená BIP42 poměrně vážná, nebyla okamžitě kritická, protože by se neprojevila až do roku 2214. Publikováno 1. dubna 2014 Pieterem Wuille, BIP42 je tak vyznamenán svým humorným tónem.