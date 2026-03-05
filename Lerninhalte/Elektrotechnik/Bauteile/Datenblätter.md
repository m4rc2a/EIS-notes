---
classification: public
---

Ein **Datenblatt** (auch englisch _datasheet_) ist ein **technisches Dokument des Herstellers**, das ein [[Bauteil]] oder Produkt eindeutig beschreibt und alle **relevanten technischen [[Kennwerte]] und Bedingungen** liefert, damit du es **korrekt auswählen, auslegen und sicher betreiben** kannst.

> [!attention] Wichtig:
> Ein **Datenblatt** ist **keine** Anleitung für Schaltungen, sondern eine **Spezifikation**
# Inhalte
In Datenblätter werden ganz unterschiedliche dinge beschrieben u. A.:
- **Funktion & Beschreibung** (was es ist, wofür gedacht)
- **Pinbelegung / Anschlussbilder**, interne Blockschaltbilder
- **Grenzwerte** (_Absolute Maximum Ratings_: was nicht überschritten werden darf)
- **Empfohlene Betriebsbedingungen** (_Recommended Operating Conditions_)
- **Elektrische [[Kennwerte]]**
- **Timing-/Schaltkennwerte** (z. B. Verzögerungszeiten, Bandbreite)
- **Thermische Daten** (z. B. Verlustleistung, $R_{\theta JA}$​)
- **Typische Applikationen** und Messbedingungen (_Test Conditions_)
# Suchbegriffe
Wenn du im PDF suchst (Strg+F), funktionieren diese Begriffe sehr gut:

- **VIH​** / **VIL​** (Eingangs-HIGH/LOW)
- **VOH​** / **VOL​** (Ausgangs-HIGH/LOW)
- **“Recommended operating”**
- **“Electrical characteristics”** / **“DC characteristics”**
- **“Switching characteristics”** / **“AC characteristics”**
- **“Absolute maximum”**
- **“Input leakage”** / **IIN​**
- **“Supply current”** / **ICC​**
- **“Threshold”** (bei Schmitt-Triggern: VT​+, VT​−)
- **“Test conditions”** (entscheidend, um Zahlen richtig zu interpretieren)
# garantiert vs. typisch
- **Min/Max** in Tabellen = meist **garantiert** (unter den genannten Bedingungen).
- **Typical** (typ.) und Kurven = gut für Gefühl/Optimierung, aber nicht als harte Spezifikation.
# Bedingungen
Fast jede Zahl gilt nur bei:

- bestimmtem VCC​ (z. B. 4.5–5.5 V),
- bestimmter Temperatur (z. B. −40∘C…85∘C),
- bestimmter Last (z. B. IO​=8 mA),
- bestimmter Frequenz / Messaufbau.

> [!tldr] Merksatz
> Erst Test Conditions lesen, dann den Wert glauben.


# Bauteilklassen
Bei unterschiedlichen Bauteilklassen sind unterschiedliche werte wichtig:
- **Logik (74HC/74HCT/74LVC):** Pegel $V_{IH​}$/$V_{IL}$​, Fanout, $V_{OH​}$/$V_{OL}$​, Timing.
- **Analog-Schalter/MUX:** RON​, Leckströme, Bandbreite, Charge injection, Signalbereich.
- **Regler/Power:** Dropout, Quiescent current, Thermal, Stability/Capacitor requirements.
- **Transceiver/Interface:** Compliance (z. B. CAN/LIN/RS-485), [[Elektrostatische Entladungen|ESD]], Common-mode.
# typische Fallen
- **Absolute Maximum** mit Operating verwechseln
- Kurven als garantiert annehmen
- Package/Pin-Variante übersehen (gleicher Name, anderer Footprint/Pinout)
- **Falsche Variante erwischt**: gleiches [[Bauteil]], aber anderes Suffix/Gehäuse/Temperaturbereich/Footprint/Pinout
- **Wert aus der falschen Spalte**: z. B. “typ” statt “max” (oder umgekehrt)
- **Bedingungen übersehen**: Werte gelten oft nur bei z. B. ($V_{CC}=5,V$), ($T=25^\circ C$), bestimmter Last, bestimmter Frequenz
- **Pinbelegung/Gehäuse**: SOIC vs TSSOP vs QFN – Pin 1 Marker und Pin-Nummerierung.
# Checkliste
- [ ] **[[Bauteil]] eindeutig identifizieren**  
    Vollständige Typnummer + Gehäuse + ggf. Hersteller. (Notfalls vom Aufdruck + Stückliste ableiten.)
- [ ] **Im Datenblatt zur richtigen Stelle springen**  
    Nutze Inhaltsverzeichnis/Bookmarks + Suche (`Ctrl+F`) nach dem Parameterkürzel: z. B. #TODO
- [ ] **Kontext prüfen (3 Checks)**
    - Gilt das im **richtigen Abschnitt**? (Operating vs Absolute Max)
    - Stimmen **Bedingungen** ([[Spannung]], Temperatur, Last)?
    - Nimmst du **min/typ/max**, was die Aufgabe verlangt?
	- schaue dir an [[#typische Fallen]]
- [ ] In PDFs mit Highlighter Funktion arbeiten (für Praxisteil der [[Abschlussprüfung Teil 1|ApT-1]] eher nicht relevant):
- [ ] **Wert mit Einheit notieren + Quelle markieren**  
    Schreib:
    - Wert
    - **Einheit (nicht vergessen)**
- [ ] **Plausibilitätscheck (10‑Sekunden‑Check)**  
    Kurz überlegen: “Ist das realistisch?” (z. B. Pull‑Up $10\,\Omega$ wäre auffällig, Gate‑Charge von $200\,\text{nC}$ bei kleinem [[MOSFET]] auch.)

# Übung

## A) “5‑Werte‑Sprint” (10 Minuten)
Nimm 1 Datenblatt (z. B. 7805, LM358, 2N2222/BC547, IRLZ44N o. ä.) und such **5 typische Werte**:

- Versorgung/Operating Range
- Max. Strom/Output
- Verlustleistung/thermischer [[Widerstand]]
- Pinout
- 1–2 elektrische [[Kennwerte]] (z. B. $V_{CE(sat)}$, $R_{DS(on)}$, Offset, Ripple)

Stoppuhr an. Ziel: erst richtig, dann schneller.

## Fehlerliste führen
Jedes Mal, wenn ein Wert falsch war, notierst du **warum** (z. B. "typ statt max", "falsches Gehäuse").  
Nach 1–2 Wochen siehst du ein Muster und kannst es gezielt abstellen.