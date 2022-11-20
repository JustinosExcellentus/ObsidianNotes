---
aliases: [Zahlen]

tags:
- Analysis_fuer_Informatik
---

Die wichtigste Menge der Mathematik sind die natürlichen Zahlen $\mathbb{N} = \{1,2,3,4,...\}$  

1) $\mathbb{N}$ lässt sich axiomatisch definieren, oder aus den reellen Zahlen herleiten
2) $\mathbb{N} \cup \{0 \} = \mathbb{N_{0}}$ 
3) Für die Mächtigkeit einer Menge A ("Anzahl") schreiben wir $\vert A \vert$ , zum Beispiel $\vert 0 \vert = 0, \vert \{ a,b,c \} \vert  = 3, \vert \infty \vert:= \vert \mathbb{N} \vert$ 
4) $\infty$ ist keine natürliche Zahl

Die natürlichen Zahlen erlauben "Beweise durch Induktion"



Satz : Betrachte die Summe 1+2+3+...+n $= \sum_{k=1}^{n} (k)$ . $\forall n \in \mathbb{N}$  gilt : $= \sum_{k=1}^{n} (k) = \frac{n(n+1)}{2}$ 

Beweis: (Durch Induktion) Induktionsverankerung (hier n =1)
$$ \sum_{k=1}^{1} (k) = 1 = \frac{1(1+1)}{2}$$


Induktionsschritt (n -1 gegeben, beweise den Fall n)
Es gelte also $\sum_{k=1}^{n-1} (k) = \frac{(n-1)(n)}{2}$  (Induktionsvoraussetzung)

Zu zeigen: $\sum_{k=1}^{n} (k) = \frac{n(n+1)}{2}$ , es folgt $\sum_{k=1}^{n} (k)= \sum_{k=1}^{n-1} (k) + n =  \frac{(n-1)(n)}{2} + n = \frac{n(n+1)}{2}$ q.e.d

Allgemeines Vorgehen bei Induktion: zu beweisen $A(n) \forall n \in \mathbb{N}$ 

1) Verankerung
2) Induktionsvoraussetzung (Es gilt A(n-1) oder A(n))
3) Induktionsschritt (A(n-1) $\Rightarrow$ A(n) oder A(n) $\Rightarrow$ A(n+1) )


Direkter Beweis: Beim direkten Beweis wird aus der Voraussetzung die Aussage B direkt hergeleitet. A $\Rightarrow$ B.
Satz: $forall n \in \mathbb{N} :  \sum_{k=1}^{n} (k) = \frac{n(n+1)}{2}$ .

Beweis: 
  $S_{n} = 1 + 2 + 3 ... (n-1) + n$
  $S_{n} = n + (n-1) + (n-2) ... (2) + 1$
  Beides aufaddiert ergibt = $2S_{n} = (n+1) + (n+1) +...+ (n+1)$ 
  $\Rightarrow 2S_{n} = n(n+1) \Rightarrow S_{n} = \frac{n(n+1)}{2}$ q.e.d

Indirekter Beweis: Beweis durch Widerspruch: Wir nehmen das Gegenteil der Aussage A ($\lnot A)$ an und leiten etwas offensichtlich falsches ab, dann muss die Aussage $\lnot A$ falsch gewesen sein. Daraus folgen wir, dass die ursprüngliche Annahme falsch sein muss.

Satz: Es gibt unendlich viele Primzahlen

Beweis: Annahme: Es gibt endlich viele Primzahlen, $p_{n}$  ist die höchste Primzahl . Die Menge aller Primzahlen $\mathbb{P} = \{ p_{1}, p_{2}, p_{3},...,p_{n} \}$  
Nun schauen wir uns den Term $\prod_{k =1}^{n} (p_{k}) =  p_{1} \cdot p_{2} \cdot p_{3} \cdot ... \cdot p_{n}$   an. Addieren wir auf diesen Term 1 auf, so ist dieser Term nicht mehr durch eine Primzahl teilbar, da immer ein Rest von 1 bleibt. So ist diese Zahl eine Primzahl, die nicht in unserer Menge liegt.







Die reellen Zahlen

Def: Für eine Menge $\mathbb{R}$ seien folgende Bedingungen erfüllt:

1) Es gibt zwei Verknüpfungen $(+, \cdot)$ und $(\mathbb{R} , +, \cdot)$ ist ein Körper-
2) Es gibt eine Ordnungsrelation "$\leq$" auf $\mathbb{R}$ verträglich mit + und $\cdot$ , das heißt für $x,y,z \in \mathbb{R}$ gilt
a) $x \leq y \Rightarrow x + z \leq y +z$ 
b) $0 \leq x \land  0 \leq y \Rightarrow 0 \leq x \cdot y$ 

3) (Vollständigkeitsaxion) Jede nichtleere nach ben beschränkte Telmenge $A \subseteq \mathbb{R}$ besitzt eine kleinste obere Schranke.

Dann heißt $\mathbb{R}$ reeller Zahlenkörper und die Elemente reelle Zahlen, wir schreiben $x \in \mathbb{R}$ .

 Bemerkungen:
 1) Damit ist $\mathbb{R}$ im Prinzip eindeutig definiert
 2) Wegen der Anordnung kann man $\mathbb{R}$ als orientierten Zahlenstrahl vorstellen
$$ 
\usepackage{tikz}
\begin{tikzpicture}[thick]
    \draw(0,0)--(12.5,0);
    \foreach \x/\xtext in {0/0,3/1,6/2,9/3,12/4}
      \draw(\x,0pt)--(\x,3pt) node[above] {\xtext};
    \foreach \x in {0,1,...,12}
      \draw(\x,0pt)--(\x,-3pt) node[below] {\frac{\x}{3}};
  \end{tikzpicture}$$
  
3) Aus "$\leq$" leiten wir "<", "$\ge$" und ">" her.
4) Wir definieren offene und geschlossene  Intervalle
$[a,b] := \{  x \in \mathbb{R} \vert a \leq x \leq b \}$
$(a,b) := \{  x \in \mathbb{R} \vert a < x < b \}$ 


Definition: Für $x \in \mathbb{R}$ sei der (Absolut-)Betrag defiiert durch
$\vert x \vert = \{x : x \ge 0 \vert -x : x < 0 \}$ 

Lemma: Für $x,y \in \mathbb{R}$ gilt
1) $\vert x+y \vert \leq \vert x \vert + \vert y \vert$ (Dreiecksungleichung)
2) $\vert x \vert - \vert y \vert \leq \vert x-y \vert$ (Umgekehrte Dreiecksungleichung)

Beweis zu 1) : $\vert x+y \vert \leq \vert x \vert + \vert y \vert$ 
$\Leftrightarrow \vert x+y \vert ^{2} \leq \vert x \vert ^{2} + \vert y \vert ^{2}$ 
$\Leftrightarrow x^{2} + 2xy + y^{2} \leq \vert x \vert ^{2} + 2\vert x\vert \cdot \vert y \vert + \vert y \vert ^{2}$ 
$\Leftrightarrow 2xy \leq 2\vert xy \vert$ 
$\Leftrightarrow xy \leq \vert xy \vert$
Es gilt $a \leq \vert a \vert$   $\forall a \in \mathbb{R}$ 


  
 