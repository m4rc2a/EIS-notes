---
classification: public
---
# [[Gleichtakt|Common‑Mode]] bei RS‑485
Bei RS‑485 hast du zwei Leitungen **A** und **B**. Der Empfänger interessiert sich nur für das Differenzsignal.

# Grundidee
- **Differenzverstärker**: Verstärkt die _Differenz_ zweier Eingangssignale und unterdrückt Anteile, die an beiden Eingängen gleich sind.
- **Störunterdrückung**: Störungen (z. B. eingekoppelte Brumm-/EMI-Signale), die auf beiden Leitungen ähnlich auftreten, werden weitgehend „wegsubtrahiert“.

---

# Wichtige Begriffe (Glossar)

## Signalarten

- **Differenzsignal (Nutzsignal)**
    - Anteil, der _zwischen_ den beiden Eingängen unterschiedlich ist.
    - Formal: $(V_d = V_+ - V_-)$
- **Gleichtaktsignal (Common-Mode)**
    - Anteil, der _auf beiden_ Eingängen gleich/ähnlich ist (typische eingekoppelte Störung).
    - Formal: $(V_{cm} = \frac{V_+ + V_-}{2})$

## Verstärkungen

- **Differenzverstärkung (A_d)**
    - Verstärkung für das Differenzsignal (V_d).
    - Ausgangsanteil: (V_{out,d} = A_d \cdot V_d)
- **Gleichtaktverstärkung (A_{cm})**
    - (Unerwünschte) Verstärkung für den Gleichtaktanteil (V_{cm}).
    - Ausgangsanteil: (V_{out,cm} = A_{cm} \cdot V_{cm})

## Kennzahl für Störunterdrückung

- **CMRR (Common-Mode Rejection Ratio / [[Gleichtaktunterdrückung]])**
	- Verhältnis, wie viel stärker der Verstärker Differenz- statt Gleichtaktsignal verstärkt.
$$\mathrm{CMRR} = \frac{A_d}{A_{cm}}$$
- In dB:  
$$\mathrm{CMRR}_{dB} = 20\log_{10}\left(\frac{A_d}{A_{cm}}\right)$$
> [!tldr] Merksatz:
> **Je höher CMRR, desto besser die Störunterdrückung.**

---

# Wie funktioniert die Unterdrückung praktisch?

## „Subtraktion“ als Prinzip

- Wenn eine Störung auf beiden Leitungen gleich ist:
    - (V_+ = V_{sig+} + V_{stör})
    - (V_- = V_{sig-} + V_{stör})
- Dann wird beim Differenzbilden:
    - (V_d = (V_{sig+} + V_{stör}) - (V_{sig-} + V_{stör}) = V_{sig+} - V_{sig-})
- Ergebnis: **(V_{stör}) hebt sich idealerweise auf.**

## Realität: Warum bleibt manchmal doch Störung übrig?

- **Widerstands-/Impedanz-Mismatch** (kleine Abweichungen reichen)
- **Endliche CMRR** des Verstärkers (nicht unendlich)
- **Eingangsbiasströme / Offset** (je nach Schaltung relevant)
- **Frequenzabhängigkeit**: CMRR sinkt oft bei höheren Frequenzen
- **Unsymmetrische Verkabelung** oder ungleiche Quellenimpedanzen

---

# Typische Ursachen für Gleichtaktstörungen

- **EMI-Einkopplung** (Motoren, Schaltregler, Umrichter, Funk)
- **Brumm durch Netzfelder** (50/60 Hz)
- **Potentialunterschiede/Masseverschleppung** (Ground Loops)
- **Kapazitive/induktive Kopplung** in langen Leitungen

---

# Praxisregeln (Checkliste)

## Verkabelung / Layout

- **[[Differenzführung|Symmetrische Führung]]** (beide Leitungen gleich behandeln)
- **Verdrillte Adern (Twisted Pair)** → gleiche Einkopplung auf beide Leiter
- **Schirmung** (richtig aufgelegt, je nach Konzept einseitig/beidseitig)
- **Kurze Leitungen, kleine Schleifenflächen**
- **Gute Masse-/Potentialführung** (Grounding-Konzept)

## Schaltungsauswahl

- **Instrumentenverstärker (In-Amp)**
    - Speziell für hohe Eingangsimpedanz + hohe CMRR (oft besser als „einfacher“ Diff-Verstärker).
- **[[Widerstand|Widerstände]] präzise matchen**
    - Für klassische Diff-Verstärker-Schaltungen sind enge Toleranzen entscheidend.

## Spezifikationen, auf die man achtet

- **CMRR (bei relevanter Frequenz!)**
- **Eingangs-Common-Mode-Bereich** (darf nicht überschritten werden)
- **Eingangsimpedanz**
- **Offset / Drift**
- **Rauschen** (v. a. bei kleinen Sensorsignalen)

---

# Mini-Beispiel (Merkschema)

- Nutzsignal ist differenziell: (+10\ \mathrm{mV}) auf (V_+), (-10\ \mathrm{mV}) auf (V_-) → (V_d = 20\ \mathrm{mV})
- Störung ist gleich auf beiden: (+1\ \mathrm{V}) auf beiden → ideal: weg
- Real bleibt ein Rest je nach CMRR und Mismatch.
