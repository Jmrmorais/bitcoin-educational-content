---
term: KANDIDÁTNÍ BLOK
---

Kandidátní blok je blok, který je ve fázi vytváření těžařem účastnícím se procesu těžby v systému Bitcoin. Kandidátní blok je dočasná datová struktura obsahující transakce čekající na potvrzení, ale ještě nemá platný důkaz práce (proof-of-work) pro přidání do blockchainu. Těžař vybírá transakce, které zahrne do kandidátního bloku, na základě různých faktorů, jako jsou přidružené transakční poplatky a omezení velikosti bloku. Jakmile jsou transakce vybrány, těžař generuje hlavičku bloku, která zahrnuje verzi, souhrn transakcí (Merkle root), časové razítko, hash předchozího bloku, cílovou obtížnost a nonce. Těžař poté pokouší najít hash své hlavičky, který odpovídá aktuální cílové obtížnosti. K tomu těžař upravuje nonce přítomné v hlavičce. Těžař může také upravovat jiné informace přítomné v jeho kandidátním bloku. To je mechanismus důkazu práce. Pokud těžař uspěje v nalezení platného hashe, kandidátní blok se stává platným blokem a je vysílán do sítě, aby byl přidán do blockchainu.