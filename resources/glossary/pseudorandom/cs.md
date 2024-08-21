---
term: PSEUDO-NÁHODNÝ
---

Tento přídavný jméno se používá k popisu sekvence čísel, která, ačkoliv je výsledkem deterministického procesu, vykazuje vlastnosti blízké ideální skutečně náhodné sekvenci. Koncept ideální náhodnosti zahrnuje úplnou absenci předvídatelnosti a korelace mezi po sobě jdoucími prvky. Pseudo-náhodné číslo je generováno deterministickým algoritmem a teoreticky je tedy zcela předvídatelné, pokud známe počáteční stav generátoru.

Generátor pseudo-náhodných čísel (PRNG) je algoritmus používaný k produkci takových čísel. Obvykle začíná od počáteční hodnoty, nebo "semenu", a poté aplikuje sérii matematických transformací k vytvoření sekvence čísel. Kvůli této determinovatelnosti je důležité pro kryptografickou bezpečnost, aby počáteční semeno zůstalo tajné. Pseudo-náhodné sekvence se široce používají v různých oblastech, včetně kryptografie, protože vykazují zdánlivě náhodné chování, které postačuje pro mnoho aplikací. Hodnocení kvality PRNG je založeno na míře, do které se jeho výstup blíží skutečné náhodnosti z hlediska distribuce, korelací a dalších statistických vlastností. V kontextu Bitcoinu se pseudo-náhodná čísla používají k vytvoření soukromých klíčů nebo k generování semene pro deterministické a hierarchické peněženky.