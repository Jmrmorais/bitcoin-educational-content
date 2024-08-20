---
term: TAPROOT
---

Ein bedeutendes Update für das Bitcoin-Protokoll, das durch einen Soft Fork im November 2021 angenommen wurde. Dieses Update bringt signifikante Verbesserungen in Bezug auf Privatsphäre, Effizienz und Flexibilität durch die Implementierung von BIP340, BIP341 und BIP342. Dieses Update wurde bei Block 687.284 am 12. Juni 2021 gesperrt, als 90% der in einem Zeitraum generierten Blöcke dafür signalisierten, was die Bereitschaft der Miner zur Aktivierung des Updates anzeigte (*Speedy Trial*). Die Aktivierung fand schließlich bei Block 709.632 am 14. November 2021 statt, fast vier Jahre nach den ersten Diskussionen zu dem Thema zwischen Pieter Wuille, Andrew Poelstra und Gregory Maxwell. Es war der erste bedeutende Aktualisierungsversuch seit der kontroversen Aktivierung von SegWit im Jahr 2017.

Taproot ist auch der Name von BIP341, das innerhalb des gleichnamigen Soft Forks implementiert wurde und ein neues Skriptmodell namens P2TR einführt. Ein P2TR-Skript sperrt Bitcoins auf einem einzigartigen Schnorr-Öffentlichen-Schlüssel, bezeichnet als $K$. Dieser Schlüssel $K$ ist jedoch tatsächlich eine Aggregation eines öffentlichen Schlüssels $P$ und eines öffentlichen Schlüssels $M$, wobei letzterer aus der Merkle-Wurzel einer Liste von `scriptPubKey` berechnet wird. Die mit einem P2TR-Skript gesperrten Bitcoins können auf zwei unterschiedliche Weisen ausgegeben werden: entweder durch Veröffentlichung einer Signatur für den öffentlichen Schlüssel $P$ oder durch Erfüllung eines der Skripte im Merkle-Baum. Die erste Option wird als "*key path*" bezeichnet und die zweite als "*script path*".