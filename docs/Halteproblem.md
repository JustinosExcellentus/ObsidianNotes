---
aliases: [Unentscheidbarkeit]

tags:
- Berechenbarkeit_Und_Komplexitaet
---

Beim Halteproblem geht es darum, zu entscheiden, obe ein Programm mit einer gegeben Eingabe terminiert.

In der Notation der TMen ergibt sich

H = {(M)w |M hält auf w}


Diagonalsprache D= {$w \in (0,1)^{*}$  | w = wi, und Mi akzeptiert nicht}

Die Diagonalsprache D ist nicht entscheidbar


Aij = {1, falls Mi das Wort wj akzeptiert}

"Diagonalsprachenmatrix "




Beweis:

Sei D entscheidbar, dann existiere eine TM 
Wir starten die TM Mi mit der Eingabe wj. Es ergeben sich zwei Fälle, die jeweils direkt zum Widerspruch führen

wi \in D \rightarrow Mi akzeptiert wi => wj \not in D

Widerspruchsbeweis Menge aller Mengen

=> Somit ist D unentscheidbar



Das 



Sei $M_{H}$ eine TM, die H entscheidet, also eine TM die auf jeder Eingabe hält und nur Eingaben der Form $<M>$ w akzeptiert, bei denen M auf w hält.

Wir konstruieren eine TM $M_{\bar{D}}$  mit $M_{H}$ als Unterprogramm, die  $\bar{D}$ entscheidet, was aber unentscheidbar ist.


Algorithmus der TM  $M_{\bar{D}}$  mit Unterprogramm $M_{H}$ 

1) Auf Eingabe w berechne i mit w =$w_{i}$ (Prüfung der Gödelnummer)
Wenn es keine Gödelnummer ist, dann wird es verworfen


$w_{i}$ ist  die Gödelnummer der i.ten TM, also $<M_{i}> = w$.
Jetzt starte $M_{H}$  als Unterprogramm mit Eingabe $<M_{i}> = w$ .

Falls $M_{H}$  akzeptiert, so simuliere das Verhalten $M_{i}$ auf w (genau wie die universelle TM U dies tun würde)

Falls $M_{H}$ verwirft, so verwirf die Eingabe.


Man zeige dass  $M_{\bar{D}}$ korrekt arbeitet


1. w in D- | Mi akzeptiert wi
=> Mh und U akzeptieren <Mi> wi



2. w nich in D- | Mi akzeptiert wi nicht
Mi halt nicht auf wi oder Mi verwirft wi
Mh verwirft <Mi> wi oder Mh akzeptiert und U verwirft <Mi> wi




Das spezielle Halteproblem ist definiert als

Heps = {<M> | M haält auf Eingabe eps}
Neps = {wi | Mi hält auf Eingabe eps}

Wir nutzen wieder Unteprogrammtechnik



Die TM Mh mit Unterprogramm Meps arbeitet wie folgt