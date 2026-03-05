---
aliases:
  - differenzielle Signalführung
  - symmetrische Signalführung
  - symmetrische Führung
classification: public
---
**Differenzführung** (auch _differenzielle Signalführung_, _symmetrische Führung_) ist eine Art der Signalführung, bei der ein [[elektrische Signale|Signal]] über **zwei Leiter als Paar** geführt wird und der Empfänger **nicht die [[Spannung]] eines Leiters gegen Masse** auswertet, sondern **die Spannungsdifferenz zwischen beiden Leitern**.
# Prinzip
Zwei Leitungen tragen entgegengesetzte Signalanteile (V_1) und (V_2). Ausgewertet wird:

$$V_\mathrm{diff} = V_1 - V_2$$

Zusätzlich kann es einen gemeinsamen Anteil geben ([[Gleichtakt]]):

$$V_\mathrm{CM} = \frac{V_1 + V_2}{2}$$

Der große Vorteil: **Störungen**, die auf beide Leitungen ähnlich einwirken (Gleichtaktstörungen), werden im Idealfall bei der Differenzbildung **weitgehend unterdrückt**.

# Typische Merkmale
- **zwei Adern als Paar** (oft verdrillt)
- Empfänger misst **Differenz** statt „gegen GND“
- **bessere Störfestigkeit** und meist **geringere Abstrahlung (EMV)**
- wichtig: **gleiche Leitungslänge/Impedanz** im Paar (symmetrisches Routing)

# Beispiele
- Digitale Schnittstellen: **[[RS-485]]**, **CAN**, **LVDS**, **Ethernet**
- Analog: **symmetrisches Audio**, **Messbrücken (Wheatstone)**, differenzielle Sensorsignale
