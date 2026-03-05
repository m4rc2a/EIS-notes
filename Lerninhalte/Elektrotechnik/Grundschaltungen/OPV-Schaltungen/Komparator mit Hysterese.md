---
aliases:
  - Schmitt Trigger
tags:
  - LF06
classification: public
---
Ein **Komparator mit Hysterese** (oder auch: **[[Komparator mit Hysterese|Schmitt Trigger]]**) ist eine elektronische Schaltung, mit [[Operationsverstärker]], die zwei analoge Spannungssignale mit einem Schwellwert miteinander vergleicht und am Ausgang ein digitales Spannungssignal liefert.
-> Ausgang nur HIGH oder LOW
-> Beim Vergleich mit Schwellwert

Es besitzt eine [[Mitkopplungen]] (positive [[Rückkopplungen]]) in Form eines Widerstandes.

```Mermaid
graph LR
    V1[12V] --> S1[Schalter]
    S1 --> R1[220Ω]
    R1 --> LED1[LED]
    LED1 --> GND
```

Es gibt eine Hysterese [[Spannung]] #TODO

# Beschaltung
![[KomparatorHyst.svg]]
