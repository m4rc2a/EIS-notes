---
aliases:
  - Z-Diode
classification: public
---
Eine [[Zener-Diode]] (auch [[Zener-Diode|Z-Diode]] genannt) ist eine besondere Art von [[Dioden|Diode]], welche für die Spannungsbegrenzung oder -stabilisierung eingesetzt wird.

> [!NOTE] Begriffszusammensetzung
**[Clarence Zener](https://de.wikipedia.org/wiki/Clarence_Melvin_Zener)** entdeckte in den 1930er Jahren den physikalischen Effekt, bei dem eine [[Dioden|Diode]] in Sperrrichtung plötzlich [[Stromstärke]] leitet, wenn eine bestimmte [[Spannung]] (die "Zenerspannung") überschritten wird. Dieser Effekt heißt **Zener-Effekt**. Daher der Name.
# Symbol
Das Schaltzeichen der [[Zener-Diode|Z-Diode]] sieht aus wie das einer Standarddiode, hat aber zusätzlich an der Spitze kleine Knicke oder "Häkchen" (als Unterscheidungsmerkmal).
![[D_Zener.svg]]
# Spannungsbegrenzung
Eine [[Zener-Diode]] kann u. A. auch dafür benützt werden, [[Spannung]] zu begrenzen.
- Dafür muss die [[Zener-Diode]] in Sperrrichtung ("rückwärts") eingebaut werden.
- Wenn die anliegende [[Spannung]] unterhalb der so genannten Zenerspannung liegt, passiert nichts
- Wenn aber die richtige [[Spannung]] erreicht wurde fängt die [[Dioden|Diode]] an zu leiten
- Die [[Spannung]] bleibt dann nahezu konstant auf Höhe der Zenerspannung.
- Ein [[Widerstand]] in Reihe ist notwendig, um die [[Stromstärke]] zu begrenzen.

# Spannungsstabilisierung
Bei der Spannungsstabilisierung wird die [[Zener-Diode]] parallel zum Verbraucher geschaltet.
- Schwankt die Eingangsspannung, ändert sich hauptsächlich die [[Stromstärke]] durch die [[Zener-Diode]].
- Die [[Spannung]] am Verbraucher bleibt nahezu konstant.
- Voraussetzung: Die Eingangsspannung muss größer sein als die Zenerspannung.
- Auch hier ist ein Vorwiderstand erforderlich.
-> Die [[Zener-Diode]] wirkt somit wie eine einfache Spannungsreferenz.

# Variablen

# Bauteilabhäng

_(stehen im Datenblatt – abhängig vom konkreten Z-Dioden-Typ)_

- Zenerspannung (auch: Durchbruchsspannung) **$U_Z$
- **$I_{Z,\min}$**
    
    - Minimaler Zenerstrom
    - nötig für stabile Spannungsregelung
- **$I_{Z,\max}$**
    
    - Maximal zulässiger Zenerstrom
    - darf nicht überschritten werden
- **$P_\text{tot}$** bzw. **$P_Z$**
    
    - Maximale Verlustleistung der Z-Diode
    - z. B. 0,25 W / 0,5 W / 1 W
- **$r_Z$**
    
    - Dynamischer Innenwiderstand im Durchbruchbereich
    - beeinflusst Spannungsgenauigkeit
- **$\alpha_T$**
    
    - [[Temperaturkoeffizient]] der Zenerspannung
    - < 5 V → negativ
    - > 6 V → positiv
        
- **$I_R$**
    
    - Sperrstrom unterhalb von $U_Z$
    - meist im µA-Bereich
- **$U_F$**
    
    - Durchlassspannung (in Vorwärtsrichtung)
    - ca. 0,7 V bei Silizium

---

# 2️⃣ Schaltungs- / Berechnungsvariablen

_(abhängig von der konkreten Schaltung)_

- **$U_E$**
    
    - Eingangsspannung
- **$U_A$**
    
    - Ausgangsspannung
    - näherungsweise $U_A \approx U_Z$
- **$R_V$**
    
    - Vorwiderstand zur Strombegrenzung
- **$I_Z$**
    
    - Tatsächlicher Zenerstrom
- **$I_L$**
    
    - Laststrom (Verbraucher)
- **$I_\text{ges}$**
    
    - Gesamtstrom durch den Vorwiderstand
    - $I_\text{ges} = I_Z + I_L$
- **$P_Z$**
    
    - Tatsächliche Verlustleistung
    - $P_Z = U_Z \cdot I_Z$
