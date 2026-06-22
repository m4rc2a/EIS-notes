---
aliases:
  - Java Operatoren
  - arithmetische Operatoren
  - Inkrement
  - Dekrement
tags:
  - LF8
  - LF8-Klausur
classification: public
---
**Operatoren** führen Operationen auf [[Datentypen|Werten]] und [[Variablen und Konstanten|Variablen]] aus.

# Arithmetische Operatoren

| Operator | Bedeutung | Beispiel |
| -------- | --------- | -------- |
| `+` | Addition | `preis + 1.50` |
| `-` | Subtraktion | `summe - rabatt` |
| `*` | Multiplikation | `anzahl * preis` |
| `/` | Division | `gesamt / 2` |
| `%` | Modulo (Rest) | `7 % 2 → 1` |

# Inkrement und Dekrement

```java
int zahl = 5;
zahl++;   // jetzt 6 (zahl = zahl + 1)
zahl--;   // jetzt 5 (zahl = zahl - 1)
```

`++variable` und `variable++` sind gleichbedeutend mit `variable = variable + 1`.

# Zusammengesetzte Zuweisungen

```java
int x = 10;
x += 5;     // x = x + 5 → 15
x *= 2;     // x = x * 2 → 30
```

# Operator-Rangfolge (Punkt vor Strich)

Wie in der Mathematik gilt: `*`, `/`, `%` vor `+`, `-`.

```java
int ergebnis = 5 + 3 * 2;  // → 11 (nicht 16)
```

In den [[Beispiele/PizzaBerechnung|Beispielen]] siehst du, wie Operatoren im EVA-Prinzip ([[Systemdenken/EVA-Prinzip|EVA]]) eingesetzt werden.
