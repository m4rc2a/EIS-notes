---
aliases:
  - DEMUX
  - Demux
classification: public
---

Ein **Demultiplexer** (kurz: DEMUX) ist ein **[[Bauteil]]**, das ein **einzelnes Eingangssignal** auf **genau einen von mehreren Ausgängen** durchschaltet (je nach **Selektleitungen**).

# Eingänge
| Bezeichnung       | Bedeutung                                                                 |
| ----------------- | ------------------------------------------------------------------------- |
| $I$ (oder $D$)    | Dateneingang ([[elektrische Signale|Signal]], das verteilt/geroutet wird)                         |
| $S_0, S_1, \dots$ | Selektleitungen (wählen aus, *welcher* Ausgang aktiv ist)                 |
| $EN$ (optional)   | Enable / Freigabe (aktiviert den DEMUX; sonst sind Ausgänge inaktiv)      |

# Ausgänge
| Bezeichnung                  | Bedeutung                                              |
| --------------------------- | ------------------------------------------------------ |
| $Y_0, Y_1, Y_2, \dots$      | Ausgänge (genau einer übernimmt das Eingangssignal $I$) |

# Funktionsidee
- Für jede Selekt-Kombination wird **genau ein Ausgang** ausgewählt.
- Der ausgewählte Ausgang bekommt das [[elektrische Signale|Signal]]: $Y_x = I$
- Alle anderen Ausgänge sind **inaktiv** (typisch: $0$ oder hochohmig $Z$, je nach Baustein).

# Verhältnis-Schreibweise
"$m:n$" bedeutet: $m$ Eingänge und $n$ Ausgänge

- **Typischer DEMUX** ist **"$1:n$"**: ein Eingang, viele Ausgänge  
- **"$m:1$"** ist typischerweise ein [[Multiplexer|MUX]] (viele Eingänge, ein Ausgang)

## Beispiele

## 1:2 Demultiplexer
- 1 Dateneingang: $I$
- 2 Ausgänge: $Y_0$, $Y_1$
- Selekt: $S_0$

## 1:4 Demultiplexer
- 1 Dateneingang: $I$
- 4 Ausgänge: $Y_0, Y_1, Y_2, Y_3$
- Selekt: $S_1, S_0$

## 1:8 Demultiplexer
- 1 Dateneingang: $I$
- 8 Ausgänge: $Y_0 \dots Y_7$
- Selekt: $S_2, S_1, S_0$

## Hinweis (Abgrenzung)
Wenn du eine Schreibweise wie **"1:4"** siehst (ein Eingang, vier Ausgänge), ist das **ein DEMUX** (oder sehr nah verwandt: ein *Decoder* mit Enable).
