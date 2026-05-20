---
aliases:
  - Voltage Independent USV
  - Line-Interactive-USV
  - VI-USV
tags:
  - ApT-1-2025
classification: public
---
Eine **[[VI-USVs|VI-USV]]** (auch **Line-Interactive-USV**) ist eine [[USVs|USV]], die im Normalbetrieb die Netzspannung durch einen automatischen Spannungsregler (AVR) stabilisiert.

# Funktionsweise
## Im Normalbetrieb
Die angeschlossenen Geräte werden aus dem Stromnetz versorgt, aber die [[USVs|USV]] reguliert Spannungsschwankungen automatisch nach (z. B. bei Unter- oder Überspannung).

## Bei Störungen
Bei einem Stromausfall schaltet die [[USVs|USV]] auf die interne Batterie um – typisch innerhalb von 2–4 ms.

# Merkmale
- Automatischer Spannungsausgleich (AVR), ohne auf Batterie zu wechseln
- Umschaltzeit auf Batterie: ca. 2–4 ms
- Besserer Schutz als [[VFD-USVs|VFD-USV]], aber nicht komplett entkoppelt vom Netz
- Typischer Einsatz: Server, professionelle IT-Umgebungen
