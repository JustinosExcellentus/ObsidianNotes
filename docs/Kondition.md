---
aliases: [Kondition, Konditionszahl]

tags:
- Numerik_I
---


Definition: 

Eine Kondition beschreibt die Empfindlichkeit von Fehlern in der Eingabe in Bezug auf die Fehler in der Ausgabe

 Kondition bei Vektoren

Sei $$x = \left ( \begin{matrix} x_{1}\\ x_{2}\\ x_{3}\\ ...\\ x_{n} 
\end{matrix} \right )$$ Dann ist  $f(x)$ und $\nabla f(x)$ 
$$f(x) =  \left (\begin{array}{r}

f(x_{1})\\
f(x_{2})\\
f(x_{3})\\
.....\\
f(x_{n})\\
\end{array} \right ), \nabla f(x) = \left (\begin{array}{r}
\frac{\partial f(x_{1})}{\partial x_{1}}\\
\frac{\partial f(x_{2})}{\partial x_{2}}\\
\frac{\partial f(x_{3})}{\partial x_{3}}\\
.....\\
\frac{\partial f(x_{n})}{\partial x_{n}}\\
\end{array} \right )$$

Für einen fehlerhaften Vektor $\tilde{x}$ gilt nun laut Taylorpolynom 1. Ordnung an der Entwicklungsstelle x: 
$f(\tilde{x}) = f(x) + (\nabla f(x))^{T} \cdot (\tilde{x} -x) \Rightarrow \frac{f(\tilde{x}) - f(x)}{f(x)}  = \sum_{j=1}^{n} (\frac{\partial f(x)}{\partial x_{j}} \cdot \frac{x_{j}}{f(x)}) \cdot \frac{\tilde{x}_{j} - x_{j}}{x_{j]}} \dot{\leq} max_{1 \leq j \leq n}  (\frac{\partial f(x)}{\partial x_{j}} \cdot \frac{x_{j}}{f(x)}) =  max_{1 \leq j \leq n} (\phi _{i} (x)) := \kappa_{rel}$



Beispiele zur Kondition

Sei $f: \mathbb{R} \rightarrow \mathbb{R}, f(x) = e^{3x^{2}}$ 
Für $\kappa_{rel} =  \vert \frac{f'(x)}{f(x)} \cdot x \vert = 6x^{2}$ 
Für $x  << 1 \Rightarrow r_{x} > r_{f} \Rightarrow$ Funktion ist gut konditioniert
Für $x  >> 1 \Rightarrow r_{x} <  r_{f} \Rightarrow$ Funktion ist schlecht konditioniert

Für $x = 0.1$ und $\tilde{x} =0.10001$ gilt $\kappa _ {rel} (0.1) = 6 \cdot 10 ^{-2}$ 
Also gilt für die Größenordnung, dass sich f(x) verbessern muss.
$r_{x} =10^{-4}, r_{f} = 6 \cdot 10^{-6} \Rightarrow$ Gut konditioniert  

Für $x = 4$ und $\tilde{x} =4.0004$ gilt $\kappa _ {rel} (0.1) = 96$ 
Also gilt für die Größenordnung, dass sich f(x) verbessern muss.
$r_{x} =10^{-4}, r_{f} = 9 \cdot 10^{-3} \Rightarrow$ Schlecht  konditioniert   


Kondition bei Multiplikation


\Sei $f : \mathbb{R^{2}} \rightarrow \mathbb{R}$ mit $f(x_{1},x_{2}) = x_{1} \cdot x_{2}$    $\vert  x_{1}, x_{2} \in \mathbb{R}$ 
Berechnen der Verstärkungsfaktoren $\phi_{1}, \phi_{2}$ 
$\phi_{1}(x) = \frac{\partial f(x)}{\partial x_{1}} \cdot \frac{x_{1}}{f(x)}$ = $x_{2}\cdot \frac{x_{1}}{x_{1} \cdot x_{2}}$ = 1
$\phi_{2}(x) = \frac{\partial f(x)}{\partial x_{2}} \cdot \frac{x_{2}}{f(x)}$ = $x_{1}\cdot \frac{x_{2}}{x_{1} \cdot x_{2}}$ = 1
$\kappa_{rel} = max_{1 \leq j \leq 2} ( \phi_{j})$ = 1 $\Rightarrow$ Kondition ist unabhängig von x$\Rightarrow$ Sehr gut konditioniert

Kondition bei Addition


Sei $f : \mathbb{R^{2}} \rightarrow \mathbb{R}$ mit $f(x_{1},x_{2}) = x_{1} + x_{2}$    $\vert  x_{1}, x_{2} \in \mathbb{R}$ 
Berechnen der Verstärkungsfaktoren $\phi_{1}, \phi_{2}$ 
$\phi_{1}(x) = \frac{\partial f(x)}{\partial x_{1}} \cdot \frac{x_{1}}{f(x)}$ = $\frac{x_{1}}{x_{1} + x_{2}}$ 
$\phi_{2}(x) = \frac{\partial f(x)}{\partial x_{2}} \cdot \frac{x_{2}}{f(x)}$ = $\frac{x_{2}}{x_{1} + x_{2}}$ 
$\kappa_{rel} = max_{1 \leq j \leq 2} ( \phi_{j})$ = $max \{ \vert  \frac{x_{1}}{x_{1} + x_{2}}\vert, \vert  \frac{x_{2}}{x_{1} + x_{2}}\vert\} \Rightarrow$  Für $x_{1}, x_{2} \in \mathbb{R}^{+} \Rightarrow \kappa_{rel} \leq 1 \Rightarrow$ Sehr gut konditioniert. Für $ x_{1} \approx -x_{2}$ ist der Bruch sehr klein $\Rightarrow \kappa_{rel} >> 1 \Rightarrow$ Sehr schlecht konditioniert

Kondition bei Nullstellen

Für die kleinere Nullstelle $y*$ der Funktion  $f(y) = y^{2} - 2y x _{1} + x_{2}$  mit $x_{1}, x_{2} \in \mathbb{R}$ gilt $y* = x_{1} - \sqrt{x_{1}^{2}-x_{2}}$ 

Berechnung der Konditionszahl aus $max \{ \phi_{1} , \phi_{2}\}$ 

Wenn $x_{2} < 0 \Rightarrow \phi_{1} \leq 1$ und $\kappa _{rel} \leq 1 \Rightarrow$  Gut konditioniert. Ist $x_{1} > 0, x_{2} > 0, x_{1} \approx x_{2}$ ist $\phi_{1} >> 1 und \kappa_{rel} >> 1 \Rightarrow$ Schlecht konditioniert, im schlimmsten Fall existiert durch einen Fehler keine Nullstelle mehr, falls $x_{1}^{2} \ge x_{2} \land \tilde{x_{1}}^{2} < \tilde{x_{2}}$ gilt.

Kondition bei Matrizen 

Sei $f: \mathbb{R}^{n} \rightarrow \mathbb{R}^{n}$ , $f$ linear.
Sei $B \in \mathbb{R}^{n \times n}$, mit $det(B) \neq 0$  \\
$f(x) = Bx$  bzw. $B^{-1}f(x) = x$ (i).\\

Für die gestörte Eingabe $\tilde{x}$ gilt:\\
$f(\tilde{x})  = B\tilde{x}$      $\vert -f(x)$ \\
$f(\tilde{x})  -f(x) = B\tilde{x} - f(x) = B \tilde {x} - Bx = B(\tilde{x} - x)$        $\vert /f(x) : f(x) \neq 0$ \\
$\frac{f(\tilde{x})  -f(x) }{f(x)} = \frac{B(\tilde{x} - x)}{f(x)} \Rightarrow  \frac{\vert \vert f(\tilde{x})  -f(x) \vert \vert}{\vert \vert f(x)\vert \vert} = \frac{\vert \vert B(\tilde{x} - x)\vert \vert}{\vert \vert f(x)\vert \vert}$ 
$x = B^{-1}f(x) \Rightarrow \vert \vert x \vert \vert = \vert \vert B^{-1}f(x) \vert \vert \leq \vert \vert B^{-1} \vert \vert \cdot \vert \vert f(x) \vert \vert$ 
Da $\vert \vert x \vert \vert , \vert \vert f(x) \vert \vert > 0$ gilt: $\frac{\vert \vert x \vert \vert}{\vert \vert B^{-1} \vert \vert} \leq \vert \vert f(x) \vert \vert   \Rightarrow  \frac{f(\tilde{x})  -f(x) }{f(x)} = \frac{B(\tilde{x} - x)}{f(x)} \leq  \vert \vert B \vert \vert \cdot \vert \vert B^{-1} \vert \vert \cdot \frac{\vert \vert \tilde{x} -x \vert \vert}{\vert \vert x \vert \vert}$ 
Hierbei gilt $\kappa_{rel} =  \vert \vert B \vert \vert \cdot \vert \vert B^{-1} \vert \vert$  

Beispiel Schnittpunkte

Bestimmung des Schnittpunktes von 2 Geraden:
$u_{1} + 1.001 u_{2} = 1.999 6$
$u_{1} + 1.997 u_{2} = 4.003$ 

Es ergibt die Lösung $u = A^{-1} b$ mit 
$$A = \left (\begin{array}{rr} 
3 & 1.001 \\
6 & 1.997 


\end{array} \right ), b = \left (\begin{array}{c} 
1.99 \\
4.003


\end{array} \right ) \rightarrow  u = \left (\begin{array}{c} 
1 \\
-1



\end{array} \right ) \\\\$$


Da wir auf $\mathbb{R}^{n}$ abbilden, aber $\kappa _{rel} \in \mathbb{R}$ ist, benutzen wir die Vektornorm um auf $\mathbb{R}$ abbzubilden.  Für die Norm von f(x) gilt : $\vert \vert f(x) \vert \vert = \vert \vert Bx \vert \vert$ Für die gestörte Eingabe $\tilde{x}$ gilt:
$\vert  \vert f(\tilde{x})$ 

