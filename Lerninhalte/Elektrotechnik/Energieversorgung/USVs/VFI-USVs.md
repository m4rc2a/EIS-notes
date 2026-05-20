---
aliases:
  - Voltage and Frequency Independent USV
  - Online-USV
  - VFI-USV
  - Doppelwandler-USV
tags:
  - ApT-1-2025
classification: public
---
Eine **[[VFI-USVs|VFI-USV]]** (auch **Online-USV** oder **Doppelwandler-USV**) ist die hochwertigste Art der [[USVs|USV]].

# Funktionsweise
## Immer über den Doppelwandler
Die angeschlossenen Geräte werden **immer** über die [[USVs|USV]] versorgt – auch im Normalbetrieb. Der Strom läuft durch zwei Wandlungsstufen:
1. **Gleichrichter**: Netz-Wechselspannung → Gleichspannung (lädt gleichzeitig die Batterie)
2. **Wechselrichter**: Gleichspannung → saubere Wechselspannung für die Verbraucher

## Bei Störungen
Da die Verbraucher ohnehin immer aus der [[USVs|USV]] versorgt werden, gibt es **keine Umschaltzeit** (0 ms). Fällt das Netz aus, liefert die Batterie einfach weiter.

# Merkmale
- Keine Umschaltzeit (0 ms) – immer unterbrechungsfrei
- Vollständige Entkopplung vom Netz: Spannung und Frequenz werden neu erzeugt
- Bester Schutz vor allen Netzstörungen (Spannungsspitzen, Frequenzabweichungen, Verzerrungen)
- Höherer Preis und höhere Eigenverluste (durch doppelte Wandlung)
- Typischer Einsatz: Kritische Systeme, Rechenzentren, Medizintechnik
