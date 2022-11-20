

Idee: Grenzwert soll Funktionswert sein, bzw. wenn x wenig variiert, soll f(x) auch wenig variieren.



Definition:

Eine Funktion $f: \mathbb{D} \subset \mathbb{R} \rightarrow \mathbb{R}$  heißt stetig in $x \in \mathbb{D}$, wenn
$\forall \varepsilon, \exists \delta = \delta(x,c)$, sodass $\vert x - x_0 \vert \leq \delta \Rightarrow \vert f(x) - f(x_0) \vert \leq \varepsilon \quad \forall x \in \mathbb{D}$
Zu jeder gewünschten Genauigkeit $\varepsilon$ von  $f(x_0)$ (Auswertung) findet sich eine erlaubte Abweichung $\delta$ von $x_0$, sodass die Abweichung $f(x_0)$ $\varepsilon$-genau ist.

Bemerkung 

a) Stetigkeit hängt vom Auswertungspunkt $x_0 \in \mathbb{D}$ ab.
Außerdem hängt das $\delta$ von $\varepsilon$ und $x_0$ ab

b)  Bild 


c) Auswertungen von stetigen Funktionen in Computer sind "stabil" bzw. "robust"

Satz: Ist f stetig bei x = a, so gilt $\lim_{x \rightarrow a}  f(x)$   = f($\lim_{x \rightarrow a}$ x) = f(a) und umgekehrt.

Beweis (Nur stetig $\Rightarrow \lim_{x \rightarrow a}  f(x) = f(a)$ )

Zu zeigen: Für folge mit lim n-> unendlich xn = a gilt lim(x.> a) (x) = a

Voraussetzung: $\forall \varepsilon >0, \exists \delta > 0, \vert x - a\vert , \Rightarrow \vert f(x) - f(a) \vert \leq \varepsilon$ 

Wegen Definition von lim : $\forall \varepsilon > 0 \exists n_{\varepsilon} \in \mathbb{N} \mid f(n_{\varepsilon}) - f(a) \vert \leq \varepsilon \quad n > n_{\varepsilon}$
Wegen Stetigkeit ex. ein $\delta_{\varepsilon}$ sodass $\vert x - a \vert \leq \delta _{\varepsilon} , \forall x \in \mathbb{R}$ 
Wähle nun $n_{\varepsilon} \in \mathbb{N},$ sodass $\vert x_n - a \vert \leq \delta _{\varepsilon} \forall n > n_{\varepsilon}$ (geht wegen der Konvergenz der Folge)



Beispiele:

1) $x, x^2, sin(x), e^x$ sind stetig auf $\mathbb{R}$
2) $\frac{1}{x}$ ist stetig auf $\mathbb{R} \setminus \{0 \}$ , $ln(x)$ ist stetig für x > 0
3) $f: [0;\infty ) \rightarrow \mathbb{R}; x \rightarrow \sqrt{x}$ stetig auf $[0; \infty)$ .
Beweis: Zunächst sei $x_0 = 0$. Sei $\{ x_n\}$ Folge mit ...

Genauigkeit $\delta(x_0) = \vert f(x) - f(x_0) \vert  =  \vert \sqrt{x_n} - \sqrt{x_0} \vert = \vert  \frac{x_n - x_0}{\sqrt{x_n} - \sqrt{x_0}}  \vert \leq \frac{x_n - x_0}{\sqrt{x_n}}$ -> 0.


$x_0 = 0$ mit $\varepsilon - \delta - Kriterium$ :

Sei $\delta_{\varepsilon} = \varepsilon ^2 , dann \forall \varepsilon > 0 \exists \delta = \delta_{\varepsilon} = \varepsilon ^2$ 
$\vert x - x_0 \vert = \vert x \vert \leq \delta_{\varepsilon} \Rightarrow \vert f(x) - f(x_0) \vert = \sqrt{x} \leq \varepsilon$ , denn $\vert x \vert \leq \varepsilon ^2  \Rightarrow \sqrt{x} \leq \varepsilon$ 


4) f(x) = $\frac{x^2 - 4}{x-2}$ ist stetig auf  R ohne 2.
Die stetige Fortsetzung benutzt den Grenzwert lim x-> 2 f(x) = 4. 
g(x) = $\frac{x^2 - 4}{x-2}$ für x $\in \mathbb{R} \setminus \{2\}$ , 4 für x = 2


Satz: Seien f und g stetig bei $x_0$, Dann sind $\alpha g + \beta f$ mit $\alpha, \beta \in \mathbb{R}$, $f \cdot g, \frac{f}{g} (f(x_0) \neq 0)$  auch stetig in $x_0$, Desweiteren ist $f \circ g$ stetig, falls f stetig bei $g(x_0)$ 

Beispiel

1) f(x) = 1  mit $x \in \mathbb{Q}$ und 0 mit $x \notin \mathbb{Q}$ ist $\forall x \in \mathbb{D}$  nicht stetig 




#### Verfeinerte Stetigkeitsbegriffe

Definition 

1) f heißt gleichmäßig stetig, falls $\forall y \in \mathbb{D}
gilt $\forall \varepsilon > 0 \exists \delta : \delta (\varepsilon) > 0 ,$ sodass $\vert x - y \vert \leq \delta  \Rightarrow \vert f(x) - f(y) \vert \leq \varepsilon \quad \forall x \in \mathbb{D}$ 

2) f heißt  Lipschitz-stetig, falls für alle $x,y \in \mathbb{D} \quad \exists L > 0$ mit $\vert f(x) - f(y) \vert \leq L \vert x - y \vert$ 
3) f heißt Kontraktion , falls f Lipschitz-stetig mit L $\leq$ 1 ist


Bemerkung 

a) Es gilt für alle Funktion f: $\mathbb{R} \rightarrow \mathbb{R}$ :
- g : g stetig $\subset$ f
- h: h gleichmäßig stetig $\subset$ g
- k: k Lipschitz-stetig $\subset$ h
- m : m Kontraktion $\subset$ k

b) f(x) = $\frac{1}{x}$ 
$\Rightarrow$ nicht gleichmäßig-stetig, denn die Stetigkeit liefert die erlaubte Abweichung bei $x_0$ also $\delta(\varepsilon , x_0) = x_0 \frac{\varepsilon x_0}{2x_0 + 1} \quad x_0 \in (0,1) \quad \delta = 0$ 

c) Lipschitz-Funktionen verlaufen überall in $\mathbb{D}$ in einem Kegel mit maximaler/minimaler Steigung L.
c.1) $\sqrt{x}$ ist nicht Lipschitz-stetig, aber ist gleichmäßig-stetig



Satz

>Jede Lipschitz-Funktion ist gleichmäßig-stetig


d) Kontraktion haben Kegel mit Steigung zwischen $\pm 1$ 
z.B. $f(x) = x, f(x) = x^2$ ist Kontraktion für $x \in (\frac{-1}{2}, \frac{1}{2})$


Satz (Zwischenwertsatz):

>Sei f auf [a,b] stetig und f(a) < 0, f(b) > 0. Dann hat f in [a,b] mindestens eine Nullstelle.

Beweis: 

Bisektion:

$a_0 = a, b_0 = b$ 
Für $k = 1,2,..$ : Iteriere k mit t = $\frac{a_k + b_k}{2}.
Falls f(t) < 0, dann ist $a_{k+1} = t, b_{k+1} = b_k$
Falls f(t) > 0, dann ist $a_{k+1} = a_k, b_{k+1} = t$

Es gilt f(a_k) < 0, f(b_k) > 0 \forall k = 0,1,....
Der Abstand $b_k - a_k$ fällt monoton (Halbierung)

Folge $a_k$ ist monoton wachsend und beschränkt durch b $\Rightarrow$ es existiert $\lim_{n \rightarrow \infty} a_k$ 

Folge $a_k$ ist monoton fallend und beschränkt durch a $\Rightarrow$ es existiert $\lim_{n \rightarrow \infty} b_k$ 

Es muss wegen $\vert b_k - a_k \vert \rightarrow 0 gelten $\xi := \lim_{n \rightarrow \infty} a_k = \lim_{n \rightarrow \infty} b_k$
Behauptung: f($\xi$)=0.
Wäre f($\xi$) > 0, dann existiert $\vert x - \xi \vert \leq \delta \Rightarrow \vert f(x) - f(\xi) \vert \leq \varepsilon$ und zusätzlich f(x) > 0 für $x \in [ \delta - \xi, \delta + \xi ]$ muss ein $a_k$ enthalten, denn $a_k \rightarrow \xi$ monoton von unten. $a_k < \xi$ 
$\Rightarrow$ Widerspruch, denn $f(a_k) < 0$

Bem:

a) Dieses Verfahren wird tatsächlich benutzt
b) Allgemein gilt: Ist f stetig auf [a,b], dann wird jeder Wert im Invervall [f(a), f(b)] angenommen.
c) Folgerung f : $[a,b] \rightarrow \mathbb{R}$ hat ein Maximum/Minimun in $[a,b]$, eventuell am Rand. 

=> Differentialrechnung

