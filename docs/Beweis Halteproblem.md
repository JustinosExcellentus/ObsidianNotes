---
aliases: [Halteproblem, Unberechenbarkeit]

tags:
- Berechenbarkeit_Und_Komplexitaet
---

Matrix


Angenommen: D ist entscheibar.
Dann existiert eine TM Mi, die D entscheidet, d.h Mi hält bei jeder Eingabe und

Mi akz. w, falls w in D
Mi verw. w, falls w nicht in D

Wir betrachten wi = <Mi>
1. Fall wi in D
=> Mi akz. wi => Aii = 1

Aber wi in D => (Definition von D) => Ai,i = 0
0 => Widerspruch


2.Fall wi nicht in D

=> Mi akz. wi nicht => Aii = 0
=> Aber wi nicht in D => Aii = 1


=> Widerspruch