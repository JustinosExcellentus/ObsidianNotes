
## Definition

>Eine Verknüpfung ist eine Relation zwischen einem geordneten Paar $(x,y) \in M \times M$ und einem Element $z \in M$ mit $(x,y) \rightarrow z \quad \mid x \circ y = z$  beziehungsweise die Abbildung $\circ: M \times M \rightarrow M$ .
>Man schreibt auch $x \circ y := \circ(x,y)$ 


## Beispiele

- auf $\mathbb{N}_0: \quad +: \mathbb{N}_0 \times\mathbb{N}_0 \rightarrow \mathbb{N}_0, \quad (x,y) \rightarrow x+y$  
- auf $\mathbb{N}_0: \quad \cdot:\mathbb{N}_0 \times \mathbb{N}_0 \rightarrow \mathbb{N}_0, \quad (x,y) \rightarrow x \cdot y$  
"-" Verknüpfung existiert nicht in $\mathbb{N}_0$ , da x - y mit y > x nicht mehr in $N_0$ liegt/
- Auf $\mathbb{Z}$ existieren die Verknüpfungen $(+, \cdot)$ wie in $\mathbb{N}_0$ 
- auf $\mathbb{Z}: \quad -: \mathbb{Z} \times \mathbb{Z} \rightarrow \mathbb{Z}, \quad (x,y) \rightarrow x-y$ 
- auf $\mathbb{Q}$ existieren die Verknüpfungen $(+, \cdot, -)$ wie in $\mathbb{Z}$ 
- "/" Verknüpfung existiert nicht in $\mathbb{Q}$ , da für einen Nenner y = 0 jene Zahl nicht mehr in $\mathbb{Q}$ liegt.
- auf $\mathbb{Q} \setminus \{ 0\}: \quad \mathbb{Q} \times \mathbb{Q} \rightarrow \mathbb{Q}, \quad (x,y) \rightarrow x : y = x /y = \frac{x}{y}$  




## Eigenschaften einer Verknüpfung 

- $\circ$ assoziativ:    für alle $x,y,z \in M$ gilt:     $x \circ (y \circ z) = (x\circ y) \circ z$ 
- $\circ$ kommutativ: für alle $x,y \in  M$ gilt:    $x \circ y = y \circ x$ 

#### Neutrales Element

##### Definition

>Eine neutrales Element bezüglich $\circ: \quad e \in M$, sodass für alle $x \in M$ gilt:
>$e \circ x = x = x \circ e$ 

##### Bemerkung
>Es gibt höchstens ein neutrales Element bezüglich $\circ$ 

##### Beweis

Seien e, e' zwei neutrale Elemente bezüglich $\circ$ . 
Daraus folgt: $e=e \circ e' = e'$ . Somit gilt, dass $e = e'$ gilt. Also existiert nur ein neutrales Element bezüglich $\circ$ .

#### Beispiele

- Neutrales Element der Verknüpfung + ist 0, da  $x \circ e = x + 0 = x$ gilt.
- Neutrales Element der Verknüpfung $\cdot$ ist 1, da  $x \circ e = x \cdot 1 = x$ gilt.
- Neutrales Element der Verknüpfung $*$ (Vektormultiplikation) ist der Einheitsvektor v mit
 $$\begin{align}
    v &= \begin{pmatrix}
          1 \\
           1 \\
           \vdots \\
           1
         \end{pmatrix}
, da \: x \circ  v= 
\begin{pmatrix}
          x_1\\
           x_2 \\
           \vdots \\
           x_n
         \end{pmatrix}

    *
          \begin{pmatrix}
          1 \\
           1 \\
           \vdots \\
           1
         \end{pmatrix} = \begin{pmatrix}
          x_1\\
           x_2 \\
           \vdots \\
           x_n
         \end{pmatrix}
  \end{align}$$ 
gilt.


Neutrales Element der Verknüpfung $*$ (Matrixmultiplikation) ist die Einheitsmatrix I mit
 $$\begin{align}
    v &= \begin{pmatrix}
          1 & 0 & ... & 0 \\
           0 & 1 & ... & 0 \\
           \vdots & \vdots & \vdots & \vdots \\
           0 & 0 & ... & 1
         \end{pmatrix}
, da \: x \circ  

    v= \begin{pmatrix}
          a_{1,1} & a_{1,2} & ... & a_{1,n} \\
           a_{2,1} & a_{2,2} & ... & a_{2,n} \\
           \vdots & \vdots & \vdots & \vdots \\
           a_{n,1} & a_{n,2} & ... & a_{n,n}
         \end{pmatrix}
    *
    \begin{pmatrix}
          1 & 0 & ... & 0 \\
           0 & 1 & ... & 0 \\
           \vdots & \vdots & \vdots & \vdots \\
           0 & 0 & ... & 1
         \end{pmatrix}
            = \begin{pmatrix}
           a_{1,1} & a_{1,2} & ... & a_{1,n} \\
           a_{2,1} & a_{2,2} & ... & a_{2,n} \\
           \vdots & \vdots & \vdots & \vdots \\
           a_{n,1} & a_{n,2} & ... & a_{n,n}
         \end{pmatrix}
  \end{align}$$ 
gilt.


#### Inverses Element

Sei e das neutrale Element bezüglich $\circ$  und sei x $\in M$ .


##### Linksinverses Element

>Linksinverses Element zu x bezüglich $\circ$ ist ein $y \in M$ , sodass folgendes gilt:
> $y \circ x = e$ 

##### Rechtsinverses Element

> Rechtsinverses Element zu x bezüglich $\circ$ ist ein $y \in M$ , sodass folgendes gilt:
> $x \circ y = e$ 

##### Inverses Element

> Inverses  Element zu x bezüglich $\circ$ ist ein $y \in M$ , dass sowohl links- als auch rechtsinverses Element von x ist:
> $x \circ y = e  = y \circ x$ 


##### Bemerkung

- Sei M eine Menge und $\circ$ eine assoziative Menge Verknüpfung auf M
- Sei e das neutrale Element bezüglich $\circ$ und $x \in M$.


Dann existiert höchstens ein inverses Element x bezüglich $\circ$ .

##### Beweis:

Seien y, y' inverse Element zu x.
Daraus folgt $y =  y \cdot e = y \cdot (x \cdot y') \overset{AG}{=} (y \cdot x) \cdot y' = e \cdot y' = y'$ 
Also existiert nur ein inverses Element, da y = y' gilt.


##### Beispiele

-Inverses  Element der Menge $\mathbb{Z}$ bezüglich der Verknüpfung $+$ von $x \in \mathbb{Z}$  ist (-x), da  $y \circ x = (-x) + x = 0 = e = x + (-x) = x \circ y$  gilt.
-Inverses  Element der Menge $\mathbb{Q} \setminus \{ 0 \}$ bezüglich der Verknüpfung $\cdot$ von $x \in \mathbb{Z}$  ist $\frac{1}{x}$ , da  $y \circ x = \frac{1}{x} \cdot x = 1 = e = x \cdot \frac{1}{x} = x \circ y$  gilt.
- Für (nichtsinguläre) Matrizen $A \in \mathbb{R}^{n \times n} \quad  \mid det(M) \neq 0$ existiert eine inverse Matrix $A^{-1}$, sodass A bezüglich der Matrixmultipikation ein inverses Element besitzt $y \circ x =  A^{-1} \cdot A = I = e = A \cdot A^{-1} = x \circ y$ .


