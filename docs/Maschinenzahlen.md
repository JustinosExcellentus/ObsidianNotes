
---
aliases: [Zahlendarstellung, Zahlen]

tags:
- Numerik_I
---

Normalisierte Gleitpunktdarstellung


x = $plusminus$ 0,d1,d2,dm*b^e

wobei Basis $b \in \mathbb{N} \setminus 1$ 
Exponent $e \in \mathbb{Z}$ mit $r \leq e  \leq R$
Mantisse f = plsm $
Mantissenlänge m
Normalisierung (d1 = 1)

Nur endliche Anzahl von Zahlen darstellbar

$\Rightarrow \mathbb{M}(b,m,r,R)$ 
Betragsmäßig kleinste bzw. größte Zahl in $\mathbb{M}$ 
xmin xmax


Reduktionsabbildung

fl(x) = .....

Die letzte Stelle der Mantisse wird um eins erhöht


Rür den relativen Rundungsfehler erhält man

$\mid \frac{fl(x)-x}{x} \mid \leq \frac{\frac{b^{-m}}{2}b^{e}}{b^{-1}b^{e}} =   \frac{b^{1-m}}{2}$ 

Die relative Maschinengenauigkeit
eps := $\frac{b^{1-m}}{2}$ 
charakterisiert das Auflösevermögen des Rechners,
eps = $inf \{ \delta > 0 \mid fl(1+\delta) > 1\}$ 


Der Rundungsfehler 
