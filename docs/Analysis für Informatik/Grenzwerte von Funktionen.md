Definition

$\lim_{x \rightarrow \infty} f(x) = b$ 


Bemerkungen 

a) b muss nicht Funktionswert sein
b) b $\pm \infty$ ist möglich (bestimmte Divergenz)
c) Für Folgen xn < a heißt der Grenzwert linksseitig, für >a rechtsseitig


Bspe: a) f(x) = x (zwischen 0 und 1) U x+1 (x $\geq$ 1)
$\lim_{x \rightarrow 2} f(x) = 3, \lim_{x \rightarrow 1} f(x)$  existiert nicht
Linksseitig ist 1
Rechtsseitig ist 2

2) f(x) = sin x, $x \in \mathbb{R} \setminus \{ \frac{\pi}{2} \}, 2 \: für \: x = \frac{\pi}{2}$ 


$\lim_{x \rightarrow 2} f(x) = sin(2) = 0,....$ 
$\lim_{x \rightarrow \frac{\pi}{2}} f(x) = sin(\frac{\pi}{2}) = 1 \neq f(\frac{\pi}{2})$


3) $f: \mathbb{R} \setminus \{2 \} \rightarrow \mathbb{R}, x \rightarrow f(x) = \frac{x^2 -4}{x-2}$
$\lim_{x \rightarrow 2} = ?$
Wähle $\{ x_n\}_{n \in \mathbb{N}} \quad x_n \neq 2 mit \lim_{n \rightarrow \infty} x_n = 2$ 
$f(x_n) = \frac{x_n^2 - 4}{x_n -2} = \frac{(x_n - 2)(x_n +2)}{x_n -2}$



4) f(x) = $1 : x \in \mathbb{Q}, , 0 : x \notin \mathbb{Q}$
$\lim_{x \rightarrow a} f(x)$ existiert für kein $a \in \mathbb{R}$
$x_n \in$($\frac{a-1}{n}, \frac{a+1}{n}$) und $x \in \mathbb{Q}$ , $\lim_{x \rightarrow a} f(x) = 1$ (1)

$x_n \in \mathbb{R}$ mit $x_n \in (a -\frac{1}{n}, a + {1}{n})$ und $x_n \notin \mathbb{Q}, \lim_{x \rightarrow a} f(x) = 0$ (2)

(1) und (2) kreiren einen Widerspruch


5) $f(x) = e^{-\frac{1 }{x}} \mid x \neq 0$

$\lim_{x \rightarrow 0} f(x)$ existier nicht.
$\lim_{x \rightarrow 0+} f(x) = 0
$\lim_{x \rightarrow 0-} f(x) = \infty


6) $f(x) = \frac{1}{x-2}$
[Linke seite - unendlich, rechte seite plus unendlich]



7) f(x) = $\frac{sin(x)}{x}$
$\lim_{x \rightarrow 0} f(x) = \lim_{x \rightarrow 0} \frac{sin(x)}{x} = \lim_{x \rightarrow 0} \frac{x - \frac{ x^3}{6} + \frac{x^5}{5!} +.... }{x} = \lim_{x \rightarrow 0} 1 - \frac{ x^2}{6} + \frac{x^4}{5!} +.... = 1$  


Bem:

$\lim_{x \rightarrow 0} f(x)$ mit $a = \pm \infty$ heißt uneigentlicher Grenzwert
d.h $\{ x_n\}_{n \rightarrow \infty}$


Bsp. Merksätze

1) Limes x unendlich 1/ x = 0
2) Limes x unendlich sin(x) ex. nicht (schwingt zwischen $[-1; 1]$ )
3) Limes x unendlich $\frac{e^x}{x^p} = \infty$ mit $p \in \mathbb{R}$ , folg aus Exponentialreihe $e^x = \sum_{k=0}^{\infty} \left ( \frac{x^k}{k!} \right)$ 
4) Limes x unendlich $\frac{ln(x)}{x^p} = 0$, da jede Polynomfunktion schneller wächst als jede Logarithmusfunktion
5) Limes x gegen 0 $x \cdot sin (\frac{1}{x}) = \lim_{y \rightarrow \infty} \frac{1}{y} \cdot sin(y) =  \lim_{y \rightarrow \infty} \frac{sin(y)}{y}$ 
