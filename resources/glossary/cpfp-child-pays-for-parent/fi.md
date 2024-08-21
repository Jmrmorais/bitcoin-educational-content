---
termi: CPFP (CHILD PAYS FOR PARENT)
---

Transaktiomekanismi, jonka tavoitteena on nopeuttaa Bitcoin-siirron vahvistumista, samankaltaisesti kuin mitä Replace-by-Fee (RBF) tekee, mutta vastaanottajan puolelta. Kun siirto, jonka kulut ovat liian matalat markkinavergleicheen nähden, jää jumiin solmujen mempooleihin eikä vahvistu tarpeeksi nopeasti, vastaanottaja voi tehdä uuden siirron, käyttäen bitcoineja, jotka on saatu jumissa olevassa siirrossa, vaikka sitä ei ole vielä vahvistettu. Tämä toinen siirto edellyttää välttämättä, että ensimmäinen louhitaan ennen kuin se voidaan vahvistaa. Louhijat pakotetaan siten sisällyttämään molemmat siirrot yhdessä. Toinen siirto osoittaa paljon enemmän transaktiokuluja kuin ensimmäinen, siten että keskimääräinen kulu kannustaa louhijoita sisällyttämään molemmat siirrot. Lapsitransaktio (toinen) maksaa vanhemman transaktion puolesta, joka on jumissa (ensimmäinen). Tästä syystä sitä kutsutaan "CPFP:ksi".

Näin ollen CPFP mahdollistaa vastaanottajan saada varansa nopeammin huolimatta lähettäjän alun perin maksamista matalista kuluista, toisin kuin RBF (*Replace-By-Fee*), joka mahdollistaa lähettäjän ottaa aloitteen nopeuttaakseen omaa siirtoaan lisäämällä kuluja.