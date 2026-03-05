---
tags:
  - Grundlagen
  - Thermik
  - Löten
  - Ausbildung
aliases:
  - thermische Masse
  - Wärmekapazität
  - thermische Trägheit
  - thermische Massen
  - Wärmekapazitäten
classification: public
---
Das **Wärmespeichervermögen** (auch: thermische Masse) beschreibt, wie viel Wärmeenergie ein Körper "speichern" kann, ohne dass seine Temperatur **sofort** sich stark ändert.
Wärmekapazität

> [!tldr] Kurzgesagt
> - **Hohes Wärmespeichervermögen** -> der Körper bleibt beim Abgeben/ Aufnehmen von Wärme **länger stabil** in der Temperatur.
> - **Niedriges Wärmespeichervermögen** -> die Temperatur kann sich **schneller** ändern.
# Beispiel
- Ein **dicker Stein** in der Sonne wird langsam warm und kühlt abends langsam wieder aus
	-> **hohes** Wärmespeichervermögen.
- Ein **dünnes Blech** wird schnell heiß und schnell wieder kalt
	→ **niedriges** Wärmespeichervermögen.
# Zusammenhang mit Wärmekapazität (für die Einordnung)
In der Physik heißt das dahinterliegende Maß **Wärmekapazität** $C$.
- $C$ sagt: *Wie viel Energie braucht es, um die Temperatur um $1\,\mathrm{K}$ zu ändern?*
- Einheit: $\mathrm{J/K}$

Formel:

$$
C=\frac{\Delta Q}{\Delta T}
$$

Für ein bestimmtes Material gilt außerdem:

$$
C=m\cdot c
$$

- \(m\) = Masse (kg)  
- \(c\) = spezifische Wärmekapazität \(\bigl(\mathrm{J/(kg\cdot K)}\bigr)\)

**Wichtig:** In der Praxis sagt man oft „Wärmespeichervermögen“, weil es verständlicher ist als „Wärmekapazität“.

---

## Warum ist das beim Löten wichtig?
Beim Löten soll die Lötspitze Wärme **in die Lötstelle** bringen. Dabei passiert Folgendes:
- Die Lötstelle „zieht“ Wärme aus der Spitze.
- Wenn die Spitze **wenig Wärmespeichervermögen** hat, fällt ihre Temperatur schnell ab → das Lot schmilzt schlechter, man muss länger draufhalten.
- Wenn die Spitze **viel Wärmespeichervermögen** hat, bleibt die Temperatur stabiler → schnelleres, saubereres Löten.

---

## Typische Beobachtungen in der Werkstatt
### Hohe „thermische Masse“/Wärmespeichervermögen (z. B. größere Spitze)
- Temperatur bricht beim Kontakt weniger ein
- gut für: größere Pads, dicke Leitungen, Masseflächen
- Nachteil: kann bei feinen Bauteilen schneller „zu viel“ Wärme eintragen

### Niedrige „thermische Masse“/Wärmespeichervermögen (z. B. sehr feine Spitze)
- reagiert schnell, gut dosierbar
- gut für: SMD, kleine Pads
- Nachteil: bei großen Kupferflächen kühlt sie schnell ab

---

## Wovon hängt das Wärmespeichervermögen einer Lötspitze ab?
- **Masse/Größe der Spitze** (mehr Metall = mehr gespeicherte Wärme)
- **Materialaufbau** (z. B. Kupferkern, Beschichtungen)
- **Geometrie** (Meißelspitzen übertragen oft besser als sehr spitze Nadeln)
- **Kontaktfläche zur Lötstelle** (mehr Kontakt = mehr Wärmeübertragung)

---

## Häufige Verwechslung: Wärmespeichervermögen vs. Heizleistung
- **Wärmespeichervermögen**: „Wie viel Wärme ist *drin*?“ (Puffer)
- **Heizleistung/Regelung** der Station: „Wie schnell kommt Wärme *nach*?“ (Nachschub)

Beides zusammen entscheidet, ob die Temperatur beim Löten stabil bleibt.

---

## Mini-Checkliste (praxisnah)
Wenn du merkst, dass das Lot schlecht schmilzt oder du zu lange heizen musst:
1. **Spitze größer/geeigneter wählen** (mehr Wärmespeichervermögen + bessere Kontaktfläche)
2. **Spitze sauber und verzinnt?** (Oxid wirkt wie Isolator)
3. **Temperatur passend?** (nicht zu niedrig – aber auch nicht unnötig hoch)
4. **Masseflächen**: ggf. breitere Spitze, Vorheizen oder mehr Leistung nutzen

---

## Kurzfazit
**Wärmespeichervermögen** bedeutet: *Wie gut kann ein Körper Wärme „puffern“, ohne stark abzukühlen?*  
Bei Lötspitzen hilft ein passendes Wärmespeichervermögen dabei, die **Temperatur an der Lötstelle stabil** zu halten und **schnell sauber** zu löten.



lunker
