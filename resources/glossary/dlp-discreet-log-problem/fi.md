---
termi: DLP (DISCREET LOG PROBLEM)
---

Diskreetin logaritmin ongelma (DLP) on matemaattinen ongelma, joka on julkisen avaimen kryptografisten algoritmien turvallisuuden perustana, erityisesti niiden, joita käytetään Bitcoinissa. Syklisessä ryhmässä, jonka järjestys on $q$, ja jolla on generaattori $g$, jos on olemassa yhtälö muodossa $g^x = h$, silloin $x$ kutsutaan $h$:n diskreetiksi logaritmiksi suhteessa kantaan $g$, modulo $q$. Yksinkertaisesti sanottuna, se sisältää eksponentin $x$ määrittämisen, kun $g$, $h$ ja $q$ ovat tiedossa. Diskreetti logaritmi on siis eksponentiaalifunktion käänteisoperaatio äärellisessä syklisessä ryhmässä. Kuitenkin suurille $q$:n arvoille diskreetin logaritmin ongelman ratkaiseminen katsotaan algoritmisen vaikeaksi. Tätä ominaisuutta hyödynnetään monien kryptografisten protokollien, kuten Diffie-Hellmanin protokollan avainvaihdon, turvaamisessa. Diskreettiä logaritmia käytetään myös elliptisen käyrän kryptografiassa (ECC), mukaan lukien Elliptisen Käyrän Digitaalisessa Allekirjoitus Algoritmissa (ECDSA). Elliptisten käyrien kontekstissa diskreetin logaritmin ongelma laajenee skalaarin $k$ löytämiseen siten, että $k \cdot G = K$, missä $G$ ja $K$ ovat pisteitä käyrällä, ja $\cdot$ edustaa pisteen kertolaskuoperaatiota. Bitcoinin kontekstissa standarditransaktiot käyttävät joko ECDSA:ta tai Schnorrin protokollaa UTXO:jen lukitsemiseen. Molemmat nojaavat diskreetin logaritmin laskennan epäkäytännöllisyyteen.