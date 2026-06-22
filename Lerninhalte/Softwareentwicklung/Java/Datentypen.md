---
aliases:
  - Datentyp
  - Variablentypen
  - primitive Datentypen
  - Java Datentypen
tags:
  - LF8
  - LF8-Klausur
classification: public
---
Ein **Datentyp** legt fest, welche Werte eine [[Variablen und Konstanten|Variable]] annehmen kann und welche Operationen auf ihr erlaubt sind. Java ist **typsicher** – der Typ einer Variable wird bei der Deklaration festgelegt und kann nicht geändert werden.

# Primitive Datentypen

| Typ | Beschreibung | Beispiel-Wert |
| --- | ------------ | ------------- |
| `int` | Ganze Zahl (Ganzzahl) | `42` |
| `double` | Gleitkommazahl (Kommazahl) | `3.14` |
| `boolean` | Wahrheitswert | `true` / `false` |
| `char` | Einzelnes Zeichen | `'A'` |

> [!tldr] Merksatz
> **i**nt, **d**ouble, **b**oolean, **c**har – die vier primitiven Datentypen in Java

# Zuweisungsregeln (aus der Übung)

Nicht jede Zuweisung ist in Java erlaubt. Der Typ des Wertes muss zum Typ der [[Variablen und Konstanten|Variable]] passen.

| Zuweisung | Zulässig? | Begründung |
| --------- | --------- | ---------- |
| `double x = 10;` | ✔ | `10` ist eine ganze Zahl, kann aber als Gleitkommazahl gespeichert werden (implizite Konvertierung) |
| `groesse++;` | ✔ | Inkrementation um 1 – gleichbedeutend mit `groesse = groesse + 1` |
| `boolean b = true;` | ✔ | `boolean` kennt nur `true` und `false` |
| `double d = 19;` | ✔ | `19` ist als `double` gültig (10er-Potenz ohne Nachkommastelle) |
| `double d = 20.0;` | ✔ | Explizite Gleitkommazahl |
| `int i = 10.5;` | ✘ | `double` auf `int` verlangt expliziten Cast |
| `char c = 5;` | ✔ | Ein einzelnes Zeichen (hier das Zeichen für den Zahlencode 5) |
| `int i = 23 + 5.0;` | ✔ | `int` + `double` ergibt `double` → erfordert Cast für `int`-Variable |

# Typkompatibilität
- **Automatische (implizite) Konvertierung**: `int` → `double` (von klein nach groß, sicher)
- **Expliziter Cast nötig**: `double` → `int` (`(int) 3.14` → `3`)

```java
double d = 10;           // ✔ implizit: int → double
int i = (int) 3.14;      // ✔ explizit: double → int (ergibt 3)
```

Weitere [[Operatoren|Operatoren]] und [[Variablen und Konstanten|Variablen]] bauen auf diesen Datentypen auf.
