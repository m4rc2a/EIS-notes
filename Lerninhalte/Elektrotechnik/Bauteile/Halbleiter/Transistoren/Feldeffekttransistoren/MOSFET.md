---
classification: public
---


Der **[[MOSFET]] (Metall-Oxid-Halbleiter-Feldeffekttransistor)** ist der meistverwendete FET-Typ und ein Grundbaustein aller modernen Computerchips.

# Funktionsweise

Das Gate ist isoliert (meit durch Siliziumdioxid). Wird eine [[Spannung]] am Gate angelegt, bildet sich im [[Halbleiter]] ein leitender Kanal zwischen Source und Drain. Der Hauptvorteil: Am Gate fließt praktisch kein [[Stromstärke]] – ideal für schnelle, stromsparende Schaltungen!

# Symbol
![[IRLIZ44N.svg]]

# Typen
- **n-MOS:** leitet bei positiver Gatespannung
- **p-MOS:** leitet bei negativer Gatespannung


> [!Merke]
> MOSFETs sind die Grundlage für digitale Elektronik – von Speicher, Logikbausteinen bis hin zu Prozessoren.
# FET – Was muss ich berechnen können? (Checkliste)

## Gleichstrom (DC) – 6.6.1
1) Gleichstromleistung
- Formel: $P = U_{DS}\cdot I_D$
- Umstellen: $I_D = \frac{P}{U_{DS}}$, $U_{DS} = \frac{P}{I_D}$

2) Eingangswiderstand aus Gate-Leckstrom
- Formel: $R_{GS}=\frac{U_{GS}}{I_{GSS}}$

3) Kennlinienwerte/Begriffe ablesen/verstehen
- $I_{DSS}$ bei $U_{GS}=0$
- $U_{GS(\mathrm{OFF})}$ (Abschnür-/Sperrspannung)
- $U_{DS\mathrm{sat}}$ (Übergang in Abschnürbereich/Sättigung)

## Wechselstrom/Kleinsignal – 6.6.2
1) Steilheit (Transkonduktanz)
- Bei konstantem $U_{DS}$: $S=\frac{\Delta I_D}{\Delta U_{GS}}$
- Umstellen: $\Delta I_D = S\cdot \Delta U_{GS}$, $\Delta U_{GS}=\frac{\Delta I_D}{S}$

2) Ausgangswiderstand
- Bei konstantem $U_{GS}$: $r_{DS}\approx \frac{\Delta U_{DS}}{\Delta I_D}$
- Umstellen: $\Delta I_D \approx \frac{\Delta U_{DS}}{r_{DS}}$

3) Kombinierte Änderungsaufgaben (typisch)
- Schritt 1: Aus $(\Delta U_{DS}, \Delta I_D)$ den $r_{DS}$ bestimmen
- Schritt 2: Aus benötigtem $(\Delta I_D, \Delta U_{GS})$ die Steilheit $S$ bestimmen
- Ziel häufig: $I_D$ nach einer $U_{DS}$-Änderung durch passende $U_{GS}$-Änderung wieder auf den Ausgangswert bringen

---

## Aus Kennlinien (Diagrammen) ablesen
7) Arbeitspunkt bestimmen
- gegeben z.B. $U_{DS}$ und $I_D$ $\rightarrow$ passendes $U_{GS}$ aus Kennlinien ablesen

8) Lokale Kleinsignalwerte aus Kennlinien
- $S$ lokal aus $I_D$-$U_{GS}$ bei konstantem $U_{DS}$
- $r_{DS}$ lokal aus $I_D$-$U_{DS}$ bei konstantem $U_{GS}$