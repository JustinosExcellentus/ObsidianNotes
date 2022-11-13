---
aliases: [Algebra]

tags:
- Analysis_fuer_Informatik
---

Abzählbarkeit bezeichnet die Anzahl der Elemente, die in einer Menge liegt. ($\vert A \vert$ Mächtigkeit)


#### Definition:

1) Zwei Mengen A, B heißen gleichmächtig, falls es eine bijektive Abbildung $f: A \rightarrow B$ gibt.
2) Eine Menge A heißt abzählbar unendlich, falls sie zu $\mathbb{N}$ gleichmächtig ist, also ein bijektives $f : A \rightarrow \mathbb{N}$ existiert.


#### Satz: $\mathbb{Z}$ und $\mathbb{Q}$ sind abzählbar unendlich.

Beweis: zu $\mathbb{Z}$ . Wir schreiben  
$\mathbb{Z}$ = $\{ 0, -1, 1, -2, 2, -3, 3, -4, 4, .......\}$  
$\mathbb{N}$ = $\{ 1,2,3,4,5,6,7,8,9,......\}$ 
Wir können somit eine bijektive Abbildung $f()$

zu $\mathbb{Q}$ mit a = p/q

$$x = \left ( \begin{matrix} q\vert p & 1 &2 & 3 & 4\\ 1 & \frac{1}{1} & \frac{2}{1} &\frac{3}{1} &\frac{4}{1} \\ 2 & \frac{1}{2} & \frac{2}{2} &\frac{3}{2} &\frac{4}{2}\\ 3 & \frac{1}{3} & \frac{2}{3} &\frac{3}{3} &\frac{4}{3}\\4 & \frac{1}{4} & \frac{2}{4} &\frac{3}{4} &\frac{4}{4}
\end{matrix} \right ) \Rightarrow \left ( \begin{matrix} q\vert p & \mid1 &2 & 3 & 4\\ \hline   1 & \mid 1 & 3 &4 & 10\\ 2 & \mid 2 & 5 & 9 & 11\\ 3 & \mid 6 & 8 & 12 & 15\\4 & \mid 7 & 13 & 14 & 16
\end{matrix} \right )$$

$\mathbb{Q}$  ist somit abzählbar.



#### Satz: $\mathbb{R}$  ist nicht abzählbar unendlich

Beweis: (Diagonalverfahren nach Cantor) Wir zeigen, dass das offene Intervall (0,1) nicht abzählbar unendlich ist.

Annahme: R ist abzählbar unendlich, das heißt also ein bijektives $f : \mathbb{R} \rightarrow \mathbb{N}$ existiert, Also gibt es eine Tabelle N -> (0,1)
a $\leq \mathbb{R}$ in Dezimaldarstellung, Ziffern (0,1,2,3,...,9)


Es existiert ein 0,c1c2c3c4 ...., dass  sich in der n.ten Nachkommastelle mit der n.ten  Zahl der Menge unterscheidet. Also haben wir eine Zahl die zwischen 0 un 1 liegt, die nicht in der Tabelle liegt. Würden wir sie der Tabelle hinzufügen, so können wir eine neue Zahl konstruieren, die ebenfalls zwischen 0 und 1 ist und nicht in der Liste ist.


##### Bemerkung

1) $\mathbb{R}$ ist überabzählbar. Es enthält "mehr" Elemente als $\mathbb{N}$ .
2) $\vert \mathbb{R} \vert \neq \infty$ ,  $\vert \mathbb{R} \vert = \aleph_{1}, \infty = \aleph _{0}$
3) Die Menge A = $\{ f \vert f$ Abbildung von $[0,1] \rightarrow [0,1]\}$ ist mächtiger als $\mathbb{R}$ 
4) Die Mengen $\mathbb{R}, \mathbb{R} \times \mathbb{R}, \mathbb{R} \times \mathbb{R} \times \mathbb{R}$ sind alle gleich mächtig.


##### Komplexe Zahlen
Körper ohne Ordnung => Kein direkter Vergleich der Eemente
$(a,b) \in \mathbb{R} \times \mathbb{R}$ 
$(a,b) + (c,d) = (a +c, b + d)$ Neutrales Element (0,0)
$(a,b) \cdot + (c,d) = (ac -bd) (ad + bc)$ Neutrales Element (1, 0), inverse Element (a,b) = a/a2+b2 , -b/a2+b2


##### Potenzmengen

Potenzmenge P(N), die Menge aller Teilmengen von N
P(N) ist überabzählbar.

Beweis: Matrix stellt die Elemente der Menge Sj dar.
Diagonalargument => Eine Menge =>
[Noch einzufügen]