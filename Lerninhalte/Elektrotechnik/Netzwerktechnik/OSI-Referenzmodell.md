---
classification: public
---

# Schichten
1. **Bitübertragung**
   Physical
2. **Sicherungsschicht**
   _(Data Link)_
	1. LLC (Logic Link Control)
	2. MAC (Media Access Control)
3. **Vermittlungsschicht**
   _(Network)_
4. **Transportschicht**
## Anwendungsebene (TCP/IP)
5. **Sitzung** (Client <-> Server)
   _(Session)_
6. **Darstellung**
   _(Presentation)_
7. **Anwendung**
   _(Application)_

# Random [[Netzwerktechnik]] facts
- Es gibt immer Sender und Empfänger
- Ein IP Packet besteht aus ein Segment und anderen Dingen
- Ein IP Packet hat SRC (Source) und DST (Destenation)
- Das IP Packet kommt in ein Frame
- trailer (FCS) kommt dazu

# PDU (Protocol Data Unit)
Eine **PDU** (Protocol Data Unit) ist die Dateneinheit, die auf einer bestimmten OSI-Schicht ausgetauscht wird. Jede Schicht hat einen eigenen Namen für ihre PDU:

| Schicht | PDU-Bezeichnung |
|---|---|
| 1 – Bitübertragung | **Bit** |
| 2 – Sicherungsschicht | **Frame** |
| 3 – Vermittlungsschicht | **Packet** |
| 4 – Transportschicht | **Segment** (TCP) / **Datagram** (UDP) |
| 5–7 – Anwendungsebene | **Data** |

> [!tldr] Merksatz
> Eine PDU besteht immer aus: **Header** (Steuerdaten) + **Payload** (Nutzdaten) + ggf. **Trailer**