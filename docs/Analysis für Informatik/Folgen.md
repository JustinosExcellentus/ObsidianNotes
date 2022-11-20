---
aliases: []

tags:
- Analysis_fuer_Informatik
---



$\mathbb{N} \rightarrow \mathbb{R}$ : Folgen (a$_{n}$)$_{n \in \mathbb{N}}$ 

$lim_{n \rightarrow \infty} a_{n} = a$  $\Leftrightarrow$ an konvergiert gegen a
$\forall \varepsilon > 0$   $\exists \tilde{a}_{n} \in \mathbb{N}$ 

### Definition
Die $a_n\subset\mathbb{R}$ heißt beschränkt falls es ein S $\in \mathbb{R}$ , S $\geq$ 0 gibt mit $\vert a_n \vert \leq S, \forall n \in \mathbb{N}$


### Satz 
Jede konvergente Folge  $a_n\subset\mathbb{R}$ ist beschränkt.

### Beweis
Sei limes = a, d.h zum Beispiel für eps = 1 exists n eps in N  \mid \vert an - a \vert \leq eps \forall n > eps


a) gilt nicht beschränkt $\Rightarrow$ konvergiert

Beispiel an = $(-1)^n$ ist beschränkt, aber nicht konvergent
Beschränktheit ist notwendig, aber nicht hinreichend für Konvergenz


b) Unbeschränkte Folgen, die gegen $\pm \infty$ konvergieren heißen bestimmt divergent.
an = $(-1)^n$ ist unbestimmt divergent.

### Definition

- Eine reelle Folge $a_n\subset\mathbb{R}$ heißt monoton wachsend, falls $a_n \leq a_{n+1} \forall n \in \mathbb{N}$ 
- Eine reelle Folge $a_n\subset\mathbb{R}$ heißt monoton fallend, falls $a_n \geq a_{n+1} \forall n \in \mathbb{N}$ 
- Eine reelle Folge $a_n\subset\mathbb{R}$ heißt streng monoton wachsend, falls $a_n < a_{n+1} \forall n \in \mathbb{N}$ 
- Eine reelle Folge $a_n\subset\mathbb{R}$ heißt streng monoton fallend, falls $a_n > a_{n+1} \forall n \in \mathbb{N}$ 

### Satz:
Sei $a_n\subset\mathbb{R}$ eine monoton wachsende Folge. Falls aber $a_n$ beschränkt ist, so ist die Folge konvergent.

Beweis $A = \{a_n \mid a \in R \} \subset R$, es ist nach oben beschränkt $\Rightarrow$  Es ex. ein Supremum A = n
Wähle ein $\varepsilon$ > 0 beliebig, a ist Supremum, also gibt es ein neps in N mit aneps > an - eps. Da an monoton wächst, gilt a - eps < aneps \leq an für alle alle n \geq neps, aber auch \leq A, da A Supremum ist. d.h , A + eps <=> \vert A+eps \vert \leq eps.

Bemerkung: 

Beschränktheit + Monotonie ist hinreichend, aber nicht notwendig für Konvergenz.
$(-1 )^n \cdot 1/n$

b) Bild Zusammenfassung

Konvergente Folgen Teilmenge von Folgen, Teilmenge der beschränkten Folgen
Monotone Folgen Teilmenge der 
Fm und Fk = nicht leer
Beschränkte Folgen Teilmenge der Folgen


Def: (an) Teilmenge R heißt Cauchy - Folge wenn gilt
Forall epsilon eps exits schwelle in N 
forall n und m > neps, Abstand zwischen beliebigen Folgeglieder \leq epsilon

d.h ab der schwelle neps wird der abstanf beliebiger Folgenglieder beliebig klein (kleiner gleich als epsilon)


Beispiel $a_n = 1/(n+1) \mid \vert 1/(n+1) - 1/(m+1) \vert \leq epsilon$
setze m > n \rightarrow  \vert 1(n+1) 

Bemerkung: Cauchy-Folge ist eine Eigenschaft analog von Folgen analog zu Beschränktheit oder Monotonier

Satz: an teilmenge R ist konvergent genau dann, wenn die Folge eine Cauchy-Folge ist.

Beweis:

Konvergenz folgt Cauchy

...


Bemerkung Cauchy folgt Konvergenz, ist äquiv. zur Vollständigkeit der reellen Zahlen. Oft wird der Körper R definiert mit/über Cauchy-Folgen

Rechnen mit folgen

Satz: Seien an und bn konvergente Folgen mit Grenzwerten a und b. Dann gilt:
1) Der Grenzwert gegen unendlich von (aalpha + bbeta) = alpha a + beta b, alpha, beta in R
2) limes (an* bn) = a * b
3) limes ( 1/an) = 1/a
4) limes (\sqrt(an)) = \sqrt(an)

Beweis: Nachrechnen des Konvergenzkriteriums

Beispiel: 
a) an = /(2an^2+1)

