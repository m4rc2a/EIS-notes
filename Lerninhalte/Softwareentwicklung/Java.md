---
aliases:
  - Java Sprache
  - Java-Programmierung
tags:
  - LF8
  - LF8-Klausur
classification: public
---
**Java** ist eine plattformunabhängige, objektorientierte [[Programmiersprachen|Programmiersprache]], die 1995 von Sun Microsystems (heute Oracle) entwickelt wurde.

# Eigenschaften
- **Plattformunabhängigkeit** – Java läuft auf jeder Plattform mit einer Java Virtual Machine (JVM)
- **Objektorientiert** – Daten und Methoden werden in Klassen zusammengefasst
- **Typsicher** – jeder Wert hat einen festen [[Java/Datentypen|Datentyp]]
- **Automatische Speicherverwaltung** – Garbage Collector räumt nicht mehr benötigten Speicher auf

# Ablauf
```
Quellcode (.java)
    → javac (Compiler)
    → Bytecode (.class)
    → JVM (Java Virtual Machine)
    → Ausführung
```

# Grundstruktur eines Java-Programms
```java
public class Klassenname {
    public static void main(String[] args) {
        // Hier steht der Code
    }
}
```

Jedes ausführbare Java-Programm benötigt eine `main`-Methode – sie ist der Einstiegspunkt und folgt dem [[Systemdenken/EVA-Prinzip|EVA-Prinzip]].

# Themen in Java
- [[Java/Datentypen|Datentypen]] – `int`, `double`, `boolean`, `char`
- [[Java/Variablen und Konstanten|Variablen und Konstanten]] – Werte speichern
- [[Java/Operatoren|Operatoren]] – Rechnen und Vergleichen
- [[Java/Steuerzeichen|Steuerzeichen]] – Text formatieren
- [[Java/Beispiele/PizzaBerechnung|Beispiele]] – komplette Programme
