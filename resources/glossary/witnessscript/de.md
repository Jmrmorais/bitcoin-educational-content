---
term: WITNESSSCRIPT
---

Ein Skript, das die Bedingungen festlegt, unter denen Bitcoins von P2WSH oder P2SH-P2WSH UTXOs ausgegeben werden können. Typischerweise bestimmt `witnessScript` die Bedingungen einer Multisignatur-Wallet unter dem SegWit-Standard. In diesen Skriptstandards enthält das `scriptPubKey` des UTXO (der Ausgang) einen Hash des `witnessScript`. Um dieses UTXO als Eingabe in einer neuen Transaktion zu verwenden, muss der Inhaber das ursprüngliche `witnessScript` offenlegen, um dessen Übereinstimmung mit dem Fingerabdruck im `scriptPubKey` zu beweisen. Das `witnessScript` muss dann im `scriptWitness` der Transaktion enthalten sein, das auch die Elemente enthält, die zur Validierung des Skripts notwendig sind, wie z.B. Signaturen. Daher ist das `witnessScript` das Äquivalent für SegWit des `redeemScript` in einer P2SH-Transaktion, mit dem Unterschied, dass es im Zeugenbereich der Transaktion platziert wird und nicht im `scriptSig`.

> ► *Vorsicht, das `witnessScript` sollte nicht mit dem `scriptWitness` verwechselt werden. Während das `witnessScript` die Ausgabebedingungen eines P2WSH oder P2SH-P2WSH UTXO definiert und ein eigenständiges Skript darstellt, enthält das `scriptWitness` die Zeugendaten jeder SegWit-Eingabe.*