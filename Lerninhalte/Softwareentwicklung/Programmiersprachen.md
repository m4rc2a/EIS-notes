---
aliases:
  - Programmiersprache
  - Compiler
  - Interpreter
  - Hochsprache
tags:
  - LF8
  - LF8-Klausur
classification: public
---
Eine **Programmiersprache** ist eine formale Sprache, mit der Menschen Anweisungen für einen Computer formulieren können. Sie bildet die Brücke zwischen menschlichem Denken und maschinenlesbarem Code.

# Kategorien

## Nach Abstraktionsgrad
- **Maschinensprache** – Binärcode (Nullen und Einsen), direkt vom Prozessor ausführbar
- **Assembler** – menschenlesbare Kurzbefehle, die 1:1 in Maschinensprache übersetzt werden
- **Höhere Programmiersprachen** – abstrahieren von der Hardware ([[Java]], C, Python)

## Nach Übersetzungsverfahren
- **Compiliert** – Quellcode wird vor der Ausführung komplett in Maschinensprache übersetzt (C, C++)
- **Interpretiert** – Code wird zur Laufzeit Zeile für Zeile ausgeführt (Python, JavaScript)
- **Just-in-Time (JIT)** – Mischform: Code wird in Zwischencode übersetzt und bei Bedarf compiliert ([[Java]])

# Beispiele

| Sprache | Typ | Einsatzgebiet |
| ------- | --- | ------------- |
| [[Java]] | Compiliert + JIT | Unternehmenssoftware, Android |
| C | Compiliert | Betriebssysteme, Embedded |
| Python | Interpretiert | Datenanalyse, KI, Skripte |
| JavaScript | Interpretiert | Webentwicklung |

# Vom Quellcode zum Programm

```
Quellcode (.java)
    → Compiler (javac)
    → Bytecode (.class)
    → JVM (Just-in-Time Compiler)
    → Maschinencode
```

Dieser Prozess wird in der [[Java|Java]]-Einführung näher erklärt. Die [[Software|Software]]-Entwicklung nutzt Programmiersprachen, um [[Systemdenken/EVA-Prinzip|EVA-Prinzipien]] in lauffähige Programme umzusetzen.
