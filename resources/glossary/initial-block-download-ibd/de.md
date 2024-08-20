---
term: INITIAL BLOCK DOWNLOAD (IBD)
---

Bezieht sich auf den Prozess, durch den ein Knoten die Blockchain vom Genesis-Block herunterlädt und verifiziert und sich mit anderen Knoten im Bitcoin-Netzwerk synchronisiert. IBD muss durchgeführt werden, wenn ein neuer Full Node gestartet wird. Zu Beginn dieser anfänglichen Synchronisierung hat der Knoten keine Informationen über vorherige Transaktionen. Daher lädt er jeden Block von anderen Knoten im Netzwerk herunter, überprüft dessen Gültigkeit und fügt ihn dann seiner lokalen Version der Blockchain hinzu. Es ist erwähnenswert, dass IBD aufgrund der wachsenden Größe der Blockchain und des UTXO-Sets langwierig und ressourcenintensiv sein kann. Die Geschwindigkeit seiner Ausführung hängt von den Rechenkapazitäten des Computers ab, der den Knoten hostet, seiner RAM-Kapazität, der Geschwindigkeit des Speichergeräts und der Bandbreite. Um Ihnen eine Vorstellung zu geben, wenn Sie eine leistungsfähige Internetverbindung haben und der Knoten auf dem neuesten MacBook mit viel RAM gehostet wird, dauert der IBD nur wenige Stunden. Im Gegensatz dazu, wenn Sie einen Mikrocomputer wie einen Raspberry Pi verwenden, könnte der IBD eine Woche oder länger dauern.

> ► *Im Französischen wird allgemein direkt auf einen IBD Bezug genommen. Die manchmal verwendete Übersetzung ist "synchronisation initiale" oder "téléchargement initial des blocs".*