---
aliases:
  - Blutalkohol
  - Blutalkohol Aufgabe
  - Alkoholberechnung
  - Promilleberechnung
tags:
  - LF8
  - LF8-Klausur
classification: public
---
Die **BlutalkoholBerechnung** berechnet den Promillewert einer Person. Sie zeigt das [[Systemdenken/EVA-Prinzip|EVA-Prinzip]] mit mehreren [[../.../Benutzereingabe|Benutzereingaben]] und einer Berechnungsformel.

```java
public class BlutalkoholSchlechter {

    public static void main(String[] args) {
        // E – Eingabe
        double aufgenommenerAlkohol = InOut.readDouble(
            "Wie viel Alkohol wurde aufgenommen? Angabe in ml\t");
        double verteilungsFaktor = InOut.readDouble("Verteilungsfaktor?\t");
        int gewicht = InOut.readInt("Gewicht? Angabe in kg\t");
        double getraenkIndex = InOut.readDouble("Getränke Alkoholindex?\t");

        // V – Verarbeitung
        double aufgenommerAlkoholGramm =
            aufgenommenerAlkohol * getraenkIndex * 0.8;
        double promille =
            aufgenommerAlkoholGramm / (gewicht * verteilungsFaktor);

        // A – Ausgabe
        System.out.println("Promille: " + promille);
    }
}
```

# Verwendete Konzepte
- [[../Variablen und Konstanten|Variablen]] – Speichern von Zwischenergebnissen
- [[../.../Benutzereingabe|Benutzereingabe]] mit `InOut.readDouble()` und `InOut.readInt()`
- [[../Operatoren|Operatoren]] – Multiplikation, Division, Klammerung
- [[../Datentypen|Datentypen]] – `double` und `int`
- [[Systemdenken/EVA-Prinzip|EVA-Prinzip]] – klare Trennung in Eingabe, Verarbeitung, Ausgabe

# Zur Formel

```
Promille = (Alkoholmenge in ml × Getränkeindex × 0,8) / (Gewicht in kg × Verteilungsfaktor)
```

Der Verteilungsfaktor ist abhängig vom Geschlecht (Mann: ~0,7, Frau: ~0,6).
