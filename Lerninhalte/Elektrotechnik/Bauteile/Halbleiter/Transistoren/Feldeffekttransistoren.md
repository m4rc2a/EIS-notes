---
aliases:
  - Feldeffekttransistor
tags:
  - LF06
classification: public
---
Ein **[[Feldeffekttransistoren|Feldeffekttransistor]] (FET)** ist ein [[Bauteile|elektronisches Bauteil]], das [[Stromstärke|Ströme]] und [[Spannung|Spannungen]] [[Steuern]] kann. Im Unterschied zum Bipolartransistor wird ein FET nicht durch einen [[Stromstärke]], sondern durch eine elektrische *[[Spannung]]* am sogenannten „Gate“ gesteuert.

# Aufbau
Ein FET besitzt drei Anschlüsse:
- **Source (S):** Hier fließen die Elektronen hinein ^Source
- **Drain (D):** Hier fließen die Elektronen hinaus ^Drain
- **Gate (G):** Steuert den [[Stromstärke|Stromfluss]] zwischen Source und Drain ^Gate
# Funktionsweise
Am FET wird der elektrische [[Stromstärke]] durch ein elektrisches Feld beeinflusst, das sich zwischen Gate und Source aufbaut. Wird am Gate eine bestimmte [[Spannung]] angelegt, verändert sich die Leitfähigkeit des Halbleiterkanals zwischen Source und Drain – und der [[Stromstärke]] kann fließen (oder eben nicht).

> [!Merke]
> Ein FET wird *spannungs*gesteuert (nicht stromgesteuert) und benötigt am Gate fast keinen Strom, solange die [[Spannung]] konstant bleibt.

# Typen

Es gibt verschiedene FET-Typen, am wichtigsten sind:
- **[[MOSFET]]** (Metall-Oxid-Halbleiter-Feldeffekttransistor)
- **[[J-FET]]** (Junction-Feldeffekttransistor)

> [!note] #TODO Hier irgendwas hinschreiben Notizen:
>CMOS Technik -> Bulk anschluss?
> IG Feld $I_G$ ([[#^Gate|Gate]])
> -> siehe lf6 Notizen Tablet

# Variablen
- Drain‑Source‑[[Spannung]] $U_{DS}$
- Drain Strom $I_D$
- Gate‑Source‑[[Spannung]] $U_{GS}$

- $I_{DSS}$: Drain‑Source‑„Kurzschlussstrom“ (bei (U_{GS}=0); typisch für JFET‑Daten).
- $U_{GS(\text{OFF})}$: „Abschnürspannung“/Sperrspannung am Gate—ab hier ist der Kanal praktisch zu (Drainstrom geht gegen 0).
- $U_{DS\text{sat}}$: Drain‑Source‑Sättigungsspannung (Übergang vom linearen Bereich in den Sättigungs-/Abschnürbereich).

### Was kann man damit rechnen?

- **Gleichstromleistung am FET:**

$$P = U_{DS}\cdot I_D$$

- **Eingangswiderstand aus Gate‑Leckstrom** (bei (U_{DS}=0)):

$$R_{GS}=\frac{U_{GS}}{I_{GSS}}$$

### Bilder rechts

- Zeigt die **Bezugsrichtungen** (Pfeile/Polungen) für Strom und [[Spannung]] beim **IGFET/MOSFET (Verarmungstyp)** und beim **JFET** – damit man weiß, wie (U_{GS}), (U_{DS}) und (I_D) im Schaltbild „gezählt“ werden.

### Unten: Aufgaben/Beispiel

- Rechenübungen wie: **Leistung**, **Drainstrom**, **Gate‑Leckstrom/Eingangswiderstand**, sowie Werte aus **Kennlinien ablesen**.

Wenn du willst: Sag mir, welche **Aufgabe (z. B. 1–9)** du meinst oder lade die **Kennlinien-Seite** mit hoch, dann rechne ich sie mit dir Schritt für Schritt durch.
