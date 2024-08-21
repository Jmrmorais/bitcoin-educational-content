---
term: EELDADA KEHTIVAT
---

Konfiguratsiooniparameeter enamuses kliendis Bitcoin Core, mis võimaldab äsja initsialiseeritud sõlmel (kuid pole veel teostanud IBD-d) jätta vahele kõikide tehingute allkirjade kontrollimise blokkides, mis on enne teatud kindlat blokki. See kuulus blokk on määratletud oma päise jäljendi, ehk selle räsi järgi. Valitud blokki uuendatakse iga uue Bitcoin Core versiooniga. Selle parameetri aktiveerimisel kontrollib sõlm oma initsialiseerimisel blokipeade ahelat, et leida haru, millel on kõige rohkem kogunenud tööd. Kui sõlm tuvastab Core'i poolt antud räsi valitud harus, jätab ta eelnevate blokkide allkirjade kontrollimise vahele. Vastasel juhul jätkab sõlm traditsioonilise sünkroniseerimisega (IBD), et kõike ise kontrollida.

Eeldada Kehtivat eesmärk on kiirendada sõlme esialgse sünkroniseerimise protsessi, ohverdamata turvalisust, eeldades, et enamik võrgust on neid tehinguid minevikus juba valideerinud. Ainus tegelik kompromiss sõlme jaoks on see, et varasema bitcoini varguse korral ei teavitata seda. Siiski saab see siiski tagada väljastatud bitcoinide koguse täpsuse. Sõlmed jätkavad allkirjade kontrollimist tehingutele, mis järgnevad Eeldada Kehtivat blokile. See lähenemine põhineb eeldusel, et kui tehing on võrgustiku poolt piisavalt kaua ilma vaidlusteta aktsepteeritud, on ebatõenäoline, et see on petlik.