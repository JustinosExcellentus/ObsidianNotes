
## Definition

Ein Monoid besteht aus:

- Einer Menge M
- Eine assoziative Verknüpfung $\circ$ auf M
- Ein neutrales Element e bezüglich $\circ$


## Spezialisierung von Monoiden

#### Abelsches Monoid

Ein Monoid heißt **abelsch** (oder kommutativ), wenn $\circ$ kommutativ ist.

#### Wortmonoid

- Die Menge A wird als **Alphabet** definiert (bspw. $A = \{ a,b,...,z\}$)
- Für $n \in \mathbb{N}$ und $a_1 , a_2 , ..., a_n \in A$ nennen wir $a_1 a_2... a_n$  ein **Wort** der Länge n über A .
- $A^{*} := \{ w \mid$ w ist Wort der Länge n über A, $n \in \mathbb{N}_0\}$ 
- $A^{*}$ enthält das Wort $\varepsilon$ der Länge 0
- Für 2 Wörter $v:= a_1 a _2 ... a_n$ und $w:= b_1 b_2 ... b_m$ über A sei
$v*w = a_1 a_2 ... a_n b_1 b_2 ... b_m$
die Verkettung oder **Konkatenation** von v und w
$\Rightarrow$ ($A^{*}$ , $*$) ist ein Monoid mit neutralem Element $\varepsilon$, das **Wortmonoid** über A


#### Abbildungsmonoid



Abbildung(M,M) ist Monoid mit Verknüpfung $(g,f) \rightarrow g \circ f$ 
und neutralem Element $id_M$ ,

##### Bemerkung

Sei M Menge und $f \in Abb(M,M)$.
- f besitzt Rechtsinverses $\Leftrightarrow$ f ist surjektiv.
- f besitzt Linksinverses $\Leftrightarrow$ f ist injektiv.
- f besitzt Inverses $\Leftrightarrow$ f ist bijektiv.

## Notation


- Multiplikation auf M:
$\Rightarrow \quad x \cdot y := x \circ y$ 
$\Rightarrow \quad x  y := x \circ y$ 



#### Axiome in Standardnotation:


##### Multiplikation
- Monoid M:
-- für $x,y,z \in M$ gilt: $\quad \quad x(yz) = (xy)z$ 
-- $\exists e \in M \mid \forall x \in M$: $\quad \quad ex = x = xe$ 

- Abelsches Monoid M:
-- für $x,y,z \in M$ gilt: $\quad \quad x(yz) = (xy)z$ 
-- $\exists e \in M \mid \forall x \in M$: $\quad \quad ex = x = xe$ 
-- für $x,y \in M$ gilt: $\quad \quad xy = yx$ 

##### Addition
- Monoid M:
-- für $x,y,z \in M$ gilt: $\quad \quad x+(y+z) = (x+y)+z$ 
-- $\exists e \in M \mid \forall x \in M$: $\quad \quad e+x = x = x+e$ 

- Abelsches Monoid M:
-- für $x,y,z \in M$ gilt: $\quad \quad x+(y+z) = (x+y)+z$ 
-- $\exists e \in M \mid \forall x \in M$: $\quad \quad e+x = x = x+e$ 
-- für $x,y \in M$ gilt: $\quad \quad x+y = y+x$ 






## Beispiele


- $\mathbb{N}$ mit üblicher Addition ist kein Monoid, da kein neutrales Element existiert.
- $\mathbb{N}$ mit üblicher Multiplikation ist ein Monoid, da das neutrale Element = 1 ist.
- $\mathbb{N}_0$ mit üblicher Addition ist ein Monoid, da das neutrale Element = 0 ist.
- $\mathbb{N}_0$ mit üblicher Multiplikation ist ein Monoid, da das neutrale Element = 1 ist.




## Invertierbarkeit


#### Definition

- Sei M ein Monoid, und sei $x \in M$
$\Rightarrow$ x invertierbar in M : es gibt ein inverses Element zu x bezüglich $\circ$ 
$\Rightarrow$ x invertierbar $\Leftrightarrow$     $\exists y \in M : \quad x \circ y = e = y \circ x$ 

- Inverse zu x in M: das zu x inverse Element y bezüglich $\circ$ .


- Menge der invertierbaren Elemente in M:
$M^{\times}$ = $\{ x \in M \mid x \: invertierbar\}$ 

- Notation: 
"$\cdot$" : M multiplikativ geschrieben, $x \in M$ invertierbar, $x^{-1}$ das Inverse von x
"$+$" : M additiv geschrieben, $x \in M$ invertierbar, $-x$ das Inverse von x.



#### Beispiele

- $(N_0 , \cdot)^{\times} = \{1 \}$ 
- 0 einziges invertierbares Element in $(N_0 , +)$ 


#### Proposition

M sei ein Monoid

- Besitzen $x,y \in M$ eine Inverse, so besitzt auch $x \circ y$ eine Inverse.
- Das neutrale Element ist seine eigene Inverse ($e \circ e = e$ ).
- Die Inverse der Inversen von x ergibt wieder x.