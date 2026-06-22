---
aliases:
  - Variable
  - Variablen
  - Konstante
  - Konstanten
  - finale Variable
tags:
  - LF8
  - LF8-Klausur
classification: public
---
**Variablen** sind benannte Speicherplätze für Werte eines bestimmten [[Datentypen|Datentyps]]. **Konstanten** sind Variablen, deren Wert nach der Initialisierung nicht mehr geändert werden kann.

# Deklaration und Initialisierung

```java
// Deklaration (Speicherplatz reservieren)
int alter;

// Initialisierung (Wert zuweisen)
alter = 18;

// Deklaration + Initialisierung in einem Schritt
double preis = 9.99;
```

# Konstanten mit `final`

```java
final double MWST = 0.19;
final int MAX_ANZAHL = 100;
```

Konstanten werden per Konvention **GROSS_GESCHRIEBEN**. Der Wert einer `final`-Variable kann nach der ersten Zuweisung nicht mehr geändert werden.

# Namenskonventionen

| Art | Beispiel |
| --- | -------- |
| Variable | `anzahlBelag`, `gesamtPreis` (camelCase) |
| Konstante | `GRUNDPREIS_PIZZA`, `MWST` (UPPER_SNAKE_CASE) |
| Klasse | `PizzaAufgabe` (PascalCase) |

# Das EVA-Prinzip mit Variablen

Das [[../Benutzereingabe|EVA-Prinzip]] (Eingabe → Verarbeitung → Ausgabe) wird in Java mit Variablen umgesetzt:

```java
// E – Eingabe (Benutzereingabe)
int anzahl = InOut.readInt("Anzahl:");

// V – Verarbeitung (Berechnung)
double gesamt = anzahl * preis;

// A – Ausgabe (Ergebnis anzeigen)
System.out.println("Gesamt: " + gesamt);
```

Ein vollständiges Beispiel mit Konstanten und Variablen ist die [[Beispiele/PizzaBerechnung|PizzaBerechnung]].
