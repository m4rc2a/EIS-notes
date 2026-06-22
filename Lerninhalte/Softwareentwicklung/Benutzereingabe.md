---
aliases:
  - Benutzereingabe
  - Benutzereingaben
  - Nutzereingabe
  - User Input
  - Benutzereingabe und Ausgabe
  - Benutzereingabe / Ausgabe
tags:
  - LF8
  - LF8-Klausur
classification: public
---
**Benutzereingabe** beschreibt, wie ein Nutzer Daten und Anweisungen an ein Programm übergibt. Die **Ausgabe** ist die Rückmeldung des Programms an den Nutzer.

Dies ist ein zentraler Bestandteil des [[Systemdenken/EVA-Prinzip|EVA-Prinzips]] (Eingabe → Verarbeitung → Ausgabe).

# Eingabearten
- **Tastatureingabe** – Texte, Zahlen, Befehle
- **Maus/Gesten** – Klicks, Auswahl, Touch
- **Dateien** – Konfigurationsdateien, Messdaten
- **Schnittstellen** – Sensoren, APIs, Datenbanken

# Ausgabearten
- **Bildschirm** – Textausgabe, Grafiken, GUIs
- **Dateien** – Logs, Ergebnisse, Berichte
- **Schnittstellen** – API-Responses, Drucker, Aktoren

# Benutzereingabe in der Konsole
Der Nutzer gibt Text über die Tastatur ein. Das Programm liest die Eingabe mit `InOut.readInt()` oder `InOut.readDouble()` und gibt das Ergebnis mit `System.out.println()` aus.

```java
int zahl = InOut.readInt("Gib eine Zahl ein: ");
System.out.println("Deine Zahl ist: " + zahl);
```

Komplette Beispiele mit Eingabe und Ausgabe finden sich unter:
- [[Java/Beispiele/PizzaBerechnung|PizzaBerechnung]] – `InOut.readInt()` + Rechnung + Ausgabe
- [[Java/Beispiele/BlutalkoholBerechnung|BlutalkoholBerechnung]] – mehrere Eingaben + Berechnung + Ausgabe

> [!info] In der Elektrotechnik
> Auch in der Elektrotechnik gibt es Benutzereingabe – z. B. Taster, Schalter, Potentiometer. Diese Signale werden dann in einer Schaltung verarbeitet ([[Systemdenken/EVA-Prinzip|EVA-Prinzip]]).
