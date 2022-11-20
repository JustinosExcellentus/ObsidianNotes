---
aliases: [Taylorpolynom]

tags:
- Numerik_I
---

Die Operation von 2 Maschinenzahlen ergeben nicht zwingend eine Maschinenzahl

Exakte Arithmetik -> Gleitpunktarithmetik (Pseudoarithmetik)


Fehler gilt für Maschinenzahlen


Grundlegende Arithmetik gelten im Allgemeinen nicht mehr auf dem Rechner (Kommuntativgesetz, Distributivgesetz etc.)
Besonders durch die schlechte Konditionierung der Subtraktion für gleich große Maschinenzahlen ist dr Fehler groß

Für ( \*, /) ist krel \leq 1
Für (+-) ist krel >> 1 , wenn |xoy| << max{|x|, |y|}
Sehr große Fehlerverstärkung möglisch bei +,- (Auslöschung)


a^100; b = a+ 2^47; b-a = 0

a = 2^100 ? 1.2 10^30
eps = 1.2 10^30  mal 2.2 10^^-16 = 5.3 10^14

Keine Maschinenzahl zwischen 2^100 und 2^100 + 2 ^47