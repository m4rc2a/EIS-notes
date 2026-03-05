---
aliases:
  - MUX
  - mux
  - Mux
classification: public
---

Ein **Multiplexer** (kurz: MUX) ist ein **[[Bauteil]]**, das aus **mehreren Eingangssignalen genau eines auswählt** und auf **einen gemeinsamen Ausgang** durchschaltet.

# Eingänge
| Bezeichnung            | Bedeutung                                             |
| ---------------------- | ----------------------------------------------------- |
| $I_0, I_1, I_2, \dots$ | Dateneingänge (Eingänge zwischen den ausgewählt wird) |
| $S_0, S_1, \dots$      | Selektleitung (wählt $I_x$ aus)                       |
| $EN$ (optional)        | Enable / Freigabe                                     |
# Ausgänge
| Bezeichnung | Bedeutung                         |
| ----------- | --------------------------------- |
| $Y$         | Ausgang (gewählter Eingang $I_x$) |
# Verhältnis-Schreibweise
"$m:n$" bedeutet: $m$ Eingänge und n Ausgänge
## Beispiele
## 2:1 Multiplexer
- 2 Dateneingänge: $I_0$, $I_1$
- 1 Ausgang: $Y$
### 4:1 Multiplexer
- 4 Dateneingänge: $I_0, I_1, I_2, I_3$
- 1 Ausgang: $Y$
### 1:4 Multiplexer
- 1 Dateneingang: $I_0$
- 4 Ausgänge: $Y_0, Y_1, Y_2, Y_3$

-> Das ist ein [[Demultiplexer|DEMUX]]
