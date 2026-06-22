---
aliases:
  - Escape-Sequenzen
  - Escape Sequences
  - Steuerzeichen
tags:
  - LF8
  - LF8-Klausur
classification: public
---
**Steuerzeichen** (Escape-Sequenzen) sind spezielle Zeichenkombinationen in Text-Strings, die nicht als Text dargestellt, sondern als Steuerbefehl interpretiert werden.

# Wichtige Steuerzeichen in Java

| Zeichen | Bedeutung | Effekt |
| ------- | --------- | ------ |
| `\n` | newline | Zeilenumbruch |
| `\t` | tab | Tabulator (Einrückung) |
| `\\` | backslash | Ein einzelner Backslash `\` |
| `\"` | double quote | Anführungszeichen im String |

# Beispiele

```java
System.out.println("Zeile 1\nZeile 2");
// Ausgabe:
// Zeile 1
// Zeile 2

System.out.println("Wert:\t42");
// Ausgabe: Wert:	42

System.out.println("Er sagte: \"Hallo\"");
// Ausgabe: Er sagte: "Hallo"
```

Steuerzeichen werden häufig in der [[../Benutzereingabe|Ausgabe]] von Programmen verwendet, um die Darstellung zu formatieren – siehe [[Beispiele/PizzaBerechnung|PizzaBerechnung]].
