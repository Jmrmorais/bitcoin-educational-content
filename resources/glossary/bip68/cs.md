---
term: BIP68
---

Zavedl možnost použití relativních časových zámků prostřednictvím pole `nSequence`. To umožňuje transakci specifikovat relativní zpoždění, než může být zahrnuta do bloku. Toto zpoždění může být definováno v počtu bloků nebo jako násobek 512 sekund (tj. reálný čas). Poznamenejme, že tato nová interpretace pole `nSequence` je platná pouze pokud je pole `nVersion` větší nebo rovno `2`. Tato interpretace pole `nSequence` se odehrává na úrovni konsenzuálních pravidel Bitcoinu. Relativní časový zámek nastavuje zpoždění začínající od přijetí předchozí transakce, zatímco absolutní časový zámek specifikuje přesný okamžik, před kterým nemůže být transakce zahrnuta do bloku. BIP68 byl zaveden prostřednictvím měkkého forku 4. července 2016 společně s BIP112 a BIP113, aktivován poprvé použitím metody BIP9.