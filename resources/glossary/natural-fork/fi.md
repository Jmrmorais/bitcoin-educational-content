---
term: LUONNOLLINEN HAARAUMA
---

Tilapäinen lohkoketjun eriytyminen, joka johtuu lähes samanaikaisesta useiden lohkojen lähettämisestä eri louhijoilta samalla korkeudella. Tämä tilanne tapahtuu, kun kaksi lohkoa, jotka on nimetty $A$ ja $B$, löydetään lähes samaan aikaan, mikä johtaa verkon tilapäiseen jakautumiseen. Koska jokainen solmu pitää ensimmäisenä vastaanottamaansa lohkoa kelvollisena, mutta kaikki eivät vastaanottaneet samaa lohkoa ensimmäisenä, osa solmuista seuraa ketjua, joka sisältää lohkon $A$, kun taas toinen osa seuraa ketjua, jossa on lohko $B$. Tämä haarauma ratkeaa, kun yksi kahdesta kilpailevasta ketjusta ylittää toisen kertyneen työn määrässä. Tässä vaiheessa kaikki verkon solmut automaattisesti hyväksyvät pidemmän ketjun (jolla on eniten kertynyttä työtä), prosessi, joka tunnetaan uudelleenjärjestelynä tai uudelleensynkronointina. Nämä luonnolliset haaraumat ovat osa Bitcoinin hajautetun toiminnan luonnetta. Ne ovat täysin normaaleja ja ratkeavat itsestään muutaman lohkon jälkeen (yleensä vain yhden). Jos ne kuitenkin tapahtuvat liian usein, nämä haaraumat voivat silti olla haitallisia, koska ne johtavat laskentatehon tuhlaukseen haaraumassa, joka lopulta muuttuu vanhentuneeksi.