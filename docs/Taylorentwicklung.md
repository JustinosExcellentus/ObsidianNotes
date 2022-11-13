---
aliases: [Taylorpolynom]

tags:
- Numerik_I
---


Gegeben sei eine skalare Funktion f : $\mathbb{R} \rightarrow \mathbb{R}$ 
Dann gilt für $f(x)$ an einem Betrachtungspunkt $(x \rightarrow x_{0})$:
$f(x) = p_{k-1} + \mathcal{O}(|x-x_{0}|^{k})$  

Für k = 1 gilt der Mittelwertsatz => Taylorpolynom ist eine Verallgemeinerung dessen. 
Für eine Funktion $f(x_{i,j}) : \mathbb{R}^{2} \rightarrow \mathbb{R}$ gilt für ihre zweite Ableitung $f''(x_{i,j}) = \frac{\partial^{2}f(x)}{\partial i \partial j}$.

Sei eine Funktion $f : \mathbb{R} \rightarrow \mathbb{R}$ .
Dann sei $\tilde{x}$ die gestörte Eingabe, $x$ der exakte Wert und $\Delta x$ der absolute Fehler. Dann gilt $\tilde{x} = x + \Delta x$ .Bilden wir über $\tilde{x}$ die Taylor-Reihe 1. Ordnung  über den Entwicklungspunkt $x$ :
$f(\tilde{x}) = f(x) + f'(x) \cdot (\tilde{x} - x) + \mathcal{O}(|\tilde{x} - x|^{2})$ . 

Der letzte Term ist wiederum vernachlässigbar, wir wollen nicht den exakten Wert, sondern nur die Größenordnung.  $f(x) + f'(x) \cdot (\tilde{x} - x) + \mathcal{O}(|\tilde{x} - x|^{2}) \dot{=} f(x) + f'(x) \cdot (\tilde{x} - x)$ , also gilt 
$f(\tilde {x} ) = f'(x) \cdot (\tilde{x} -x)$    $\vert -f(x)$  
$f(\tilde{x}) - f(x) = f'(x) \cdot (\tilde{x} - x)$    $\vert / f(x) : f(x) \neq 0$ 
$\frac{f(\tilde{x}) - f(x)}{f(x)}= \frac{f'(x)}{f(x)} \cdot (\tilde{x} - x)$ = $\frac{f(\tilde{x}) - f(x)}{f(x)}= \frac{f'(x)}{f(x)} \cdot x \cdot \frac{\tilde{x} - x}{x}$   $| x \neq 0$ .

$\frac{f(\tilde{x}) - f(x)}{f(x)}$ sei der relative Ausgabefehler, $\frac{\tilde{x} - x}{x}$ sei der relative Eingabefehler. $\frac{f'(x)}{f(x)} \cdot x$ ist damit die Fehlerverstärkung. Da uns nur die Größenverhältnisse interessieren, nehmen wir de Betrag davon.   $\vert \frac{f'(x)}{f(x)} \cdot x \vert$ Dies wird auch die Konditionszahl $\kappa_{rel}$ genannt.  

$\kappa_{rel}$ stellt die Fehlerverstärkung aus einem Eingabefehler in den Ausgabefehler dar, deswegen gilt: $\kappa_{rel} > 1 \Rightarrow r_{f} > r_{x}$ . Je größer $\kappa_{rel}$ ist, desto sensitiver reagiert $f$ auf Fehler in der Eingabe. Für $\kappa_{rel} < 1 \Rightarrow r_{f} < r_{x}$ . Je kleiner $\kappa _{rel}$ ist, desto weniger sensitiv reagiert f auf Fehler in der Eingabe.