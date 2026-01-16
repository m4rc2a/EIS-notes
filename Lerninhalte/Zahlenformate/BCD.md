# Begriffserklärung
[[BCD]] (Kurtz für **Binary Coded Decimal**) ein [[Zahlenformat]], bei der jede Dezimalziffer einzeln durch 4 Bits kodiert wird.
Dadurch können Zahlen leicht in Geräten verarbeitet oder angezeigt werden, die mit Dezimalwerten arbeiten.

# Leserichtung
[[BCD]] wird von **Von links nach rechts** geschrieben/gelesen so wie bei Dezimalzahlen.
# Kodierung
Um eine Dezimalzahl als [[BCD]] zu kodieren:
1. Wandle jede einzelne Ziffer in Binär um
2. Ordne für jede Ziffer die Binärwerte nacheinander an

> **Tipp**:
> Für die Ziffern 0 bis 9 gibt es feste Binärwerte – einfach merken oder mit der Zeit verinnerlichen.
# Dekodierung
Um eine [[BCD]] zahl zurück in Dezimalschreibweise zu konvertieren.
1. Teile als erstes die BCD-zahl in stücke, bestehend aus jeweils 4 Bits
2. Jedes 4 Bits stück zurück in Dezimal umwandeln
3. Dezimalziffern zusammen setzen
# Beispiel
- Die Zahl 1337 als [[BCD]]:
    - 1 -> `0001`
    - 3 -> `0011`
    - 3 -> `0011`
    - 7 -> `0111`
- Die BCD-Darstellung:  
    `0001 0011 0011 0111`