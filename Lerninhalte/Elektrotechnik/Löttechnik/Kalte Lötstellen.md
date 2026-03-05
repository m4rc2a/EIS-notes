---
tags:
  - elektronik
  - löten
  - fehleranalyse
aliases:
  - Cold solder joint
  - Kalte Lötstelle
created: 2026-03-04
classification: public
---
Eine **kalte Lötstelle** ist eine **mechanisch und elektrisch schlechte Lötverbindung**.
Sie entsteht dadurch, dass eine Lötstelle nicht korrekt vom Lötzinn benetzt wurde oder die Verbindung **beim Abkühlen bewegt** wurde.
-> Ergebnis: Wackelkontakt oder hoher Übergangswiderstand

![Kalte Lötstelle](https://upload.wikimedia.org/wikipedia/commons/2/20/Cold_solder_joint2.jpg)

# Typische Ursachen
- **Zu geringe Löttemperatur** (Lötspitze/Pad/Bauteil wird nicht ausreichend erwärmt)
- **Zu kurze Lötzeit** (Lot schmilzt zwar, aber Benetzung bleibt unvollständig)
- **Bewegung während des Erstarrens** (Stecker/Bauteil verrutscht)
- **Oxidierte/verschmutzte Oberflächen** (Pads, Bauteilbeinchen, alte Lötspitze)
- **Zu wenig/ungeeignetes Flussmittel**
- **Wärmeabfuhr zu hoch** (z. B. große Masseflächen ohne Vorwärmen/geeignete Spitze)
# Erkennungsmerkmale
## erste Symptome
bereits bei der Benützung eines Geräts können sich Symptome einer **kalten Lötstelle** zeigen
- Gerät funktioniert nur bei **Druck/Biegen/Klopfen**
- Wiederholend auftretende Fehler (kommen und gehen)
- **Erwärmung** an der Stelle (durch erhöhten Übergangswiderstand)
- Messbar: **instabiler [[Widerstand]]** / Spannungsabfall unter Last
## Sichtprüfung
bei einer **Sichtprüfung** der Platine lassen sich **kalte Lötstellen** erkennen an:
- **Matt**, **körnig**, manchmal **rissig**
- Wirkt wie „**aufgelegt**“ statt sauber verlaufen
- Unter Lupe: **Haarrisse** am Übergang Lot <-> Pad/Pin
# Behebung
1. **reinigen der Lötstelle**, ggf. entlöten
2. **Flussmittel** dazu geben
3. Lötstelle **sauber** benetzen
4. **Nicht bewegen**, bis vollständig erstarrt
5. Flussmittelreste je nach Typ **reinigen**
# Vorbeugung
- Passende **Lötspitze** (mit [[Wärmespeichervermögen|Wärmekapazität]]) und **Temperatur** wählen
- Genug Zeit fürs **Durchwärmen** von Pad + Anschluss
- **Saubere** Spitze (abstreifen/abziehen) und ggf. neu verzinnen
- Bei großen Masseflächen: **Vorwärmen**, mehr Leistung oder größere Spitze
- [[Bauteile]] während des Lötens **fixieren** (z. B. „dritte Hand“, Klebeband, Halteklammer)

## Merksatz
**Nicht das Lot muss nur schmelzen – die Kontaktflächen müssen heiß genug sein, damit das Lot sauber benetzt.**
