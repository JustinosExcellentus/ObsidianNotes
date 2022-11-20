

Die eulersche Zahl ist eine transzendente Zahl, die von Leonhard Euler definiert worden ist als $\lim_{n \rightarrow \infty} \left ( 1+ \frac{1}{n}\right)^n$ 



#### Herleitung der eulerschen Zahl

Dazu betrachten wir uns die Definition der Ableitung an (h-Methode) als:
$$\lim_{h \rightarrow 0} \frac{f(x+h) -f(x)}{h}$$
Für eine Exponentialfunktion $f(x) = a^x$ gilt demnach:
$$\lim_{h \rightarrow 0} \frac{f(x+h) -f(x)}{h}=\lim_{h \rightarrow 0} \frac{a^{x+h} -a^x}{h} =\lim_{h \rightarrow 0} \frac{a^{x}\cdot a^h -a^x}{h} =\lim_{h \rightarrow 0} \frac{a^{x} \cdot (a^h-1)}{h} =a^{x} \cdot lim_{h \rightarrow 0} \frac{ (a^h-1)}{h} = f(x) \cdot lim_{h \rightarrow 0} \frac{ (a^h-1)}{h}$$ Somit ergibt die Ableitung bis auf einen Faktor wieder die Funktion. Nun betrachten wir den Fall, dass f(x) = f'(x), also $\lim_{h \rightarrow 0} \frac{ (a^h-1)}{h} = 1$ ergibt.

Es gilt:

$\lim_{h \rightarrow 0} \frac{ (a^h-1)}{h} = 1 \quad \mid \cdot h$ 
$\Leftrightarrow \lim_{h \rightarrow 0}  a^h-1 = h \quad \mid +1$
$\Leftrightarrow \lim_{h \rightarrow 0}  a^h = h + 1 \quad \mid ()^{\frac{1}{h}} \: oder \: \sqrt [h]{}$ 
$\Leftrightarrow \lim_{h \rightarrow 0}  (a^h)^{\frac{1}{h}} = (1+h)^{\frac{1}{h}} \quad$ 
$\Leftrightarrow \lim_{h \rightarrow 0}  a = (1+h)^{\frac{1}{h}} \quad \mid Wir \: definieren \: n := \frac{1}{h} \Leftrightarrow h = \frac{1}{n}$ 
$\Leftrightarrow \lim_{n \rightarrow \infty}  a= (1+ \frac{1}{n})^{n} \quad \mid$

Nun muss gezeigt werden, dass diese Folge tatsächlich konvergiert.