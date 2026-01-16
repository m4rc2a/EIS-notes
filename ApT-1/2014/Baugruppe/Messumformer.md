---
aliases:
  - das Temperaturerfassungsmodul
  - das Erfassungsmodul
  - das Modul
  - der Umformer
  - Messumformmodul
  - Messumformungsmodul
---
# Begriffserklärung
Der [[Messumformer]] ist ein Temperaturerfassungsmodul aus der [[Abschlussprüfung Teil 1|ApT-1]] 
[[Messumformer|Das Modul]] verwendet nach beliebigen einen [[PT100|PT100]] bzw. einen [[PT1000|PT100]] Temperatur [[PT1000|Sensor]].

# Konstanten

| Eigenschaft                                                                                             | Wert               |
| ------------------------------------------------------------------------------------------------------- | ------------------ |
| konstanter [[PT100#Parameter\|Messstrom des PT100]] ($I_\text{Messung [[PT100]]}$) ^Messstrom100        | $1\,\mathrm{mA}$   |
| <br>konstanter [[PT1000#Parameter\|Messstrom des PT1000]] ($I_\text{Messung [[PT100]]}$) ^Messstrom1000 | $100\,\mathrm{µA}$ |
| [[Temperaturkoeffizient]] ($K_\text{U/T}$)                                                              | $10mV/K$           |
# Messprinzip
## Features
- [[Messumformer|Das Modul]] unterstützt nur [[PT100]]/[[PT1000]] [[PT100#^2draht|2-Drahtanschlüsse]] 
- [[Messumformer|Das Modul]] verwendet zur Messung das Prinzip des Spannungsfalls an einem Widerstand bei [[#^Messstrom1000|Messstrom]]. ^spannungsabfall
## Verfahren
- Die "minimale" [[#^spannungsabfall|Spannungsänderung]] wird in ein "technisch verwertbares Signal" umgewandelt.
	- dabei wird ein [[Koeffizient]] von $10 mV/K$ verwendet
	-> Spannung ist zwischen `-X2` und `-X3` abgreifbar
> **Hinweis:**
> Der richtige Temperatur [[PT1000|Sensor]] muss ausgewählt sein.
# [[PT1000|Sensor]] Auswahl
Der [[PT1000|Sensor]] lässt sich mit dem Stecker `-X7` auswählen
- `-X7-1` mit `-X7-2` für [[PT100|PT100]]
- `-X7-3` mit `-X7-2` für [[PT1000]]
