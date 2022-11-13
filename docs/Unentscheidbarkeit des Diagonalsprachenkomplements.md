---
aliases: [Diagonalsprache, Diagonalsprachenkomplement, Unentscheidbarkeit]

tags:
- Berechenbarkeit_Und_Komplexitaet
---
Das Komplement der Diagonalsprache ist

D = {w $\in$ {0,1}$^{*}$} $\mid$ w = $w_{i}$ und $M_{i}$ akzeptiert w}

Das Komplement ist unentscheidbar

Es existiere eine  TM, die das Komplement entscheidet
Hält auf jeder Eingabe an wenn $w \in \bar{D}$

Wir konstriueren eine TM M, die das als Unterprogramm verwendet. M auf der Eingabe und negiert die Ausgabe $\bar{M}$ 
Die TM M entscheidet nun offensichtlich D. Ein Widerspruch zur Unentscheidbarkeit von D.



## Unterprogrammtechnik zum Beweis von Unentscheidbarkeit


Um nachzuweisen, dass eine Sprache L unentscheidbar ist, genügt, es zu zeigen, dass man durch Unterprogrammaufruf einer TM $M_{L}$, die L entscheidet, eine andere Sorache L' entscheiden kann, von der bereits bewiesen wurde, dass sie unentscheidbar ist