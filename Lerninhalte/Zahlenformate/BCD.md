# Begriffserklärung
[[BCD]] (Kurtz für **Binary Coded Decimal**) ein [[Zahlenformat]], bei der jede Dezimalziffer einzeln durch 4 Bits kodiert wird.
Dadurch können Zahlen leicht in Geräten verarbeitet oder angezeigt werden, die mit Dezimalwerten arbeiten.

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