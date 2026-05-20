---
classification: public
---

# Fremdnetz
Ein **Fremdnetz** (auch _remote network_) ist ein Netzwerk, das sich außerhalb des eigenen (lokalen) Netzwerks befindet und nur über einen Router erreichbar ist.

- Im eigenen Subnetz → Ziel-MAC-Adresse = MAC des Endgeräts
- Im Fremdnetz → Ziel-MAC-Adresse = MAC des Default-Gateways (Routers)

# Payload
Die **Payload** (Nutzdaten) ist der Teil eines Datenpakets, der die eigentlichen Informationen enthält – ohne Header/Trailer.

# MAC-Adresstabelle
In die MAC-Adresstabelle eines Switches werden **nur Quell- (SRC-)MAC-Adressen** eingetragen, die er auf seinen Ports sieht. Die Ziel-MAC (DST) wird zum Weiterleiten verwendet, aber nicht gelernt.


```bash
arp -a
```