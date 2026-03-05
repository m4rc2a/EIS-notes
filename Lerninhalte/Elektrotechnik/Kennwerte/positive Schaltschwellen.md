---
aliases:
  - VT+
  - V_Tplus
  - positive Schaltschwelle
  - positive Trigger-Schwelle
  - Positive-going threshold voltage
  - Positive threshold voltage
  - Upper threshold voltage
  - obere Schaltschwelle
  - Rising threshold
  - Positive-going input threshold
  - Positive-going trip point
  - Input threshold
tags:
  - elektronik
  - digitaltechnik
  - schmitt-trigger
  - datenblatt
classification: public
---
Die **positive Schaltschwelle** **$V_{T+}$** (auch: **Positive-going threshold voltage**) ist eine **Schaltschwelle** eines Eingangs mit **Hysterese** (typisch für: **Schmitt-Trigger**).  
Sie gibt die **Eingangsspannung beim Ansteigen** an, **ab der** der Ausgang **umschaltet**.

> [!tldr] Kurzgesagt
$V_{T+}$ -> **Umschaltspannung bei steigender Eingangsspannung** (bei Schmitt-Trigger/Hysterese).

# Kontext
- Schmitt-Trigger-Inverter / -Buffer
- Komparatoren mit Hysterese
- Eingänge mit entprellter/rauschfester Schaltschwelle

In Datenblättern wird \(V_{T+}\) oft zusammen mit **\(V_{T-}\)** angegeben.

## Abgrenzung
- **$V_{T+}$**: Umschaltpunkt bei **steigendem** Eingangssignal (LOW → HIGH am Eingang)
- **$V_{T-}$**: Umschaltpunkt bei **fallendem** Eingangssignal (HIGH → LOW am Eingang)
- **$V_{IH}$/$V_{IL}$**: Logikpegel-Grenzen bei *normalen* Digitaleingängen (meist ohne definierte Hysterese)

## Hysterese (wichtiges Konzept)
Die **Hysterese** ist der Abstand zwischen den beiden Umschaltpunkten:

$$
V_H = V_{T+} - V_{T-}
$$

Je größer \(V_H\), desto besser ist die Stör-/Rauschunterdrückung rund um den Schaltpunkt.

## Praktische Bedeutung
- Erhöht **Störfestigkeit** bei langsamen Flanken oder verrauschten [[elektrische Signale|Signalen]]
- Hilft bei **Entprellung** von Tastern (in Kombination mit RC/Signalformung)
- Stabilisiert [[elektrische Signale|Signale]] aus [[Sensoren]] oder langen Leitungen

## Typische Datenblatt-Angaben
$V_{T+}$ wird häufig spezifiziert als:
- **min / typ / max**
- abhängig von **Versorgung** $V_{CC}$ und **Temperatur**
- ggf. abhängig von **Bauteilfamilie** (z. B. CMOS, HCT, LV, etc.)

Beispiel-Form (ohne Zahlen) bei definiertem $V_{CC}$, $T_A$:
- $V_{T+,\min}$
- $V_{T+;\text{typ}}$
- $V_{T+,\max}$

