
---
aliases: [Algebra]

tags:
- Analysis_fuer_Informatik
---


$\mathbb{N} \Rightarrow$ Addition gegeben, aber kein Inverses für jede Zahl
Lösung: Erweiterung von $\mathbb{N}$ 
$\mathbb{N} \rightarrow \mathbb{Z} \Rightarrow$ Löst das Inverse für jede Zahl, vollständig gegenüber der Addition, aber es gibt kein Inverses für die Multiplikation
Lösung: Erweiterung von $\mathbb{Z}$ 
$\mathbb{Z} \rightarrow \mathbb{Q} \Rightarrow$ Löst das Inverse für jede Zahl gegenüber der Multiplikation, vollständig gegenüber der Multiplikation, aber es gibt keine Lösung zum Problem $\sqrt{2}$ .

Satz: $\nexists n \in \mathbb{Q} : n^{2} = 2$

Beweis: Annahme $n \in \mathbb{Q} \Rightarrow n = \frac{p}{q} :$ p und q sind teilerfremd
$n^{2} = 2 \Leftrightarrow \frac {p^{2}}{q^{2}} \Leftrightarrow p^{2} = 2q^{2} \Leftrightarrow p \_ gerade$ 
Sei $r = \frac{p}{2} \in \mathbb{Z} \Rightarrow p = 2r$ 




Definition: Eine Teilmenge$A \subseteq \mathbb{R}$ heißt von oben beschränkt, falls ein $b \in \mathbb{R}$ existiert, mit  $a \subseteq b$   $\forall a \in A.$  Desweiteren heißt $s \in \mathbb{R}$ kleinste obere Schranke für A falls s eine obere Schranke ist und für jede andere Schranke $b \in \mathbb{R}$ von A gilt $s \subseteq b$ .

Bemerkung:
1) Analog für von unten beschränkt und die größte untere Schranke
2) Wir benutzen das Supremum für die kleinste obere Schranke
$sup$  $A := min \{ b \in \mathbb{R} \vert a \leq b$    $\forall a \in A\}$ 
und das Infimum für die größte untere Schranke
$inf$  $A := max \{ b \in \mathbb{R} \vert a \ge b$    $\forall a \in A\}$ 

3) Falls sup $A \in A$, so ist das Supremum das Maximum max A und falls inf $A \in A$, so ist das Infimum das Minimum min A

Beispiel:

A = (0,1) = $\{ x \in \mathbb{R} \vert 0 < x < 1 \}$ 
max A = ?, sup A = 1

A = [0,1] = $\{ x \in \mathbb{R} \vert 0 \leq x \leq 1 \}$ 
max A = sup A =1

A = $\{ a \in \mathbb{Q} \vert a^{2} \leq 2 \} \subseteq \mathbb{Q}$ 
sup A $\notin \mathbb{Q}$ 
A = $\{ a \in \mathbb{R} \vert a^{2} \leq 2 \} \subseteq \mathbb{R}$ 
sup A $\in \mathbb{R}$ nach Vollständikeitsaxiom
sup A = $\sqrt{2}$ 


Satz: Für zwei reelen Zahlen $a,b \in \mathbb{R}$ mit $a<b$ existiert ein $r \in \mathbb{Q}$  mit $a < r < b$ . "$\mathbb{Q}$ liegt dicht in $\mathbb{R}$"


Bemerkungen:
1) Die Dichtheit bedeutet, wir können reelle Zahlen beliebig gut durch rationale Zahlen approximieren, $\forall \epsilon > 0$ , $\exists r \in \mathbb{Q} : x < r < x + \epsilon \vert x \in \mathbb{R}$  
2) Man kann ähnlich beweisen dass $sup \{ a \in \mathbb{R} \vert a^{2} < 2\} =  \sqrt{2}$
3) Das Vollständigkeitsaxion wird später (durch Folgen) mehr Sinn erhalten.


