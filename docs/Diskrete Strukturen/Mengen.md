---
aliases: []

tags:
- Analysis_fuer_Informatik
- Diskrete_Strukturen
---


## Mengendefinition

#### Vorstellung einer Menge

> Unter einer **Menge** verstehen wir jede Zusammenfassung von bestimmten wohlunterscheidbaren Objekten unserer Anschauung oder unseres Denkens zu einem Ganzen.
> -Georg Cantor, 1895

Bei dieser Definition ergibt sich das Menge-Aller-Mengen-Problem. Dadurch muss auf bestimmte Mengenkonstruktionen beschränkt werden.

#### Definition

> Eine **Menge** M hat die Eigenschaft, dass für ein beliebiges Objekt x gilt, dass es entweder ein Element der Menge ist ($x \in M$), oder nicht ($x \notin M$).

Daraus ergibt sich, dass für ein beliebiges Objekt x und eine beliebige Menge der Term "$x \in M$" eine Aussage ist, also laut [[Aussagenlogik]] eine Aussageform ist. Darüber können wir die Menge definieren als Zusammenfassung aller Objekte x, für die die Aussage A(x) wahr ist.

## Eigenschaften von Mengen

#### Definition Teilmengen

> Seien M und N Mengen.
> - N $\subseteq$ M $\Leftrightarrow$ $\forall x \in N$ ist $x \in M$ 
> - N $\nsubseteq$ M $\Leftrightarrow$ $\lnot ( N \subseteq M)$
> - N = M $\Leftrightarrow$ N $\subseteq$ M $\land$ M $\subseteq$ N

#### Definition Mächtigkeit

> Sei M eine Menge
> - M heißt *endlich* , wenn M nur endlich viele Elemente besitzt. Ansonsten ist M unendlich.
> - Wenn M endlich ist, steht |M| für die Anzahl der Elemente von M
> - Wenn M unendlich ist, ist |M| = $\infty$ .
> - |M| heißt die Mächtigkeit der Menge M




## Darstellung von Mengen


#### Darstellung von Menge

Mengen werden in Mengenklammern eingeschlossen und durch Trennzeichen werden die einzelnen Elemente angegeben. Reihenfolge und Wiederholungen spielen hierbei keine Rolle:
- {-3, 1, 45}
- {1, 4, 9, 16, 25, 36}
- {1, 3, 5, 7, 9, 11, 13, ...}

#### Beschreibung von Mengen

Mengen können durch Worte beschrieben werden :
- Menge der natürlichen Zahlen
- Menge der Quadratzahlen
- Menge an Einwohner in Aachen


#### Aussondern

>Sei M eine Menge und A(x) eine Aussageform, wobei x mit den Elementen von M belegt werden kann. Dann ist 
>$$
\{ x \in M \mid A(x) \:ist \: wahr\}
$$
 eine Menge, nämlich die Teilmenge von M.

- $\{ x \in M \mid x \: ist \: ungerade\}$
- $\{ x \in M \mid x > 5\}$
- $\{ x \in M \mid x^2 = 9\}$


#### Beschreibung durch mathematische Symbole

Durch [[Mathematische Symbole]] können Mengen beschrieben werden.

#### Beispiele

- $\emptyset = \underline{0} \subseteq \underline{1} \subseteq \underline{2} \subseteq ... \subseteq \underline{\mathbb{N}} \subseteq \underline{\mathbb{Z}} \subseteq \underline{\mathbb{Q}} \subseteq \underline{\mathbb{R}} \subseteq \underline{\mathbb{C}}$
- $\{ 1, 2, 3, 4\} \nsubseteq \{ 2, 3, 4, 5, 6, 7\}$
- $\{ x \in \mathbb{R} \mid x^2 = -1 \} = \emptyset$
- $\{ x \in \mathbb{R} \mid x^3 + 2x = 3x^2\}  = \{ 0, 1, 2\}$ 