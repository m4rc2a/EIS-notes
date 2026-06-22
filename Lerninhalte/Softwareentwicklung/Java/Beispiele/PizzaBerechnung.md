---
aliases:
  - Pizza-Aufgabe
  - Pizza Aufgabe
  - Pizza Berechnung
tags:
  - LF8
  - LF8-Klausur
classification: public
---
Die **PizzaBerechnung** ist ein Java-Programm, das den Gesamtpreis einer Pizza berechnet. Sie zeigt das [[Systemdenken/EVA-Prinzip|EVA-Prinzip]] mit [[../Variablen und Konstanten|Konstanten]] (`final`) und [[../Variablen und Konstanten|Variablen]].

```java
public class PizzaAufgabe {

    public static void main(String[] args) {
        final double GRUNDPREIS_PIZZA = 5.50;
        final double PREIS_PRO_BELAG = 0.75;

        // E – Eingabe
        int anzahlBelag = InOut.readInt("Wie viele Beläge wollen Sie haben?\t");

        // V – Verarbeitung
        double belagPreisGesamt = anzahlBelag * PREIS_PRO_BELAG;
        double gesamtPreis = belagPreisGesamt + GRUNDPREIS_PIZZA;

        // A – Ausgabe
        System.out.println("\n\nGesamtpreis:\t" + gesamtPreis);
    }
}
```

# Verwendete Konzepte
- [[../Variablen und Konstanten|Konstanten]] (`final`) für feste Preise
- [[../Variablen und Konstanten|Variablen]] für Zwischenergebnisse
- [[../Steuerzeichen|Steuerzeichen]] (`\t`, `\n`) für formatierte Ausgabe
- [[../.../Benutzereingabe|Benutzereingabe]] mit `InOut.readInt()`
- [[../Operatoren|Operatoren]] für Multiplikation und Addition
