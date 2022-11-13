Aufgabe A8 (Summen und Produktformeln)

Schreiben Sie folgende Ausdrücle in Kurzform mithilfe von $\sum$ und $\prod$ Zeichen (Die Kreuze $\times$ stehen dabei für Produktzeichen)

A = $\frac{1}{2} + \frac{3}{4} + \frac{5}{8} + .... + \frac{21}{2048}$ 
B = $\frac{1}{2 \times 9 \times 64 \times625}$ 

$$A =\sum_{k=1}^{11} (\frac{2k -1}{2^{k}} )$$
$$ B = \prod_{n=1}^{4} (\frac{1}{(n+1)^{n}})$$



Aufgabe A9 (vollständige Induktion)

Beweisen Sie mittels vollständiger Induktion: Für alle $n \in \mathbb{N}$ ist die Anzahl der Möglichkeiten die Elemente einer beliebigen n-elementartigen Menge anzuordnen gegeben durch

$$ n! := \prod_{k=1}^{n} k = n \cdot (n-1) \cdot (n-2) \cdot ... \cdot 1.$$
(n+1)! = (n+1) n!
(0+1)! = (0+1) 0!
1 = 1 0!
1 = 0!



Aufgabe A10 (vollständige Induktion)

Schreiben Sie folgenden Ausdruck mithilfe von $\sum$ und/oder $\prod$ Zeichen und beweisen Sie mittels vollständiger Induktion, dass für alle $n \in \mathbb{N}$, mit n $\ge$ 2 gilt

$$S(n) = \frac{1}{1+n} + \frac{1}{1+ (n+1)} + ... + \frac{1}{2n} > \frac{13}{24}.$$

$$n! := \prod_{k=1}^{n}$$


A 11 (Justins Rätsel)


Beweise mithilfe der vollständigen Induktion, dass $\forall n \in \mathbb{N_{0}}$ folgendes gilt:


$2^{3n} + 6$ ist durch 7 teilbar
$\Leftrightarrow 2^{3n} + 6 =  7 \cdot k \mid k \in \mathbb{N}$
$\Leftrightarrow \frac{2^{3n} + 6}{7} = k \mid k \in \mathbb{N}$ 


Es $\exists n \in \mathbb{N} \mid 2^{3}+ 6$ ist durch 7 teilbar. Wenn es für ein beliebeiges n in den natürlichen Zahlen gilt, so muss es auch für n+1 gelten.

$\Rightarrow \frac{2^{3(n+1)} + 6}{7}= k \mid k \in \mathbb{N}$ 

$2^{3} \cdot 2^{5} = 2^{5+3} =  2^{8}$ 
$2^{3(n+1)} = 2^{3n +3} = 2^{3n} \cdot 2^{3} = 8 \cdot 2^{3n}$ 
 $\Rightarrow  \frac{2^{3(n+1)} + 6}{7}= k \mid k \in \mathbb{N}  \Rightarrow \frac{2^{3n+3} + 6}{7}= k \mid k \in \mathbb{N}  \Rightarrow \frac{2^{3n} \cdot 2^{3} + 6}{7}= k \mid k \in \mathbb{N}$ 
$\Rightarrow \frac{8 \cdot 2^{3n}  + 6}{7}= k \mid k \in \mathbb{N}$  
$\Rightarrow \frac{7 \cdot 2^{3n} + 2^{3n}  + 6}{7}= k \mid k \in \mathbb{N}$  
$\Rightarrow \frac{7 \cdot 2^{3n}}{7} + \frac{2^{3n}  + 6}{7}= k \mid k \in \mathbb{N}$
Sei $\frac{2^{3n}  + 6}{7} = p \mid p \in \mathbb{N}$ 
 $\Rightarrow \frac{7 \cdot 2^{3n}}{7} + p= k \mid k \in \mathbb{N}$
 $\Rightarrow 2^{3n} + p= k \mid k \in \mathbb{N}$
 $2^{3n} \in \mathbb{N}, p \in \mathbb{N} \Rightarrow k \in \mathbb{N}$
 $2^{3(n+1)} + 6$ ist durch 7 teilbar
 $\Rightarrow \forall n \in \mathbb{N_{0}} \Rightarrow 2^{3n} + 6$ ist durch 7 teilbar
 


